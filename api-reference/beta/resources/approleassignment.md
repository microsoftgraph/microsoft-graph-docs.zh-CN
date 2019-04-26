---
title: appRoleAssignment 资源类型
description: 用于记录用户或组何时被分配到应用程序。 在这种情况下，角色分配会导致用户应用访问面板上显示应用程序磁贴。 此实体还可用于授予其他应用程序（建模为服务主体）以特定角色访问资源应用程序的权限。 您可以创建、读取、更新和删除角色分配。
localization_priority: Priority
ms.openlocfilehash: 37942e45f804efaec3e94f8fe9b582e103628025
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339004"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="d31cc-106">appRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d31cc-106">appRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d31cc-107">用于记录用户或组何时被分配到应用程序。</span><span class="sxs-lookup"><span data-stu-id="d31cc-107">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="d31cc-108">在这种情况下，角色分配会导致用户应用访问面板上显示应用程序磁贴。</span><span class="sxs-lookup"><span data-stu-id="d31cc-108">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="d31cc-109">此实体还可用于授予其他应用程序（建模为服务主体）以特定角色访问资源应用程序的权限。</span><span class="sxs-lookup"><span data-stu-id="d31cc-109">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="d31cc-110">您可以创建、读取、更新和删除角色分配。</span><span class="sxs-lookup"><span data-stu-id="d31cc-110">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d31cc-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d31cc-111">JSON representation</span></span>

<span data-ttu-id="d31cc-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d31cc-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a><span data-ttu-id="d31cc-113">属性</span><span class="sxs-lookup"><span data-stu-id="d31cc-113">Properties</span></span>
| <span data-ttu-id="d31cc-114">属性</span><span class="sxs-lookup"><span data-stu-id="d31cc-114">Property</span></span>     | <span data-ttu-id="d31cc-115">类型</span><span class="sxs-lookup"><span data-stu-id="d31cc-115">Type</span></span>   |<span data-ttu-id="d31cc-116">说明</span><span class="sxs-lookup"><span data-stu-id="d31cc-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d31cc-117">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="d31cc-117">creationTimestamp</span></span>|<span data-ttu-id="d31cc-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d31cc-118">DateTimeOffset</span></span>|<span data-ttu-id="d31cc-119">创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：</span><span class="sxs-lookup"><span data-stu-id="d31cc-119">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d31cc-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d31cc-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d31cc-121">id</span><span class="sxs-lookup"><span data-stu-id="d31cc-121">id</span></span>|<span data-ttu-id="d31cc-122">Guid</span><span class="sxs-lookup"><span data-stu-id="d31cc-122">Guid</span></span>|<span data-ttu-id="d31cc-123">向主体分配的角色 id。</span><span class="sxs-lookup"><span data-stu-id="d31cc-123">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="d31cc-124">此角色必须由目标资源应用程序 **resourceId** 在其 **appRoles** 属性中声明。</span><span class="sxs-lookup"><span data-stu-id="d31cc-124">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="d31cc-125">如果资源未声明任何权限，则必须指定默认 id (0 GUID)。</span><span class="sxs-lookup"><span data-stu-id="d31cc-125">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="d31cc-126">密钥。</span><span class="sxs-lookup"><span data-stu-id="d31cc-126">Key.</span></span> <span data-ttu-id="d31cc-127">不可为空。</span><span class="sxs-lookup"><span data-stu-id="d31cc-127">Not nullable.</span></span> |
|<span data-ttu-id="d31cc-128">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="d31cc-128">principalDisplayName</span></span>|<span data-ttu-id="d31cc-129">String</span><span class="sxs-lookup"><span data-stu-id="d31cc-129">String</span></span>|<span data-ttu-id="d31cc-130">已授权访问权限的主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d31cc-130">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="d31cc-131">principalId</span><span class="sxs-lookup"><span data-stu-id="d31cc-131">principalId</span></span>|<span data-ttu-id="d31cc-132">Guid</span><span class="sxs-lookup"><span data-stu-id="d31cc-132">Guid</span></span>|<span data-ttu-id="d31cc-133">授予访问权限的主体的唯一标识符 (**id**)。</span><span class="sxs-lookup"><span data-stu-id="d31cc-133">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="d31cc-134">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="d31cc-134">Required on create.</span></span>            |
|<span data-ttu-id="d31cc-135">principalType</span><span class="sxs-lookup"><span data-stu-id="d31cc-135">principalType</span></span>|<span data-ttu-id="d31cc-136">String</span><span class="sxs-lookup"><span data-stu-id="d31cc-136">String</span></span>|<span data-ttu-id="d31cc-137">主体类型。</span><span class="sxs-lookup"><span data-stu-id="d31cc-137">The type of principal.</span></span>  <span data-ttu-id="d31cc-138">它可以是“User”、“Group”或“ServicePrincipal”。</span><span class="sxs-lookup"><span data-stu-id="d31cc-138">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="d31cc-139">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d31cc-139">resourceDisplayName</span></span>|<span data-ttu-id="d31cc-140">String</span><span class="sxs-lookup"><span data-stu-id="d31cc-140">String</span></span>|<span data-ttu-id="d31cc-141">已对其进行分配的资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d31cc-141">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="d31cc-142">resourceId</span><span class="sxs-lookup"><span data-stu-id="d31cc-142">resourceId</span></span>|<span data-ttu-id="d31cc-143">Guid</span><span class="sxs-lookup"><span data-stu-id="d31cc-143">Guid</span></span>|<span data-ttu-id="d31cc-144">已为其分配目标资源（服务主体）的唯一标识符 (**id**)。</span><span class="sxs-lookup"><span data-stu-id="d31cc-144">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d31cc-145">关系</span><span class="sxs-lookup"><span data-stu-id="d31cc-145">Relationships</span></span>
<span data-ttu-id="d31cc-146">无</span><span class="sxs-lookup"><span data-stu-id="d31cc-146">None</span></span>


## <a name="methods"></a><span data-ttu-id="d31cc-147">方法</span><span class="sxs-lookup"><span data-stu-id="d31cc-147">Methods</span></span>

| <span data-ttu-id="d31cc-148">方法</span><span class="sxs-lookup"><span data-stu-id="d31cc-148">Method</span></span>           | <span data-ttu-id="d31cc-149">返回类型</span><span class="sxs-lookup"><span data-stu-id="d31cc-149">Return Type</span></span>    |<span data-ttu-id="d31cc-150">说明</span><span class="sxs-lookup"><span data-stu-id="d31cc-150">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d31cc-151">获取 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d31cc-151">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="d31cc-152">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d31cc-152">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="d31cc-153">读取 appRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d31cc-153">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="d31cc-154">更新</span><span class="sxs-lookup"><span data-stu-id="d31cc-154">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="d31cc-155">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d31cc-155">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="d31cc-156">更新 appRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="d31cc-156">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="d31cc-157">删除</span><span class="sxs-lookup"><span data-stu-id="d31cc-157">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="d31cc-158">无</span><span class="sxs-lookup"><span data-stu-id="d31cc-158">None</span></span> |<span data-ttu-id="d31cc-159">删除 appRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="d31cc-159">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
