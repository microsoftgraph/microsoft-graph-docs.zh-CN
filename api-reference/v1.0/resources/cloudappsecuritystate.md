# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="2f09a-101">cloudAppSecurityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f09a-101">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="2f09a-102">包含有状态信息的云应用程序 （destinationServiceName、destinationServiceIp）。</span><span class="sxs-lookup"><span data-stu-id="2f09a-102">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="2f09a-103">属性</span><span class="sxs-lookup"><span data-stu-id="2f09a-103">Properties</span></span>

| <span data-ttu-id="2f09a-104">属性</span><span class="sxs-lookup"><span data-stu-id="2f09a-104">Property</span></span>     | <span data-ttu-id="2f09a-105">类型</span><span class="sxs-lookup"><span data-stu-id="2f09a-105">Type</span></span>        | <span data-ttu-id="2f09a-106">说明</span><span class="sxs-lookup"><span data-stu-id="2f09a-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2f09a-107">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="2f09a-107">destinationServiceIp</span></span>|<span data-ttu-id="2f09a-108">字符串</span><span class="sxs-lookup"><span data-stu-id="2f09a-108">String</span></span>|<span data-ttu-id="2f09a-109">连接到云应用程序/服务的目标 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="2f09a-109">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="2f09a-110">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="2f09a-110">destinationServiceName</span></span>|<span data-ttu-id="2f09a-111">字符串</span><span class="sxs-lookup"><span data-stu-id="2f09a-111">String</span></span>|<span data-ttu-id="2f09a-112">云应用程序/服务名称 （例如"销售"、"收存箱"等）。</span><span class="sxs-lookup"><span data-stu-id="2f09a-112">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="2f09a-113">riskScore</span><span class="sxs-lookup"><span data-stu-id="2f09a-113">riskScore</span></span>|<span data-ttu-id="2f09a-114">字符串</span><span class="sxs-lookup"><span data-stu-id="2f09a-114">String</span></span>|<span data-ttu-id="2f09a-115">提供程序生成/计算的云应用程序/服务风险评分。</span><span class="sxs-lookup"><span data-stu-id="2f09a-115">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="2f09a-116">建议值的范围为 0-1，相当于百分比。</span><span class="sxs-lookup"><span data-stu-id="2f09a-116">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f09a-117">JSON 表达式</span><span class="sxs-lookup"><span data-stu-id="2f09a-117">JSON representation</span></span>

<span data-ttu-id="2f09a-118">下面是资源的 JSON 表达式。</span><span class="sxs-lookup"><span data-stu-id="2f09a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->