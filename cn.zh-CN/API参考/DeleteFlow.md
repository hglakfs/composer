# DeleteFlow {#doc_api_composer_DeleteFlow .reference}

删除一个工作流编排实例

## 调试 {#api_explorer .section}

[您可以在OpenAPI Explorer中直接运行该接口，免去您计算签名的困扰。运行成功后，OpenAPI Explorer可以自动生成SDK代码示例。](https://api.aliyun.com/#product=composer&api=DeleteFlow&type=RPC&version=2018-12-12)

## 请求参数 {#parameters .section}

|名称|类型|是否必选|示例值|描述|
|--|--|----|---|--|
|FlowId|String|是|lc-abcdefg|需要删除的工作流编排实例 ID

 |
|Action|String|否|DeleteFlow|系统规定参数。取值：DeleteFlow。

 |

## 返回数据 {#resultMapping .section}

|名称|类型|示例值|描述|
|--|--|---|--|
|RequestId|String|D264C934-2DA8-44B4-B034-C659A63AC659|本次请求 ID

 |
|Success|Boolean|true|是否删除成功，true 表示删除成功

 |

## 示例 {#demo .section}

请求示例

``` {#request_demo}

http(s)://[Endpoint]/?Action=DeleteFlow
&FlowId=lc-abcdefg
&<公共请求参数>

```

正常返回示例

`XML` 格式

``` {#xml_return_success_demo}
<root>
    <RequestId>D264C934-2DA8-44B4-B034-C659A63AC659</RequestId>
    <Success>true</Success>
</root>
```

`JSON` 格式

``` {#json_return_success_demo}
{
	"RequestId":"D264C934-2DA8-44B4-B034-C659A63AC659",
	"Success":true
}
```

## 错误码 { .section}

访问[错误中心](https://error-center.aliyun.com/status/product/composer)查看更多错误码。

