# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="d5300-101">securityVendorInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5300-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="d5300-102">包含安全产品/服务提供商、提供程序和次级提供程序相关的详细信息（例如，vendor=Microsoft；provider=Windows Defender ATP；subProvider=AppLocker）。</span><span class="sxs-lookup"><span data-stu-id="d5300-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="d5300-103">属性</span><span class="sxs-lookup"><span data-stu-id="d5300-103">Properties</span></span>

| <span data-ttu-id="d5300-104">属性</span><span class="sxs-lookup"><span data-stu-id="d5300-104">Property</span></span>   | <span data-ttu-id="d5300-105">类型</span><span class="sxs-lookup"><span data-stu-id="d5300-105">Type</span></span>|<span data-ttu-id="d5300-106">说明</span><span class="sxs-lookup"><span data-stu-id="d5300-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d5300-107">provider \*</span><span class="sxs-lookup"><span data-stu-id="d5300-107">provider \*</span></span>|<span data-ttu-id="d5300-108">字符串</span><span class="sxs-lookup"><span data-stu-id="d5300-108">String</span></span>|<span data-ttu-id="d5300-109">特定提供程序 （产品/服务 — 非供应商公司）；例如，WindowsDefenderATP。</span><span class="sxs-lookup"><span data-stu-id="d5300-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="d5300-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="d5300-110">providerVersion</span></span>|<span data-ttu-id="d5300-111">字符串</span><span class="sxs-lookup"><span data-stu-id="d5300-111">String</span></span>|<span data-ttu-id="d5300-112">生成提示的提供程序或次级提供程序（如果存在）的版本。</span><span class="sxs-lookup"><span data-stu-id="d5300-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span>|
|<span data-ttu-id="d5300-113">subProvider</span><span class="sxs-lookup"><span data-stu-id="d5300-113">subProvider</span></span>|<span data-ttu-id="d5300-114">字符串</span><span class="sxs-lookup"><span data-stu-id="d5300-114">String</span></span>|<span data-ttu-id="d5300-115">特定次级提供程序（聚合提供程序之下）；例如，WindowsDefenderATP.SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="d5300-115">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="d5300-116">vendor \*</span><span class="sxs-lookup"><span data-stu-id="d5300-116">vendor \*</span></span>|<span data-ttu-id="d5300-117">字符串</span><span class="sxs-lookup"><span data-stu-id="d5300-117">String</span></span>|<span data-ttu-id="d5300-118">提示的供应商 (例如，Microsoft、Dell、FireEye) 的名称。</span><span class="sxs-lookup"><span data-stu-id="d5300-118">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span>|
<span data-ttu-id="d5300-119">（\* 表示必填字段。）</span><span class="sxs-lookup"><span data-stu-id="d5300-119">(\* Indicates a mandatory field.)</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5300-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5300-120">JSON representation</span></span>

<span data-ttu-id="d5300-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5300-121">The following is a JSON representation of the resource.</span></span>
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
