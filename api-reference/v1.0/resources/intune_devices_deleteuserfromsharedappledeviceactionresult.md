# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="2480e-101">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="2480e-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="2480e-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2480e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2480e-103">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="2480e-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="2480e-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2480e-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2480e-105">属性</span><span class="sxs-lookup"><span data-stu-id="2480e-105">Properties</span></span>
|<span data-ttu-id="2480e-106">属性</span><span class="sxs-lookup"><span data-stu-id="2480e-106">Property</span></span>|<span data-ttu-id="2480e-107">类型</span><span class="sxs-lookup"><span data-stu-id="2480e-107">Type</span></span>|<span data-ttu-id="2480e-108">说明</span><span class="sxs-lookup"><span data-stu-id="2480e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2480e-109">actionName</span><span class="sxs-lookup"><span data-stu-id="2480e-109">actionName</span></span>|<span data-ttu-id="2480e-110">String</span><span class="sxs-lookup"><span data-stu-id="2480e-110">String</span></span>|<span data-ttu-id="2480e-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2480e-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="2480e-112">actionState</span><span class="sxs-lookup"><span data-stu-id="2480e-112">actionState</span></span>|[<span data-ttu-id="2480e-113">actionState</span><span class="sxs-lookup"><span data-stu-id="2480e-113">actionState</span></span>](../resources/intune_devices_actionstate.md)|<span data-ttu-id="2480e-114">从 [deviceActionResult](../resources/intune_devices_deviceactionresult.md) 继承操作的状态。</span><span class="sxs-lookup"><span data-stu-id="2480e-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: , , , , , , .</span></span> <span data-ttu-id="2480e-115">可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="2480e-115">The possible values are `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`, , , , , or .</span></span>|
|<span data-ttu-id="2480e-116">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2480e-116">startDateTime</span></span>|<span data-ttu-id="2480e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2480e-117">DateTimeOffset</span></span>|<span data-ttu-id="2480e-118">启动操作的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2480e-118">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="2480e-119">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2480e-119">lastUpdatedDateTime</span></span>|<span data-ttu-id="2480e-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2480e-120">DateTimeOffset</span></span>|<span data-ttu-id="2480e-121">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="2480e-121">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="2480e-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2480e-122">userPrincipalName</span></span>|<span data-ttu-id="2480e-123">String</span><span class="sxs-lookup"><span data-stu-id="2480e-123">String</span></span>|<span data-ttu-id="2480e-124">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="2480e-124">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="2480e-125">关系</span><span class="sxs-lookup"><span data-stu-id="2480e-125">Relationships</span></span>
<span data-ttu-id="2480e-126">无</span><span class="sxs-lookup"><span data-stu-id="2480e-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2480e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2480e-127">JSON Representation</span></span>
<span data-ttu-id="2480e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2480e-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceActionResult",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



