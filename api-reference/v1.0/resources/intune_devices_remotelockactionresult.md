# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="3eb13-101">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="3eb13-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="3eb13-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3eb13-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3eb13-103">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="3eb13-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="3eb13-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3eb13-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3eb13-105">属性</span><span class="sxs-lookup"><span data-stu-id="3eb13-105">Properties</span></span>
|<span data-ttu-id="3eb13-106">属性</span><span class="sxs-lookup"><span data-stu-id="3eb13-106">Property</span></span>|<span data-ttu-id="3eb13-107">类型</span><span class="sxs-lookup"><span data-stu-id="3eb13-107">Type</span></span>|<span data-ttu-id="3eb13-108">说明</span><span class="sxs-lookup"><span data-stu-id="3eb13-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eb13-109">actionName</span><span class="sxs-lookup"><span data-stu-id="3eb13-109">actionName</span></span>|<span data-ttu-id="3eb13-110">String</span><span class="sxs-lookup"><span data-stu-id="3eb13-110">String</span></span>|<span data-ttu-id="3eb13-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3eb13-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="3eb13-112">actionState</span><span class="sxs-lookup"><span data-stu-id="3eb13-112">actionState</span></span>|[<span data-ttu-id="3eb13-113">actionState</span><span class="sxs-lookup"><span data-stu-id="3eb13-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="3eb13-114">从 [deviceActionResult](../resources/intune_devices_deviceactionresult.md) 继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="3eb13-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="3eb13-115">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="3eb13-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="3eb13-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3eb13-116">startDateTime</span></span>|<span data-ttu-id="3eb13-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb13-117">DateTimeOffset</span></span>|<span data-ttu-id="3eb13-118">启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3eb13-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="3eb13-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="3eb13-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="3eb13-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3eb13-120">DateTimeOffset</span></span>|<span data-ttu-id="3eb13-121">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="3eb13-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="3eb13-122">unlockPin</span><span class="sxs-lookup"><span data-stu-id="3eb13-122">unlockPin</span></span>|<span data-ttu-id="3eb13-123">String</span><span class="sxs-lookup"><span data-stu-id="3eb13-123">String</span></span>|<span data-ttu-id="3eb13-124">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="3eb13-124">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="3eb13-125">关系</span><span class="sxs-lookup"><span data-stu-id="3eb13-125">Relationships</span></span>
<span data-ttu-id="3eb13-126">无</span><span class="sxs-lookup"><span data-stu-id="3eb13-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3eb13-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3eb13-127">JSON Representation</span></span>
<span data-ttu-id="3eb13-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3eb13-128">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteLockActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "unlockPin": "String"
}
```



