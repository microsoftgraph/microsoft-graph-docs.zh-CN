# <a name="roledefinition-resource-type"></a><span data-ttu-id="363b1-101">roleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="363b1-101">roleDefinition resource type</span></span>

> <span data-ttu-id="363b1-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="363b1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="363b1-103">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="363b1-103">The Role Definition resource.</span></span> <span data-ttu-id="363b1-104">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="363b1-104">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="363b1-105">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="363b1-105">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="363b1-106">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="363b1-106">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="363b1-107">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="363b1-107">Built-in roles cannot be modified.</span></span> <span data-ttu-id="363b1-108">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="363b1-108">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="363b1-109">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="363b1-109">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="363b1-110">方法</span><span class="sxs-lookup"><span data-stu-id="363b1-110">Methods</span></span>
|<span data-ttu-id="363b1-111">方法</span><span class="sxs-lookup"><span data-stu-id="363b1-111">Method</span></span>|<span data-ttu-id="363b1-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="363b1-112">Return Type</span></span>|<span data-ttu-id="363b1-113">说明</span><span class="sxs-lookup"><span data-stu-id="363b1-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="363b1-114">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="363b1-114">List roleDefinitions</span></span>](../api/intune_rbac_roledefinition_list.md)|<span data-ttu-id="363b1-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="363b1-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="363b1-116">列出 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="363b1-116">List properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="363b1-117">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="363b1-117">Get roleDefinition</span></span>](../api/intune_rbac_roledefinition_get.md)|[<span data-ttu-id="363b1-118">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="363b1-118">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="363b1-119">读取 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="363b1-119">Read properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="363b1-120">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="363b1-120">Create roleDefinition</span></span>](../api/intune_rbac_roledefinition_create.md)|[<span data-ttu-id="363b1-121">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="363b1-121">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="363b1-122">创建新的 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="363b1-122">Create a new [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="363b1-123">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="363b1-123">Delete roleDefinition</span></span>](../api/intune_rbac_roledefinition_delete.md)|<span data-ttu-id="363b1-124">无</span><span class="sxs-lookup"><span data-stu-id="363b1-124">None</span></span>|<span data-ttu-id="363b1-125">删除 [roleDefinition](../resources/intune_rbac_roledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="363b1-125">Deletes a [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>|
|[<span data-ttu-id="363b1-126">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="363b1-126">Update roleDefinition</span></span>](../api/intune_rbac_roledefinition_update.md)|[<span data-ttu-id="363b1-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="363b1-127">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="363b1-128">更新 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="363b1-128">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="363b1-129">属性</span><span class="sxs-lookup"><span data-stu-id="363b1-129">Properties</span></span>
|<span data-ttu-id="363b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="363b1-130">Property</span></span>|<span data-ttu-id="363b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="363b1-131">Type</span></span>|<span data-ttu-id="363b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="363b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="363b1-133">id</span><span class="sxs-lookup"><span data-stu-id="363b1-133">id</span></span>|<span data-ttu-id="363b1-134">String</span><span class="sxs-lookup"><span data-stu-id="363b1-134">String</span></span>|<span data-ttu-id="363b1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="363b1-135">Key of the entity.</span></span> <span data-ttu-id="363b1-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="363b1-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="363b1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="363b1-137">displayName</span></span>|<span data-ttu-id="363b1-138">String</span><span class="sxs-lookup"><span data-stu-id="363b1-138">String</span></span>|<span data-ttu-id="363b1-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="363b1-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="363b1-140">说明</span><span class="sxs-lookup"><span data-stu-id="363b1-140">description</span></span>|<span data-ttu-id="363b1-141">String</span><span class="sxs-lookup"><span data-stu-id="363b1-141">String</span></span>|<span data-ttu-id="363b1-142">角色定义的描述。</span><span class="sxs-lookup"><span data-stu-id="363b1-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="363b1-143">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="363b1-143">rolePermissions</span></span>|<span data-ttu-id="363b1-144">[rolePermission](../resources/intune_rbac_rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="363b1-144">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="363b1-145">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="363b1-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="363b1-146">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="363b1-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="363b1-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="363b1-147">isBuiltIn</span></span>|<span data-ttu-id="363b1-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="363b1-148">Boolean</span></span>|<span data-ttu-id="363b1-149">角色类型。</span><span class="sxs-lookup"><span data-stu-id="363b1-149">Type of Role.</span></span> <span data-ttu-id="363b1-150">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="363b1-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="363b1-151">关系</span><span class="sxs-lookup"><span data-stu-id="363b1-151">Relationships</span></span>
|<span data-ttu-id="363b1-152">关系</span><span class="sxs-lookup"><span data-stu-id="363b1-152">Relationship</span></span>|<span data-ttu-id="363b1-153">类型</span><span class="sxs-lookup"><span data-stu-id="363b1-153">Type</span></span>|<span data-ttu-id="363b1-154">说明</span><span class="sxs-lookup"><span data-stu-id="363b1-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="363b1-155">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="363b1-155">roleAssignments</span></span>|<span data-ttu-id="363b1-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="363b1-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="363b1-157">此角色定义的角色分配列表</span><span class="sxs-lookup"><span data-stu-id="363b1-157">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="363b1-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="363b1-158">JSON Representation</span></span>
<span data-ttu-id="363b1-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="363b1-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



