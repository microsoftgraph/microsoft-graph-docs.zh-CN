# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="e4015-101">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4015-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="e4015-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e4015-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4015-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4015-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e4015-104">属性</span><span class="sxs-lookup"><span data-stu-id="e4015-104">Properties</span></span>
|<span data-ttu-id="e4015-105">属性</span><span class="sxs-lookup"><span data-stu-id="e4015-105">Property</span></span>|<span data-ttu-id="e4015-106">类型</span><span class="sxs-lookup"><span data-stu-id="e4015-106">Type</span></span>|<span data-ttu-id="e4015-107">说明</span><span class="sxs-lookup"><span data-stu-id="e4015-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4015-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="e4015-108">deviceAccount</span></span>|[<span data-ttu-id="e4015-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="e4015-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="e4015-110">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4015-110">Not yet documented</span></span>|
|<span data-ttu-id="e4015-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="e4015-111">passwordRotationEnabled</span></span>|<span data-ttu-id="e4015-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="e4015-112">Boolean</span></span>|<span data-ttu-id="e4015-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4015-113">Not yet documented</span></span>|
|<span data-ttu-id="e4015-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="e4015-114">calendarSyncEnabled</span></span>|<span data-ttu-id="e4015-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="e4015-115">Boolean</span></span>|<span data-ttu-id="e4015-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4015-116">Not yet documented</span></span>|
|<span data-ttu-id="e4015-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="e4015-117">deviceAccountEmail</span></span>|<span data-ttu-id="e4015-118">String</span><span class="sxs-lookup"><span data-stu-id="e4015-118">String</span></span>|<span data-ttu-id="e4015-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4015-119">Not yet documented</span></span>|
|<span data-ttu-id="e4015-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="e4015-120">exchangeServer</span></span>|<span data-ttu-id="e4015-121">String</span><span class="sxs-lookup"><span data-stu-id="e4015-121">String</span></span>|<span data-ttu-id="e4015-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4015-122">Not yet documented</span></span>|
|<span data-ttu-id="e4015-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="e4015-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="e4015-124">String</span><span class="sxs-lookup"><span data-stu-id="e4015-124">String</span></span>|<span data-ttu-id="e4015-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e4015-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4015-126">关系</span><span class="sxs-lookup"><span data-stu-id="e4015-126">Relationships</span></span>
<span data-ttu-id="e4015-127">无</span><span class="sxs-lookup"><span data-stu-id="e4015-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e4015-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4015-128">JSON Representation</span></span>
<span data-ttu-id="e4015-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4015-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```



