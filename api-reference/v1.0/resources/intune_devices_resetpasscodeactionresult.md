# <a name="resetpasscodeactionresult-resource-type"></a><span data-ttu-id="6989d-101">resetPasscodeActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="6989d-101">resetPasscodeActionResult resource type</span></span>

> <span data-ttu-id="6989d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6989d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6989d-103">重置密码操作结果</span><span class="sxs-lookup"><span data-stu-id="6989d-103">Reset passcode action result</span></span>

<span data-ttu-id="6989d-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6989d-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6989d-105">属性</span><span class="sxs-lookup"><span data-stu-id="6989d-105">Properties</span></span>
|<span data-ttu-id="6989d-106">属性</span><span class="sxs-lookup"><span data-stu-id="6989d-106">Property</span></span>|<span data-ttu-id="6989d-107">类型</span><span class="sxs-lookup"><span data-stu-id="6989d-107">Type</span></span>|<span data-ttu-id="6989d-108">说明</span><span class="sxs-lookup"><span data-stu-id="6989d-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6989d-109">actionName</span><span class="sxs-lookup"><span data-stu-id="6989d-109">actionName</span></span>|<span data-ttu-id="6989d-110">String</span><span class="sxs-lookup"><span data-stu-id="6989d-110">String</span></span>|<span data-ttu-id="6989d-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6989d-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="6989d-112">actionState</span><span class="sxs-lookup"><span data-stu-id="6989d-112">actionState</span></span>|[<span data-ttu-id="6989d-113">actionState</span><span class="sxs-lookup"><span data-stu-id="6989d-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="6989d-114">从[deviceActionResult](../resources/intune_devices_deviceactionresult.md)继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="6989d-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md).</span></span> <span data-ttu-id="6989d-115">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="6989d-115">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="6989d-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6989d-116">startDateTime</span></span>|<span data-ttu-id="6989d-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6989d-117">DateTimeOffset</span></span>|<span data-ttu-id="6989d-118">启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6989d-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="6989d-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="6989d-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="6989d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6989d-120">DateTimeOffset</span></span>|<span data-ttu-id="6989d-121">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="6989d-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="6989d-122">密码</span><span class="sxs-lookup"><span data-stu-id="6989d-122">passcode</span></span>|<span data-ttu-id="6989d-123">String</span><span class="sxs-lookup"><span data-stu-id="6989d-123">String</span></span>|<span data-ttu-id="6989d-124">新生成的设备密码</span><span class="sxs-lookup"><span data-stu-id="6989d-124">Newly generated passcode for the device</span></span> |

## <a name="relationships"></a><span data-ttu-id="6989d-125">关系</span><span class="sxs-lookup"><span data-stu-id="6989d-125">Relationships</span></span>
<span data-ttu-id="6989d-126">无</span><span class="sxs-lookup"><span data-stu-id="6989d-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6989d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6989d-127">JSON Representation</span></span>
<span data-ttu-id="6989d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6989d-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resetPasscodeActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resetPasscodeActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "passcode": "String"
}
```



