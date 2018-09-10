# <a name="deviceexchangeaccessstatesummary-resource-type"></a><span data-ttu-id="9182d-101">deviceExchangeAccessStateSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9182d-101">deviceExchangeAccessStateSummary resource type</span></span>

> <span data-ttu-id="9182d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9182d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9182d-103">设备 Exchange 访问状态摘要</span><span class="sxs-lookup"><span data-stu-id="9182d-103">Device Exchange Access State summary</span></span>
## <a name="properties"></a><span data-ttu-id="9182d-104">属性</span><span class="sxs-lookup"><span data-stu-id="9182d-104">Properties</span></span>
|<span data-ttu-id="9182d-105">属性</span><span class="sxs-lookup"><span data-stu-id="9182d-105">Property</span></span>|<span data-ttu-id="9182d-106">类型</span><span class="sxs-lookup"><span data-stu-id="9182d-106">Type</span></span>|<span data-ttu-id="9182d-107">说明</span><span class="sxs-lookup"><span data-stu-id="9182d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9182d-108">allowedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9182d-108">allowedDeviceCount</span></span>|<span data-ttu-id="9182d-109">Int32</span><span class="sxs-lookup"><span data-stu-id="9182d-109">Int32</span></span>|<span data-ttu-id="9182d-110">Exchange 访问状态为允许的设备总数。</span><span class="sxs-lookup"><span data-stu-id="9182d-110">Total count of devices with Exchange Access State: Allowed.</span></span>|
|<span data-ttu-id="9182d-111">blockedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9182d-111">blockedDeviceCount</span></span>|<span data-ttu-id="9182d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="9182d-112">Int32</span></span>|<span data-ttu-id="9182d-113">Exchange 访问状态为阻止的设备总数。</span><span class="sxs-lookup"><span data-stu-id="9182d-113">Total count of devices with Exchange Access State: Blocked.</span></span>|
|<span data-ttu-id="9182d-114">quarantinedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9182d-114">quarantinedDeviceCount</span></span>|<span data-ttu-id="9182d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="9182d-115">Int32</span></span>|<span data-ttu-id="9182d-116">Exchange 访问状态为隔离的设备总数。</span><span class="sxs-lookup"><span data-stu-id="9182d-116">Total count of devices with Exchange Access State: Quarantined.</span></span>|
|<span data-ttu-id="9182d-117">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9182d-117">unknownDeviceCount</span></span>|<span data-ttu-id="9182d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="9182d-118">Int32</span></span>|<span data-ttu-id="9182d-119">Exchange 访问状态为未知的设备总数。</span><span class="sxs-lookup"><span data-stu-id="9182d-119">Total count of devices with Exchange Access State: Unknown.</span></span>|
|<span data-ttu-id="9182d-120">unavailableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9182d-120">unavailableDeviceCount</span></span>|<span data-ttu-id="9182d-121">Int32</span><span class="sxs-lookup"><span data-stu-id="9182d-121">Int32</span></span>|<span data-ttu-id="9182d-122">无法找到其 Exchange 访问状态的设备总数。</span><span class="sxs-lookup"><span data-stu-id="9182d-122">Total count of devices for which no Exchange Access State could be found.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9182d-123">关系</span><span class="sxs-lookup"><span data-stu-id="9182d-123">Relationships</span></span>
<span data-ttu-id="9182d-124">无</span><span class="sxs-lookup"><span data-stu-id="9182d-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9182d-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9182d-125">JSON Representation</span></span>
<span data-ttu-id="9182d-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9182d-126">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```








