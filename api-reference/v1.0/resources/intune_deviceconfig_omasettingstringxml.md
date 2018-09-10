# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="fa0d7-101">omaSettingStringXml 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa0d7-101">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="fa0d7-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa0d7-103">OMA 设置字符串 XML 定义。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-103">OMA Settings StringXML definition.</span></span>

<span data-ttu-id="fa0d7-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa0d7-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa0d7-105">属性</span><span class="sxs-lookup"><span data-stu-id="fa0d7-105">Properties</span></span>
|<span data-ttu-id="fa0d7-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa0d7-106">Property</span></span>|<span data-ttu-id="fa0d7-107">类型</span><span class="sxs-lookup"><span data-stu-id="fa0d7-107">Type</span></span>|<span data-ttu-id="fa0d7-108">说明</span><span class="sxs-lookup"><span data-stu-id="fa0d7-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa0d7-109">displayName</span><span class="sxs-lookup"><span data-stu-id="fa0d7-109">displayName</span></span>|<span data-ttu-id="fa0d7-110">String</span><span class="sxs-lookup"><span data-stu-id="fa0d7-110">String</span></span>|<span data-ttu-id="fa0d7-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-111">Display Name.</span></span> <span data-ttu-id="fa0d7-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa0d7-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fa0d7-113">description</span><span class="sxs-lookup"><span data-stu-id="fa0d7-113">description</span></span>|<span data-ttu-id="fa0d7-114">字符串</span><span class="sxs-lookup"><span data-stu-id="fa0d7-114">String</span></span>|<span data-ttu-id="fa0d7-115">说明。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-115">Description.</span></span> <span data-ttu-id="fa0d7-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa0d7-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fa0d7-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="fa0d7-117">omaUri</span></span>|<span data-ttu-id="fa0d7-118">String</span><span class="sxs-lookup"><span data-stu-id="fa0d7-118">String</span></span>|<span data-ttu-id="fa0d7-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-119">OMA.</span></span> <span data-ttu-id="fa0d7-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa0d7-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="fa0d7-121">fileName</span><span class="sxs-lookup"><span data-stu-id="fa0d7-121">fileName</span></span>|<span data-ttu-id="fa0d7-122">String</span><span class="sxs-lookup"><span data-stu-id="fa0d7-122">String</span></span>|<span data-ttu-id="fa0d7-123">与 Value 属性关联的文件名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-123">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="fa0d7-124">value</span><span class="sxs-lookup"><span data-stu-id="fa0d7-124">value</span></span>|<span data-ttu-id="fa0d7-125">Binary</span><span class="sxs-lookup"><span data-stu-id="fa0d7-125">Binary</span></span>|<span data-ttu-id="fa0d7-126">值。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-126">Value.</span></span> <span data-ttu-id="fa0d7-127">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="fa0d7-127">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa0d7-128">关系</span><span class="sxs-lookup"><span data-stu-id="fa0d7-128">Relationships</span></span>
<span data-ttu-id="fa0d7-129">无</span><span class="sxs-lookup"><span data-stu-id="fa0d7-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fa0d7-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa0d7-130">JSON Representation</span></span>
<span data-ttu-id="fa0d7-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa0d7-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```








