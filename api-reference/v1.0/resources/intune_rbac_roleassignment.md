# <a name="roleassignment-resource-type"></a><span data-ttu-id="718aa-101">roleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="718aa-101">roleAssignment resource type</span></span>

> <span data-ttu-id="718aa-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="718aa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="718aa-103">角色分配资源。</span><span class="sxs-lookup"><span data-stu-id="718aa-103">The Role Assignment resource.</span></span> <span data-ttu-id="718aa-104">角色分配将角色定义与成员和作用域绑定在一起。</span><span class="sxs-lookup"><span data-stu-id="718aa-104">Role assignments tie together a role definition with members and scopes.</span></span> <span data-ttu-id="718aa-105">每个角色可以具有一个或多个角色分配。</span><span class="sxs-lookup"><span data-stu-id="718aa-105">There can be one or more role assignments per role.</span></span> <span data-ttu-id="718aa-106">这适用于自定义和内置角色。</span><span class="sxs-lookup"><span data-stu-id="718aa-106">This applies to custom and built-in roles.</span></span>
## <a name="methods"></a><span data-ttu-id="718aa-107">方法</span><span class="sxs-lookup"><span data-stu-id="718aa-107">Methods</span></span>
|<span data-ttu-id="718aa-108">方法</span><span class="sxs-lookup"><span data-stu-id="718aa-108">Method</span></span>|<span data-ttu-id="718aa-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="718aa-109">Return Type</span></span>|<span data-ttu-id="718aa-110">说明</span><span class="sxs-lookup"><span data-stu-id="718aa-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="718aa-111">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="718aa-111">List roleAssignments</span></span>](../api/intune_rbac_roleassignment_list.md)|<span data-ttu-id="718aa-112">[roleAssignment](../resources/intune_rbac_roleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="718aa-112">[roleAssignment](../resources/intune_rbac_roleassignment.md) collection</span></span>|<span data-ttu-id="718aa-113">列出 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="718aa-113">List properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) objects.</span></span>|
|[<span data-ttu-id="718aa-114">Get roleAssignment</span><span class="sxs-lookup"><span data-stu-id="718aa-114">Get roleAssignment</span></span>](../api/intune_rbac_roleassignment_get.md)|[<span data-ttu-id="718aa-115">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="718aa-115">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="718aa-116">读取 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="718aa-116">Read properties and relationships of the [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="718aa-117">Create roleAssignment</span><span class="sxs-lookup"><span data-stu-id="718aa-117">Create roleAssignment</span></span>](../api/intune_rbac_roleassignment_create.md)|[<span data-ttu-id="718aa-118">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="718aa-118">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="718aa-119">创建新的 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="718aa-119">Create a new [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|
|[<span data-ttu-id="718aa-120">Delete roleAssignment</span><span class="sxs-lookup"><span data-stu-id="718aa-120">Delete roleAssignment</span></span>](../api/intune_rbac_roleassignment_delete.md)|<span data-ttu-id="718aa-121">无</span><span class="sxs-lookup"><span data-stu-id="718aa-121">None</span></span>|<span data-ttu-id="718aa-122">删除 [roleAssignment](../resources/intune_rbac_roleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="718aa-122">Deletes a [roleAssignment](../resources/intune_rbac_roleassignment.md).</span></span>|
|[<span data-ttu-id="718aa-123">Update roleAssignment</span><span class="sxs-lookup"><span data-stu-id="718aa-123">Update roleAssignment</span></span>](../api/intune_rbac_roleassignment_update.md)|[<span data-ttu-id="718aa-124">roleAssignment</span><span class="sxs-lookup"><span data-stu-id="718aa-124">roleAssignment</span></span>](../resources/intune_rbac_roleassignment.md)|<span data-ttu-id="718aa-125">更新 [roleAssignment](../resources/intune_rbac_roleassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="718aa-125">Update the properties of a [roleAssignment](../resources/intune_rbac_roleassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="718aa-126">属性</span><span class="sxs-lookup"><span data-stu-id="718aa-126">Properties</span></span>
|<span data-ttu-id="718aa-127">属性</span><span class="sxs-lookup"><span data-stu-id="718aa-127">Property</span></span>|<span data-ttu-id="718aa-128">类型</span><span class="sxs-lookup"><span data-stu-id="718aa-128">Type</span></span>|<span data-ttu-id="718aa-129">说明</span><span class="sxs-lookup"><span data-stu-id="718aa-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="718aa-130">id</span><span class="sxs-lookup"><span data-stu-id="718aa-130">id</span></span>|<span data-ttu-id="718aa-131">String</span><span class="sxs-lookup"><span data-stu-id="718aa-131">String</span></span>|<span data-ttu-id="718aa-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="718aa-132">Key of the entity.</span></span> <span data-ttu-id="718aa-133">此为只读，且自动生成。</span><span class="sxs-lookup"><span data-stu-id="718aa-133">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="718aa-134">displayName</span><span class="sxs-lookup"><span data-stu-id="718aa-134">displayName</span></span>|<span data-ttu-id="718aa-135">String</span><span class="sxs-lookup"><span data-stu-id="718aa-135">String</span></span>|<span data-ttu-id="718aa-136">角色分配的显示或友好名称。</span><span class="sxs-lookup"><span data-stu-id="718aa-136">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="718aa-137">description</span><span class="sxs-lookup"><span data-stu-id="718aa-137">description</span></span>|<span data-ttu-id="718aa-138">String</span><span class="sxs-lookup"><span data-stu-id="718aa-138">String</span></span>|<span data-ttu-id="718aa-139">角色分配的说明。</span><span class="sxs-lookup"><span data-stu-id="718aa-139">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="718aa-140">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="718aa-140">resourceScopes</span></span>|<span data-ttu-id="718aa-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="718aa-141">String collection</span></span>|<span data-ttu-id="718aa-142">角色作用域成员安全组的 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="718aa-142">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="718aa-143">这些是 Azure Active Directory 中的 ID。</span><span class="sxs-lookup"><span data-stu-id="718aa-143">These are IDs from Azure Active Directory.</span></span>|

## <a name="relationships"></a><span data-ttu-id="718aa-144">关系</span><span class="sxs-lookup"><span data-stu-id="718aa-144">Relationships</span></span>
|<span data-ttu-id="718aa-145">关系</span><span class="sxs-lookup"><span data-stu-id="718aa-145">Relationship</span></span>|<span data-ttu-id="718aa-146">类型</span><span class="sxs-lookup"><span data-stu-id="718aa-146">Type</span></span>|<span data-ttu-id="718aa-147">说明</span><span class="sxs-lookup"><span data-stu-id="718aa-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="718aa-148">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="718aa-148">roleDefinition</span></span>|[<span data-ttu-id="718aa-149">roleDefinition</span><span class="sxs-lookup"><span data-stu-id="718aa-149">roleDefinition</span></span>](../resources/intune_rbac_roledefinition.md)|<span data-ttu-id="718aa-150">此分配所属的角色定义。</span><span class="sxs-lookup"><span data-stu-id="718aa-150">Role definition this assignment is part of.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="718aa-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="718aa-151">JSON Representation</span></span>
<span data-ttu-id="718aa-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="718aa-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```



