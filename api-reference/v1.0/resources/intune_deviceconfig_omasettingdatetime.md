# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="dd20f-101">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd20f-101">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="dd20f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dd20f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd20f-103">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="dd20f-103">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="dd20f-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dd20f-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dd20f-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd20f-105">Properties</span></span>
|<span data-ttu-id="dd20f-106">属性</span><span class="sxs-lookup"><span data-stu-id="dd20f-106">Property</span></span>|<span data-ttu-id="dd20f-107">类型</span><span class="sxs-lookup"><span data-stu-id="dd20f-107">Type</span></span>|<span data-ttu-id="dd20f-108">说明</span><span class="sxs-lookup"><span data-stu-id="dd20f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd20f-109">displayName</span><span class="sxs-lookup"><span data-stu-id="dd20f-109">displayName</span></span>|<span data-ttu-id="dd20f-110">String</span><span class="sxs-lookup"><span data-stu-id="dd20f-110">String</span></span>|<span data-ttu-id="dd20f-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="dd20f-111">Display Name.</span></span> <span data-ttu-id="dd20f-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dd20f-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="dd20f-113">description</span><span class="sxs-lookup"><span data-stu-id="dd20f-113">description</span></span>|<span data-ttu-id="dd20f-114">String</span><span class="sxs-lookup"><span data-stu-id="dd20f-114">String</span></span>|<span data-ttu-id="dd20f-115">说明。</span><span class="sxs-lookup"><span data-stu-id="dd20f-115">Description.</span></span> <span data-ttu-id="dd20f-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dd20f-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="dd20f-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="dd20f-117">omaUri</span></span>|<span data-ttu-id="dd20f-118">String</span><span class="sxs-lookup"><span data-stu-id="dd20f-118">String</span></span>|<span data-ttu-id="dd20f-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="dd20f-119">OMA.</span></span> <span data-ttu-id="dd20f-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dd20f-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="dd20f-121">value</span><span class="sxs-lookup"><span data-stu-id="dd20f-121">value</span></span>|<span data-ttu-id="dd20f-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd20f-122">DateTimeOffset</span></span>|<span data-ttu-id="dd20f-123">值。</span><span class="sxs-lookup"><span data-stu-id="dd20f-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd20f-124">关系</span><span class="sxs-lookup"><span data-stu-id="dd20f-124">Relationships</span></span>
<span data-ttu-id="dd20f-125">无</span><span class="sxs-lookup"><span data-stu-id="dd20f-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd20f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd20f-126">JSON Representation</span></span>
<span data-ttu-id="dd20f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd20f-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



