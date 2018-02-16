# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="9e3a9-101">deleteUserFromSharedAppleDeviceActionResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e3a9-101">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="9e3a9-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9e3a9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e3a9-103">从共享 Apple 设备删除用户操作结果</span><span class="sxs-lookup"><span data-stu-id="9e3a9-103">Delete user from shared apple device action result</span></span>

<span data-ttu-id="9e3a9-104">继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9e3a9-104">Inherits from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9e3a9-105">属性</span><span class="sxs-lookup"><span data-stu-id="9e3a9-105">Properties</span></span>
|<span data-ttu-id="9e3a9-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e3a9-106">Property</span></span>|<span data-ttu-id="9e3a9-107">类型</span><span class="sxs-lookup"><span data-stu-id="9e3a9-107">Type</span></span>|<span data-ttu-id="9e3a9-108">说明</span><span class="sxs-lookup"><span data-stu-id="9e3a9-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e3a9-109">actionName</span><span class="sxs-lookup"><span data-stu-id="9e3a9-109">ActionName</span></span>|<span data-ttu-id="9e3a9-110">String</span><span class="sxs-lookup"><span data-stu-id="9e3a9-110">String</span></span>|<span data-ttu-id="9e3a9-111">操作名称 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9e3a9-111">Action name Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9e3a9-112">actionState</span><span class="sxs-lookup"><span data-stu-id="9e3a9-112">actionState</span></span>|<span data-ttu-id="9e3a9-113">String</span><span class="sxs-lookup"><span data-stu-id="9e3a9-113">String</span></span>|<span data-ttu-id="9e3a9-114">操作状态 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md) 可取值为：`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported`。</span><span class="sxs-lookup"><span data-stu-id="9e3a9-114">State of the action Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md) Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9e3a9-115">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9e3a9-115">startDateTime</span></span>|<span data-ttu-id="9e3a9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e3a9-116">DateTimeOffset</span></span>|<span data-ttu-id="9e3a9-117">操作启动的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9e3a9-117">Time the action was initiated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9e3a9-118">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e3a9-118">lastUpdatedDateTime</span></span>|<span data-ttu-id="9e3a9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e3a9-119">DateTimeOffset</span></span>|<span data-ttu-id="9e3a9-120">操作状态上次更新的时间 继承自 [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9e3a9-120">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune_devices_deviceactionresult.md)</span></span>|
|<span data-ttu-id="9e3a9-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9e3a9-121">userPrincipalName</span></span>|<span data-ttu-id="9e3a9-122">String</span><span class="sxs-lookup"><span data-stu-id="9e3a9-122">String</span></span>|<span data-ttu-id="9e3a9-123">要删除的用户的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="9e3a9-123">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e3a9-124">关系</span><span class="sxs-lookup"><span data-stu-id="9e3a9-124">Relationships</span></span>
<span data-ttu-id="9e3a9-125">无</span><span class="sxs-lookup"><span data-stu-id="9e3a9-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9e3a9-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e3a9-126">JSON Representation</span></span>
<span data-ttu-id="9e3a9-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e3a9-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



