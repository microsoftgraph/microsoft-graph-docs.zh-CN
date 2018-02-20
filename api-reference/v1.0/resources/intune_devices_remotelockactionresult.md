# <a name="remotelockactionresult-resource-type"></a><span data-ttu-id="59b0f-101">remoteLockActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="59b0f-101">remoteLockActionResult resource type</span></span>

> <span data-ttu-id="59b0f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="59b0f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59b0f-103">锁定操作结果，包含用于解锁的 PIN</span><span class="sxs-lookup"><span data-stu-id="59b0f-103">Lock action result with a pin to unlock</span></span>

<span data-ttu-id="59b0f-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="59b0f-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="59b0f-105">属性</span><span class="sxs-lookup"><span data-stu-id="59b0f-105">Properties</span></span>
|<span data-ttu-id="59b0f-106">属性</span><span class="sxs-lookup"><span data-stu-id="59b0f-106">Property</span></span>|<span data-ttu-id="59b0f-107">类型</span><span class="sxs-lookup"><span data-stu-id="59b0f-107">Type</span></span>|<span data-ttu-id="59b0f-108">说明</span><span class="sxs-lookup"><span data-stu-id="59b0f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59b0f-109">actionName</span><span class="sxs-lookup"><span data-stu-id="59b0f-109">ActionName</span></span>|<span data-ttu-id="59b0f-110">String</span><span class="sxs-lookup"><span data-stu-id="59b0f-110">String</span></span>|<span data-ttu-id="59b0f-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="59b0f-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="59b0f-112">actionState</span><span class="sxs-lookup"><span data-stu-id="59b0f-112">actionState</span></span>|<span data-ttu-id="59b0f-113">String</span><span class="sxs-lookup"><span data-stu-id="59b0f-113">String</span></span>|<span data-ttu-id="59b0f-114">操作状态 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md) 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="59b0f-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="59b0f-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="59b0f-115">startDateTime</span></span>|<span data-ttu-id="59b0f-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59b0f-116">DateTimeOffset</span></span>|<span data-ttu-id="59b0f-117">启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="59b0f-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="59b0f-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="59b0f-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="59b0f-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="59b0f-119">DateTimeOffset</span></span>|<span data-ttu-id="59b0f-120">上次更新操作状态的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="59b0f-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="59b0f-121">unlockPin</span><span class="sxs-lookup"><span data-stu-id="59b0f-121">unlockPin</span></span>|<span data-ttu-id="59b0f-122">String</span><span class="sxs-lookup"><span data-stu-id="59b0f-122">String</span></span>|<span data-ttu-id="59b0f-123">用于解锁客户端的 PIN</span><span class="sxs-lookup"><span data-stu-id="59b0f-123">Pin to unlock the client</span></span>|

## <a name="relationships"></a><span data-ttu-id="59b0f-124">关系</span><span class="sxs-lookup"><span data-stu-id="59b0f-124">Relationships</span></span>
<span data-ttu-id="59b0f-125">无</span><span class="sxs-lookup"><span data-stu-id="59b0f-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59b0f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59b0f-126">JSON Representation</span></span>
<span data-ttu-id="59b0f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59b0f-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteLockActionResult"
}
-->
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



