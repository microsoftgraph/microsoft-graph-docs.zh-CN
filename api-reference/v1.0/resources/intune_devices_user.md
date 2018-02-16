# <a name="user-resource-type"></a><span data-ttu-id="35379-101">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="35379-101">user resource type</span></span>

> <span data-ttu-id="35379-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="35379-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35379-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="35379-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="35379-104">方法</span><span class="sxs-lookup"><span data-stu-id="35379-104">Methods</span></span>
|<span data-ttu-id="35379-105">方法</span><span class="sxs-lookup"><span data-stu-id="35379-105">Method</span></span>|<span data-ttu-id="35379-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="35379-106">Return Type</span></span>|<span data-ttu-id="35379-107">说明</span><span class="sxs-lookup"><span data-stu-id="35379-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35379-108">List users</span><span class="sxs-lookup"><span data-stu-id="35379-108">List users</span></span>](../api/intune_devices_user_list.md)|<span data-ttu-id="35379-109">[user](../resources/intune_devices_user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35379-109">[user](../resources/intune_devices_user.md) collection</span></span>|<span data-ttu-id="35379-110">列出 [user](../resources/intune_devices_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35379-110">List properties and relationships of the [user](../resources/intune_devices_user.md) objects.</span></span>|
|[<span data-ttu-id="35379-111">获取 user</span><span class="sxs-lookup"><span data-stu-id="35379-111">Get user</span></span>](../api/intune_devices_user_get.md)|[<span data-ttu-id="35379-112">user</span><span class="sxs-lookup"><span data-stu-id="35379-112">user</span></span>](../resources/intune_devices_user.md)|<span data-ttu-id="35379-113">读取 [user](../resources/intune_devices_user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="35379-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_user.md) object.</span></span>|
|[<span data-ttu-id="35379-114">创建 user</span><span class="sxs-lookup"><span data-stu-id="35379-114">Create user</span></span>](../api/intune_devices_user_create.md)|[<span data-ttu-id="35379-115">user</span><span class="sxs-lookup"><span data-stu-id="35379-115">user</span></span>](../resources/intune_devices_user.md)|<span data-ttu-id="35379-116">创建新的 [user](../resources/intune_devices_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="35379-116">Create a new user object.</span></span>|
|[<span data-ttu-id="35379-117">删除 user</span><span class="sxs-lookup"><span data-stu-id="35379-117">Delete user</span></span>](../api/intune_devices_user_delete.md)|<span data-ttu-id="35379-118">无</span><span class="sxs-lookup"><span data-stu-id="35379-118">None</span></span>|<span data-ttu-id="35379-119">删除 [user](../resources/intune_devices_user.md)。</span><span class="sxs-lookup"><span data-stu-id="35379-119">Deletes a [user](../resources/intune_devices_user.md).</span></span>|
|[<span data-ttu-id="35379-120">更新 user</span><span class="sxs-lookup"><span data-stu-id="35379-120">Update user</span></span>](../api/intune_devices_user_update.md)|[<span data-ttu-id="35379-121">user</span><span class="sxs-lookup"><span data-stu-id="35379-121">user</span></span>](../resources/intune_devices_user.md)|<span data-ttu-id="35379-122">更新 [user](../resources/intune_devices_user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35379-122">Update the properties of a user object.</span></span>|
|[<span data-ttu-id="35379-123">removeAllDevicesFromManagement 操作</span><span class="sxs-lookup"><span data-stu-id="35379-123">removeAllDevicesFromManagement action</span></span>](../api/intune_devices_user_removealldevicesfrommanagement.md)|<span data-ttu-id="35379-124">无</span><span class="sxs-lookup"><span data-stu-id="35379-124">None</span></span>|<span data-ttu-id="35379-125">停用该用户管理的所有设备</span><span class="sxs-lookup"><span data-stu-id="35379-125">Retire all devices from management for this user</span></span>|

## <a name="properties"></a><span data-ttu-id="35379-126">属性</span><span class="sxs-lookup"><span data-stu-id="35379-126">Properties</span></span>
|<span data-ttu-id="35379-127">属性</span><span class="sxs-lookup"><span data-stu-id="35379-127">Property</span></span>|<span data-ttu-id="35379-128">类型</span><span class="sxs-lookup"><span data-stu-id="35379-128">Type</span></span>|<span data-ttu-id="35379-129">说明</span><span class="sxs-lookup"><span data-stu-id="35379-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35379-130">id</span><span class="sxs-lookup"><span data-stu-id="35379-130">id</span></span>|<span data-ttu-id="35379-131">String</span><span class="sxs-lookup"><span data-stu-id="35379-131">String</span></span>|<span data-ttu-id="35379-132">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="35379-132">Unique identifier of the folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35379-133">关系</span><span class="sxs-lookup"><span data-stu-id="35379-133">Relationships</span></span>
|<span data-ttu-id="35379-134">关系</span><span class="sxs-lookup"><span data-stu-id="35379-134">Relationship</span></span>|<span data-ttu-id="35379-135">类型</span><span class="sxs-lookup"><span data-stu-id="35379-135">Type</span></span>|<span data-ttu-id="35379-136">说明</span><span class="sxs-lookup"><span data-stu-id="35379-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35379-137">managedDevices</span><span class="sxs-lookup"><span data-stu-id="35379-137">managedDevices</span></span>|<span data-ttu-id="35379-138">[managedDevice](../resources/intune_devices_manageddevice.md) 集合</span><span class="sxs-lookup"><span data-stu-id="35379-138">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="35379-139">与用户关联的管理设备。</span><span class="sxs-lookup"><span data-stu-id="35379-139">The managed devices associated with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35379-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35379-140">JSON Representation</span></span>
<span data-ttu-id="35379-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35379-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



