# CreateFlow {#doc_api_composer_CreateFlow .reference}

创建一个工作流编排实例

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=composer&api=CreateFlow&type=RPC&version=2018-12-12)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|FlowName|String|是|test|工作流编排实例的名称

 |
|Action|String|否|CreateFlow|系统规定参数。取值：CreateFlow。

 |
|Definition|String|否|\{\\"schemaVersion\\":\\"2018-12-12\\",\\"actions\\":\{\},\\"version\\":\\"1.0.0\\",\\"triggers\\":\{\}\}|工作流定义，需要将 JSON 格式化为 string

 |
|FlowDescription|String|否|这是一个工作流|工作流编排实例的描述

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|D264C934-2DA8-44B4-B034-C659A63AC659|请求 ID

 |
|FlowId|String|lc-abcdefg|创建后的工作流编排实例 ID

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=CreateFlow
&FlowName=test
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<root>
    <RequestId>D264C934-2DA8-44B4-B034-C659A63AC659</RequestId>
    <FlowId>lc-abcdefg</FlowId>
</root>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"RequestId":"D264C934-2DA8-44B4-B034-C659A63AC659",
	"FlowId":"lc-abcdefg"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/composer)查看更多错误码。

