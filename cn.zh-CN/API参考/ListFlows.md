# ListFlows {#doc_api_composer_ListFlows .reference}

查询工作流编排实例列表

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=composer&api=ListFlows&type=RPC&version=2018-12-12)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|Action|String|否|ListFlows|系统规定参数。取值：ListFlows。

 |
|FlowName|String|否|test|过滤特定的流程名称

 |
|PageNumber|Integer|否|1|当前页码

 |
|PageSize|Integer|否|10|每页返回的数量

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|Flows| | |工作流编排实例列表

 |
|CreateTime|String|2019-07-19T05:43:16.783Z|创建时间

 |
|FlowDescription|String|test flow|工作流编排实例的描述

 |
|FlowId|String|lc-abcdefg|工作流编排实例 ID

 |
|FlowName|String|test|工作流编排实例的名称

 |
|FlowStatus|String|Enabled|状态，Enabled 表示启用，Disabled 表示已禁用

 |
|RegionId|String|cn-shanghai|所属地域

 |
|UpdateTime|String|2019-07-19T05:43:16.783Z|最后更新时间

 |
|VersionId|Integer|1|当前最新版本

 |
|RequestId|String|1E70949F-F163-42C7-95FB-7346F9CA6D54|请求 ID

 |
|TotalCount|Integer|1|当前地域下工作流编排实例的总数

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=ListFlows
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<root>
    <TotalCount>1</TotalCount>
    <RequestId>1E70949F-F163-42C7-95FB-7346F9CA6D54</RequestId>
    <Flows>
        <Status>Enabled</Status>
        <FlowId>lc-azeugrfoceorod</FlowId>
        <CreatedAt>2019-07-19T05:52:00.287Z</CreatedAt>
        <CurrentVersion>10</CurrentVersion>
        <UpdatedAt>2019-07-27T10:48:42.797Z</UpdatedAt>
        <Name>test5</Name>
    </Flows>
</root>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"TotalCount":1,
	"RequestId":"1E70949F-F163-42C7-95FB-7346F9CA6D54",
	"Flows":[
		{
			"Status":"Enabled",
			"FlowName":"test",
			"RegionId":"cn-shanghai",
			"CreateTime":"2019-07-19T05:52:00.287Z",
			"FlowId":"lc-azeugrfoceorod",
			"UpdateTime":"2019-07-27T10:48:42.797Z",
			"VersionId":1,
			"FlowDescription":"test flow",
			"CurrentVersion":10
		}
	]
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/composer)查看更多错误码。

