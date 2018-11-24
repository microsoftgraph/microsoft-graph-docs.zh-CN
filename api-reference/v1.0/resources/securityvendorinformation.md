# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="86d65-101">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="86d65-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="86d65-102">包含有关安全产品/服务供应商、 提供商和 subprovider 详细信息 (例如，供应商 = Microsoft; 提供程序 = Windows Defender ATP; subProvider = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="86d65-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="86d65-103">属性</span><span class="sxs-lookup"><span data-stu-id="86d65-103">Properties</span></span>

| <span data-ttu-id="86d65-104">属性</span><span class="sxs-lookup"><span data-stu-id="86d65-104">Property</span></span>   | <span data-ttu-id="86d65-105">类型</span><span class="sxs-lookup"><span data-stu-id="86d65-105">Type</span></span>|<span data-ttu-id="86d65-106">说明</span><span class="sxs-lookup"><span data-stu-id="86d65-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86d65-107">提供程序</span><span class="sxs-lookup"><span data-stu-id="86d65-107">provider</span></span> |<span data-ttu-id="86d65-108">字符串</span><span class="sxs-lookup"><span data-stu-id="86d65-108">String</span></span>|<span data-ttu-id="86d65-109">特定提供程序 （产品/服务 — 不供应商公司）;例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="86d65-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="86d65-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="86d65-110">providerVersion</span></span>|<span data-ttu-id="86d65-111">字符串</span><span class="sxs-lookup"><span data-stu-id="86d65-111">String</span></span>|<span data-ttu-id="86d65-112">提供程序或 subprovider，如果存在，生成警报的版本。</span><span class="sxs-lookup"><span data-stu-id="86d65-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="86d65-113">*Required*</span><span class="sxs-lookup"><span data-stu-id="86d65-113">*Required*</span></span>|
|<span data-ttu-id="86d65-114">subProvider</span><span class="sxs-lookup"><span data-stu-id="86d65-114">subProvider</span></span>|<span data-ttu-id="86d65-115">字符串</span><span class="sxs-lookup"><span data-stu-id="86d65-115">String</span></span>|<span data-ttu-id="86d65-116">特定 subprovider （下聚合提供程序）;例如，WindowsDefenderATP.SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="86d65-116">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="86d65-117">供应商</span><span class="sxs-lookup"><span data-stu-id="86d65-117">vendor</span></span> |<span data-ttu-id="86d65-118">字符串</span><span class="sxs-lookup"><span data-stu-id="86d65-118">String</span></span>|<span data-ttu-id="86d65-119">警报供应商 (例如，Microsoft，Dell FireEye) 的名称。</span><span class="sxs-lookup"><span data-stu-id="86d65-119">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="86d65-120">*Required*</span><span class="sxs-lookup"><span data-stu-id="86d65-120">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="86d65-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86d65-121">JSON representation</span></span>

<span data-ttu-id="86d65-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86d65-122">The folllowing is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
