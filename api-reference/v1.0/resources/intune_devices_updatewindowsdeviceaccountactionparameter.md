# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="31902-101">updateWindowsDeviceAccountActionParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="31902-101">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="31902-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="31902-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31902-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31902-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="31902-104">属性</span><span class="sxs-lookup"><span data-stu-id="31902-104">Properties</span></span>
|<span data-ttu-id="31902-105">属性</span><span class="sxs-lookup"><span data-stu-id="31902-105">Property</span></span>|<span data-ttu-id="31902-106">类型</span><span class="sxs-lookup"><span data-stu-id="31902-106">Type</span></span>|<span data-ttu-id="31902-107">说明</span><span class="sxs-lookup"><span data-stu-id="31902-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31902-108">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="31902-108">deviceAccount</span></span>|[<span data-ttu-id="31902-109">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="31902-109">windowsDeviceAccount</span></span>](../resources/intune_devices_windowsdeviceaccount.md)|<span data-ttu-id="31902-110">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31902-110">Not yet documented</span></span>|
|<span data-ttu-id="31902-111">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="31902-111">passwordRotationEnabled</span></span>|<span data-ttu-id="31902-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="31902-112">Boolean</span></span>|<span data-ttu-id="31902-113">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31902-113">Not yet documented</span></span>|
|<span data-ttu-id="31902-114">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="31902-114">calendarSyncEnabled</span></span>|<span data-ttu-id="31902-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="31902-115">Boolean</span></span>|<span data-ttu-id="31902-116">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31902-116">Not yet documented</span></span>|
|<span data-ttu-id="31902-117">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="31902-117">deviceAccountEmail</span></span>|<span data-ttu-id="31902-118">String</span><span class="sxs-lookup"><span data-stu-id="31902-118">String</span></span>|<span data-ttu-id="31902-119">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31902-119">Not yet documented</span></span>|
|<span data-ttu-id="31902-120">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="31902-120">exchangeServer</span></span>|<span data-ttu-id="31902-121">String</span><span class="sxs-lookup"><span data-stu-id="31902-121">String</span></span>|<span data-ttu-id="31902-122">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31902-122">Not yet documented</span></span>|
|<span data-ttu-id="31902-123">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="31902-123">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="31902-124">String</span><span class="sxs-lookup"><span data-stu-id="31902-124">String</span></span>|<span data-ttu-id="31902-125">尚未记录</span><span class="sxs-lookup"><span data-stu-id="31902-125">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="31902-126">关系</span><span class="sxs-lookup"><span data-stu-id="31902-126">Relationships</span></span>
<span data-ttu-id="31902-127">无</span><span class="sxs-lookup"><span data-stu-id="31902-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="31902-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31902-128">JSON Representation</span></span>
<span data-ttu-id="31902-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31902-129">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}-->
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



