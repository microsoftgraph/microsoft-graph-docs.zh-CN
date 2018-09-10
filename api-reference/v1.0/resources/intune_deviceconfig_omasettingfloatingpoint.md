# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="c04fd-101">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="c04fd-101">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="c04fd-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c04fd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c04fd-103">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="c04fd-103">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="c04fd-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c04fd-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c04fd-105">属性</span><span class="sxs-lookup"><span data-stu-id="c04fd-105">Properties</span></span>
|<span data-ttu-id="c04fd-106">属性</span><span class="sxs-lookup"><span data-stu-id="c04fd-106">Property</span></span>|<span data-ttu-id="c04fd-107">类型</span><span class="sxs-lookup"><span data-stu-id="c04fd-107">Type</span></span>|<span data-ttu-id="c04fd-108">说明</span><span class="sxs-lookup"><span data-stu-id="c04fd-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c04fd-109">displayName</span><span class="sxs-lookup"><span data-stu-id="c04fd-109">displayName</span></span>|<span data-ttu-id="c04fd-110">String</span><span class="sxs-lookup"><span data-stu-id="c04fd-110">String</span></span>|<span data-ttu-id="c04fd-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c04fd-111">Display Name.</span></span> <span data-ttu-id="c04fd-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c04fd-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c04fd-113">description</span><span class="sxs-lookup"><span data-stu-id="c04fd-113">description</span></span>|<span data-ttu-id="c04fd-114">字符串</span><span class="sxs-lookup"><span data-stu-id="c04fd-114">String</span></span>|<span data-ttu-id="c04fd-115">说明。</span><span class="sxs-lookup"><span data-stu-id="c04fd-115">Description.</span></span> <span data-ttu-id="c04fd-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c04fd-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c04fd-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="c04fd-117">omaUri</span></span>|<span data-ttu-id="c04fd-118">String</span><span class="sxs-lookup"><span data-stu-id="c04fd-118">String</span></span>|<span data-ttu-id="c04fd-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="c04fd-119">OMA.</span></span> <span data-ttu-id="c04fd-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c04fd-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="c04fd-121">value</span><span class="sxs-lookup"><span data-stu-id="c04fd-121">value</span></span>|<span data-ttu-id="c04fd-122">单个</span><span class="sxs-lookup"><span data-stu-id="c04fd-122">Single</span></span>|<span data-ttu-id="c04fd-123">值。</span><span class="sxs-lookup"><span data-stu-id="c04fd-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c04fd-124">关系</span><span class="sxs-lookup"><span data-stu-id="c04fd-124">Relationships</span></span>
<span data-ttu-id="c04fd-125">无</span><span class="sxs-lookup"><span data-stu-id="c04fd-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c04fd-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c04fd-126">JSON Representation</span></span>
<span data-ttu-id="c04fd-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c04fd-127">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```








