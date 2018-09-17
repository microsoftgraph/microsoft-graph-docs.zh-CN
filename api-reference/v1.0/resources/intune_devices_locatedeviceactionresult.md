# <a name="locatedeviceactionresult-resource-type"></a><span data-ttu-id="9821f-101">locateDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="9821f-101">locateDeviceActionResult resource type</span></span>

> <span data-ttu-id="9821f-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9821f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9821f-103">查找设备操作结果</span><span class="sxs-lookup"><span data-stu-id="9821f-103">Locate device action result</span></span>

<span data-ttu-id="9821f-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9821f-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9821f-105">属性</span><span class="sxs-lookup"><span data-stu-id="9821f-105">Properties</span></span>
|<span data-ttu-id="9821f-106">属性</span><span class="sxs-lookup"><span data-stu-id="9821f-106">Property</span></span>|<span data-ttu-id="9821f-107">类型</span><span class="sxs-lookup"><span data-stu-id="9821f-107">Type</span></span>|<span data-ttu-id="9821f-108">说明</span><span class="sxs-lookup"><span data-stu-id="9821f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9821f-109">actionName</span><span class="sxs-lookup"><span data-stu-id="9821f-109">actionName</span></span>|<span data-ttu-id="9821f-110">字符串</span><span class="sxs-lookup"><span data-stu-id="9821f-110">String</span></span>|<span data-ttu-id="9821f-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9821f-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9821f-112">actionState</span><span class="sxs-lookup"><span data-stu-id="9821f-112">actionState</span></span>|[<span data-ttu-id="9821f-113">actionState</span><span class="sxs-lookup"><span data-stu-id="9821f-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="9821f-p101">从 [deviceActionResult](../resources/intune_devices_deviceactionresult.md) 继承操作的状态。可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="9821f-p101">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9821f-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9821f-116">startDateTime</span></span>|<span data-ttu-id="9821f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9821f-117">DateTimeOffset</span></span>|<span data-ttu-id="9821f-118">启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9821f-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9821f-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9821f-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="9821f-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9821f-120">DateTimeOffset</span></span>|<span data-ttu-id="9821f-121">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9821f-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9821f-122">deviceLocation</span><span class="sxs-lookup"><span data-stu-id="9821f-122">deviceLocation</span></span>|[<span data-ttu-id="9821f-123">deviceGeoLocation</span><span class="sxs-lookup"><span data-stu-id="9821f-123">deviceGeoLocation</span></span>](../resources/intune_devices_devicegeolocation.md)|<span data-ttu-id="9821f-124">设备位置</span><span class="sxs-lookup"><span data-stu-id="9821f-124">device location</span></span>|

## <a name="relationships"></a><span data-ttu-id="9821f-125">关系</span><span class="sxs-lookup"><span data-stu-id="9821f-125">Relationships</span></span>
<span data-ttu-id="9821f-126">无</span><span class="sxs-lookup"><span data-stu-id="9821f-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9821f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9821f-127">JSON Representation</span></span>
<span data-ttu-id="9821f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9821f-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "deviceLocation": {
    "@odata.type": "microsoft.graph.deviceGeoLocation",
    "lastCollectedDateTime": "String (timestamp)",
    "longitude": "<Unknown Primitive Type Edm.Double>",
    "latitude": "<Unknown Primitive Type Edm.Double>",
    "altitude": "<Unknown Primitive Type Edm.Double>",
    "horizontalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "verticalAccuracy": "<Unknown Primitive Type Edm.Double>",
    "heading": "<Unknown Primitive Type Edm.Double>",
    "speed": "<Unknown Primitive Type Edm.Double>"
  }
}
```








