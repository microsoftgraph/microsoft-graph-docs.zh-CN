# <a name="omasettingstring-resource-type"></a><span data-ttu-id="90dcf-101">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="90dcf-101">omaSettingString resource type</span></span>

> <span data-ttu-id="90dcf-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="90dcf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90dcf-103">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="90dcf-103">OMA Settings String definition.</span></span>

<span data-ttu-id="90dcf-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90dcf-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90dcf-105">属性</span><span class="sxs-lookup"><span data-stu-id="90dcf-105">Properties</span></span>
|<span data-ttu-id="90dcf-106">属性</span><span class="sxs-lookup"><span data-stu-id="90dcf-106">Property</span></span>|<span data-ttu-id="90dcf-107">类型</span><span class="sxs-lookup"><span data-stu-id="90dcf-107">Type</span></span>|<span data-ttu-id="90dcf-108">说明</span><span class="sxs-lookup"><span data-stu-id="90dcf-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90dcf-109">displayName</span><span class="sxs-lookup"><span data-stu-id="90dcf-109">displayName</span></span>|<span data-ttu-id="90dcf-110">String</span><span class="sxs-lookup"><span data-stu-id="90dcf-110">String</span></span>|<span data-ttu-id="90dcf-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="90dcf-111">Display Name.</span></span> <span data-ttu-id="90dcf-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90dcf-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="90dcf-113">description</span><span class="sxs-lookup"><span data-stu-id="90dcf-113">description</span></span>|<span data-ttu-id="90dcf-114">String</span><span class="sxs-lookup"><span data-stu-id="90dcf-114">String</span></span>|<span data-ttu-id="90dcf-115">说明。</span><span class="sxs-lookup"><span data-stu-id="90dcf-115">Description.</span></span> <span data-ttu-id="90dcf-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90dcf-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="90dcf-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="90dcf-117">omaUri</span></span>|<span data-ttu-id="90dcf-118">String</span><span class="sxs-lookup"><span data-stu-id="90dcf-118">String</span></span>|<span data-ttu-id="90dcf-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="90dcf-119">OMA.</span></span> <span data-ttu-id="90dcf-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="90dcf-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="90dcf-121">value</span><span class="sxs-lookup"><span data-stu-id="90dcf-121">value</span></span>|<span data-ttu-id="90dcf-122">String</span><span class="sxs-lookup"><span data-stu-id="90dcf-122">String</span></span>|<span data-ttu-id="90dcf-123">值。</span><span class="sxs-lookup"><span data-stu-id="90dcf-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90dcf-124">关系</span><span class="sxs-lookup"><span data-stu-id="90dcf-124">Relationships</span></span>
<span data-ttu-id="90dcf-125">无</span><span class="sxs-lookup"><span data-stu-id="90dcf-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="90dcf-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="90dcf-126">JSON Representation</span></span>
<span data-ttu-id="90dcf-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="90dcf-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



