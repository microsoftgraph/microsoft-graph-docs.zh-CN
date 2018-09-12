# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="80d18-101">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="80d18-101">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="80d18-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80d18-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80d18-103">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="80d18-103">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="80d18-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80d18-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80d18-105">属性</span><span class="sxs-lookup"><span data-stu-id="80d18-105">Properties</span></span>
|<span data-ttu-id="80d18-106">属性</span><span class="sxs-lookup"><span data-stu-id="80d18-106">Property</span></span>|<span data-ttu-id="80d18-107">类型</span><span class="sxs-lookup"><span data-stu-id="80d18-107">Type</span></span>|<span data-ttu-id="80d18-108">说明</span><span class="sxs-lookup"><span data-stu-id="80d18-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80d18-109">displayName</span><span class="sxs-lookup"><span data-stu-id="80d18-109">displayName</span></span>|<span data-ttu-id="80d18-110">字符串</span><span class="sxs-lookup"><span data-stu-id="80d18-110">String</span></span>|<span data-ttu-id="80d18-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="80d18-111">Display Name.</span></span> <span data-ttu-id="80d18-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80d18-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="80d18-113">说明</span><span class="sxs-lookup"><span data-stu-id="80d18-113">description</span></span>|<span data-ttu-id="80d18-114">字符串</span><span class="sxs-lookup"><span data-stu-id="80d18-114">String</span></span>|<span data-ttu-id="80d18-115">说明。</span><span class="sxs-lookup"><span data-stu-id="80d18-115">Description.</span></span> <span data-ttu-id="80d18-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80d18-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="80d18-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="80d18-117">omaUri</span></span>|<span data-ttu-id="80d18-118">字符串</span><span class="sxs-lookup"><span data-stu-id="80d18-118">String</span></span>|<span data-ttu-id="80d18-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="80d18-119">OMA.</span></span> <span data-ttu-id="80d18-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80d18-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="80d18-121">fileName</span><span class="sxs-lookup"><span data-stu-id="80d18-121">fileName</span></span>|<span data-ttu-id="80d18-122">字符串</span><span class="sxs-lookup"><span data-stu-id="80d18-122">String</span></span>|<span data-ttu-id="80d18-123">与值属性关联的文件名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="80d18-123">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="80d18-124">\*.crt</span><span class="sxs-lookup"><span data-stu-id="80d18-124">.crt</span></span> | <span data-ttu-id="80d18-125">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="80d18-125">\*.p7b</span></span> | <span data-ttu-id="80d18-126">\*.bin)。</span><span class="sxs-lookup"><span data-stu-id="80d18-126">Bin</span></span>|
|<span data-ttu-id="80d18-127">值</span><span class="sxs-lookup"><span data-stu-id="80d18-127">value</span></span>|<span data-ttu-id="80d18-128">字符串</span><span class="sxs-lookup"><span data-stu-id="80d18-128">String</span></span>|<span data-ttu-id="80d18-129">值。</span><span class="sxs-lookup"><span data-stu-id="80d18-129">Value.</span></span> <span data-ttu-id="80d18-130">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="80d18-130">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="80d18-131">关系</span><span class="sxs-lookup"><span data-stu-id="80d18-131">Relationships</span></span>
<span data-ttu-id="80d18-132">无</span><span class="sxs-lookup"><span data-stu-id="80d18-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80d18-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80d18-133">JSON Representation</span></span>
<span data-ttu-id="80d18-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80d18-134">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```








