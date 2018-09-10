# <a name="roledefinition-resource-type"></a><span data-ttu-id="86943-101">roleDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="86943-101">roleDefinition resource type</span></span>

> <span data-ttu-id="86943-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="86943-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86943-103">角色定义资源。</span><span class="sxs-lookup"><span data-stu-id="86943-103">The Role Definition resource.</span></span> <span data-ttu-id="86943-104">角色定义是在 Intune 中基于角色访问的基础。</span><span class="sxs-lookup"><span data-stu-id="86943-104">The role definition is the foundation of role based access in Intune.</span></span> <span data-ttu-id="86943-105">角色组合了 Intune 资源（例如，移动应用）和关联的角色权限（例如，资源的创建和读取）。</span><span class="sxs-lookup"><span data-stu-id="86943-105">The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource.</span></span> <span data-ttu-id="86943-106">有内置和自定义两种角色类型。</span><span class="sxs-lookup"><span data-stu-id="86943-106">There are two types of roles, built-in and custom.</span></span> <span data-ttu-id="86943-107">内置角色无法修改。</span><span class="sxs-lookup"><span data-stu-id="86943-107">Built-in roles cannot be modified.</span></span> <span data-ttu-id="86943-108">内置角色和自定义角色必须具有强制执行的分配。</span><span class="sxs-lookup"><span data-stu-id="86943-108">Both built-in roles and custom roles must have assignments to be enforced.</span></span> <span data-ttu-id="86943-109">如果要定义一个允许将任意可用资源和角色权限合并到单个角色中的角色，请创建自定义角色。</span><span class="sxs-lookup"><span data-stu-id="86943-109">Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.</span></span>
## <a name="methods"></a><span data-ttu-id="86943-110">方法</span><span class="sxs-lookup"><span data-stu-id="86943-110">Methods</span></span>
|<span data-ttu-id="86943-111">方法</span><span class="sxs-lookup"><span data-stu-id="86943-111">Method</span></span>|<span data-ttu-id="86943-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="86943-112">Return Type</span></span>|<span data-ttu-id="86943-113">说明</span><span class="sxs-lookup"><span data-stu-id="86943-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86943-114">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="86943-114">List roleDefinitions</span></span>](../api/intune_rbac_roledefinition_list.md)|<span data-ttu-id="86943-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86943-115">[roleDefinition](../resources/intune_rbac_roledefinition.md) collection</span></span>|<span data-ttu-id="86943-116">列出 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86943-116">List properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) objects.</span></span>|
|[<span data-ttu-id="86943-117">Get roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86943-117">Get roleDefinition</span></span>](../api/intune_rbac_roledefinition_get.md)|[<span data-ttu-id="86943-118">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86943-118">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="86943-119">读取 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86943-119">Read properties and relationships of the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="86943-120">Create roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86943-120">Create roleDefinition</span></span>](../api/intune_rbac_roledefinition_create.md)|[<span data-ttu-id="86943-121">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86943-121">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="86943-122">创建新的 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="86943-122">Create a new [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|
|[<span data-ttu-id="86943-123">Delete roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86943-123">Delete roleDefinition</span></span>](../api/intune_rbac_roledefinition_delete.md)|<span data-ttu-id="86943-124">无</span><span class="sxs-lookup"><span data-stu-id="86943-124">None</span></span>|<span data-ttu-id="86943-125">删除 [roleDefinition](../resources/intune_rbac_roledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="86943-125">Deletes a [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>|
|[<span data-ttu-id="86943-126">Update roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86943-126">Update roleDefinition</span></span>](../api/intune_rbac_roledefinition_update.md)|[<span data-ttu-id="86943-127">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="86943-127">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="86943-128">更新 [roleDefinition](../resources/intune_rbac_roledefinition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="86943-128">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="86943-129">属性</span><span class="sxs-lookup"><span data-stu-id="86943-129">Properties</span></span>
|<span data-ttu-id="86943-130">属性</span><span class="sxs-lookup"><span data-stu-id="86943-130">Property</span></span>|<span data-ttu-id="86943-131">类型</span><span class="sxs-lookup"><span data-stu-id="86943-131">Type</span></span>|<span data-ttu-id="86943-132">说明</span><span class="sxs-lookup"><span data-stu-id="86943-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86943-133">ID</span><span class="sxs-lookup"><span data-stu-id="86943-133">id</span></span>|<span data-ttu-id="86943-134">字符串</span><span class="sxs-lookup"><span data-stu-id="86943-134">String</span></span>|<span data-ttu-id="86943-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="86943-135">Key of the entity.</span></span> <span data-ttu-id="86943-136">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="86943-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="86943-137">displayName</span><span class="sxs-lookup"><span data-stu-id="86943-137">displayName</span></span>|<span data-ttu-id="86943-138">字符串</span><span class="sxs-lookup"><span data-stu-id="86943-138">String</span></span>|<span data-ttu-id="86943-139">角色定义的显示名称。</span><span class="sxs-lookup"><span data-stu-id="86943-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="86943-140">说明</span><span class="sxs-lookup"><span data-stu-id="86943-140">description</span></span>|<span data-ttu-id="86943-141">字符串</span><span class="sxs-lookup"><span data-stu-id="86943-141">String</span></span>|<span data-ttu-id="86943-142">角色定义的说明。</span><span class="sxs-lookup"><span data-stu-id="86943-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="86943-143">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="86943-143">rolePermissions</span></span>|<span data-ttu-id="86943-144">[rolePermission](../resources/intune_rbac_rolepermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86943-144">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="86943-145">允许此角色执行的角色权限列表。</span><span class="sxs-lookup"><span data-stu-id="86943-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="86943-146">它们必须与定义为 rolePermission 一部分的 actionName 匹配。</span><span class="sxs-lookup"><span data-stu-id="86943-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="86943-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="86943-147">isBuiltIn</span></span>|<span data-ttu-id="86943-148">布尔</span><span class="sxs-lookup"><span data-stu-id="86943-148">Boolean</span></span>|<span data-ttu-id="86943-149">角色类型。</span><span class="sxs-lookup"><span data-stu-id="86943-149">Type of Role.</span></span> <span data-ttu-id="86943-150">如果是内置角色，则设置为 True；如果是自定义角色定义，则设置为 False。</span><span class="sxs-lookup"><span data-stu-id="86943-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86943-151">关系</span><span class="sxs-lookup"><span data-stu-id="86943-151">Relationships</span></span>
|<span data-ttu-id="86943-152">关系</span><span class="sxs-lookup"><span data-stu-id="86943-152">Relationship</span></span>|<span data-ttu-id="86943-153">类型</span><span class="sxs-lookup"><span data-stu-id="86943-153">Type</span></span>|<span data-ttu-id="86943-154">说明</span><span class="sxs-lookup"><span data-stu-id="86943-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86943-155">roleAssignments</span><span class="sxs-lookup"><span data-stu-id="86943-155">roleAssignments</span></span>|<span data-ttu-id="86943-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="86943-156">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="86943-157">此角色定义的角色分配列表</span><span class="sxs-lookup"><span data-stu-id="86943-157">List of Role assignments for this role definition.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86943-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86943-158">JSON Representation</span></span>
<span data-ttu-id="86943-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86943-159">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition"
}-->
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








