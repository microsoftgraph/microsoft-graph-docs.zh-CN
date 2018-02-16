# <a name="devicemanagement-resource-type"></a><span data-ttu-id="69df6-101">deviceManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="69df6-101">deviceManagement resource type</span></span>

> <span data-ttu-id="69df6-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="69df6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69df6-103">充当所有设备管理功能的容器的单例实体。</span><span class="sxs-lookup"><span data-stu-id="69df6-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="69df6-104">方法</span><span class="sxs-lookup"><span data-stu-id="69df6-104">Methods</span></span>
|<span data-ttu-id="69df6-105">方法</span><span class="sxs-lookup"><span data-stu-id="69df6-105">Method</span></span>|<span data-ttu-id="69df6-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="69df6-106">Return Type</span></span>|<span data-ttu-id="69df6-107">说明</span><span class="sxs-lookup"><span data-stu-id="69df6-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69df6-108">获取 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="69df6-108">Get deviceManagement</span></span>](../api/intune_rbac_devicemanagement_get.md)|[<span data-ttu-id="69df6-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="69df6-109">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="69df6-110">读取 [deviceManagement](../resources/intune_rbac_devicemanagement.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69df6-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="69df6-111">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="69df6-111">Update deviceManagement</span></span>](../api/intune_rbac_devicemanagement_update.md)|[<span data-ttu-id="69df6-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="69df6-112">deviceManagement</span></span>](../resources/intune_rbac_devicemanagement.md)|<span data-ttu-id="69df6-113">更新 [deviceManagement](../resources/intune_rbac_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="69df6-113">Update the properties of a [calendar](../resources/intune_rbac_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="69df6-114">getEffectivePermissions 函数</span><span class="sxs-lookup"><span data-stu-id="69df6-114">getEffectivePermissions function</span></span>](../api/intune_rbac_devicemanagement_geteffectivepermissions.md)|<span data-ttu-id="69df6-115">[rolePermission](../resources/intune_rbac_rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69df6-115">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="69df6-116">检索当前验证的用户的有效权限</span><span class="sxs-lookup"><span data-stu-id="69df6-116">Retrieves the effective permissions of the currently authenticated user</span></span>|

## <a name="properties"></a><span data-ttu-id="69df6-117">属性</span><span class="sxs-lookup"><span data-stu-id="69df6-117">Properties</span></span>
|<span data-ttu-id="69df6-118">属性</span><span class="sxs-lookup"><span data-stu-id="69df6-118">Property</span></span>|<span data-ttu-id="69df6-119">类型</span><span class="sxs-lookup"><span data-stu-id="69df6-119">Type</span></span>|<span data-ttu-id="69df6-120">说明</span><span class="sxs-lookup"><span data-stu-id="69df6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69df6-121">id</span><span class="sxs-lookup"><span data-stu-id="69df6-121">id</span></span>|<span data-ttu-id="69df6-122">String</span><span class="sxs-lookup"><span data-stu-id="69df6-122">String</span></span>|<span data-ttu-id="69df6-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="69df6-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="69df6-124">关系</span><span class="sxs-lookup"><span data-stu-id="69df6-124">Relationships</span></span>
|<span data-ttu-id="69df6-125">关系</span><span class="sxs-lookup"><span data-stu-id="69df6-125">Relationship</span></span>|<span data-ttu-id="69df6-126">类型</span><span class="sxs-lookup"><span data-stu-id="69df6-126">Type</span></span>|<span data-ttu-id="69df6-127">说明</span><span class="sxs-lookup"><span data-stu-id="69df6-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69df6-128">roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="69df6-128">roleDefinitions</span></span>|<span data-ttu-id="69df6-129">[roleDefinition](../resources/intune_rbac_roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69df6-129">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="69df6-130">角色定义。</span><span class="sxs-lookup"><span data-stu-id="69df6-130">The Role Definitions.</span></span>|
|<span data-ttu-id="69df6-131">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="69df6-131">roleAssignments</span></span>|<span data-ttu-id="69df6-132">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69df6-132">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) collection</span></span>|<span data-ttu-id="69df6-133">角色分配。</span><span class="sxs-lookup"><span data-stu-id="69df6-133">The Role Assignments.</span></span>|
|<span data-ttu-id="69df6-134">resourceOperations</span><span class="sxs-lookup"><span data-stu-id="69df6-134">resourceOperations</span></span>|<span data-ttu-id="69df6-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="69df6-135">[resourceOperation](../resources/intune_rbac_resourceoperation.md) collection</span></span>|<span data-ttu-id="69df6-136">资源操作。</span><span class="sxs-lookup"><span data-stu-id="69df6-136">The Resource Operations.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69df6-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69df6-137">JSON Representation</span></span>
<span data-ttu-id="69df6-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69df6-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



