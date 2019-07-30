# GetVersion {#doc_api_composer_GetVersion .reference}

查询某个工作流的某个特定版本信息

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=composer&api=GetVersion&type=RPC&version=2018-12-12)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|FlowId|String|是|lc-abcdefg|需要查询的工作流编排实例的 ID

 |
|VersionId|Integer|是|10|需要查询的版本

 |
|Action|String|否|GetVersion|系统规定参数。取值：GetVersion。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|D264C934-2DA8-44B4-B034-C659A63AC659|本次请求 ID

 |
|FlowId|String|lc-abcdefg|当前版本所属工作流编排实例的 ID

 |
|RegionId|String|cn-shanghai|当前工作流编排实例所属地域

 |
|VersionId|Integer|10|当前版本

 |
|VersionName|String|test|版本名称

 |
|VersionStatus|String|Enabled|版本状态，Enabled 表示启用中

 |
|VersionDescription|String|这是版本描述|版本描述

 |
|Definition|String|\{\\"schemaVersion\\":\\"2018-12-12\\",\\"actions\\":\{\},\\"version\\":\\"1.0.0\\",\\"triggers\\":\{\}\}|当前版本对应的工作流定义

 |
|CreateTime|String|2018-12-12T07:36:22.992Z|版本创建时间

 |
|UpdateTime|String|2018-12-12T07:36:22.992Z|版本最后更新时间

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=GetVersion
&FlowId=lc-abcdefg
&VersionId=10
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<root>
    <RequestId>D264C934-2DA8-44B4-B034-C659A63AC659</RequestId>
    <FlowId>lc-abcdefg1</FlowId>
    <RegionId>cn-shanghai</RegionId>
    <VersionId>10</VersionId>
    <VersionName>test</VersionName>
    <VersionStatus>Enabled</VersionStatus>
    <VersionDescription>这是版本描述</VersionDescription>
    <Definition>{"schemaVersion":"2018-12-12","actions":{},"version":"1.0.0","triggers":{}}</Definition>
    <CreateTime>2018-12-12T07:36:22.992Z</CreateTime>
    <UpdateTime>2018-12-12T07:36:22.992Z</UpdateTime>
</root>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"CreateTime":"2018-12-12T07:36:22.992Z",
	"RegionId":"cn-shanghai",
	"RequestId":"D264C934-2DA8-44B4-B034-C659A63AC659",
	"FlowId":"lc-abcdefg1",
	"UpdateTime":"2018-12-12T07:36:22.992Z",
	"VersionId":10,
	"VersionStatus":"Enabled",
	"VersionDescription":"这是版本描述",
	"Definition":"{\"schemaVersion\":\"2018-12-12\",\"actions\":{},\"version\":\"1.0.0\",\"triggers\":{}}",
	"VersionName":"test"
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/composer)查看更多错误码。

