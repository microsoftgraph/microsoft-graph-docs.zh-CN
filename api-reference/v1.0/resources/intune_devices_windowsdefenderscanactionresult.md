# <a name="windowsdefenderscanactionresult-resource-type"></a><span data-ttu-id="8c85d-101">windowsDefenderScanActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c85d-101">windowsDefenderScanActionResult resource type</span></span>

> <span data-ttu-id="8c85d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c85d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c85d-103">Windows Defender 最后扫描结果</span><span class="sxs-lookup"><span data-stu-id="8c85d-103">Windows Defender last scan result</span></span>

<span data-ttu-id="8c85d-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c85d-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c85d-105">属性</span><span class="sxs-lookup"><span data-stu-id="8c85d-105">Properties</span></span>
|<span data-ttu-id="8c85d-106">属性</span><span class="sxs-lookup"><span data-stu-id="8c85d-106">Property</span></span>|<span data-ttu-id="8c85d-107">类型</span><span class="sxs-lookup"><span data-stu-id="8c85d-107">Type</span></span>|<span data-ttu-id="8c85d-108">说明</span><span class="sxs-lookup"><span data-stu-id="8c85d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c85d-109">actionName</span><span class="sxs-lookup"><span data-stu-id="8c85d-109">actionName</span></span>|<span data-ttu-id="8c85d-110">String</span><span class="sxs-lookup"><span data-stu-id="8c85d-110">String</span></span>|<span data-ttu-id="8c85d-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c85d-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8c85d-112">actionState</span><span class="sxs-lookup"><span data-stu-id="8c85d-112">actionState</span></span>|[<span data-ttu-id="8c85d-113">actionState</span><span class="sxs-lookup"><span data-stu-id="8c85d-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="8c85d-114">从 [ deviceActionResult ](../resources/intune_devices_deviceactionresult.md)  继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="8c85d-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="8c85d-115">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="8c85d-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="8c85d-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="8c85d-116">startDateTime</span></span>|<span data-ttu-id="8c85d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c85d-117">DateTimeOffset</span></span>|<span data-ttu-id="8c85d-118">启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c85d-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8c85d-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c85d-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="8c85d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c85d-120">DateTimeOffset</span></span>|<span data-ttu-id="8c85d-121">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="8c85d-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="8c85d-122">scanType</span><span class="sxs-lookup"><span data-stu-id="8c85d-122">scanType</span></span>|<span data-ttu-id="8c85d-123">String</span><span class="sxs-lookup"><span data-stu-id="8c85d-123">String</span></span>|<span data-ttu-id="8c85d-124">扫描类型（完全扫描或快速扫描）</span><span class="sxs-lookup"><span data-stu-id="8c85d-124">Scan type either full scan or quick scan</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c85d-125">关系</span><span class="sxs-lookup"><span data-stu-id="8c85d-125">Relationships</span></span>
<span data-ttu-id="8c85d-126">无</span><span class="sxs-lookup"><span data-stu-id="8c85d-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c85d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c85d-127">JSON Representation</span></span>
<span data-ttu-id="8c85d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c85d-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "scanType": "String"
}
```



