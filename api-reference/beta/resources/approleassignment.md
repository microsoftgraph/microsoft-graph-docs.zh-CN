---
title: appRoleAssignment 资源类型
description: 用于记录用户或组何时被分配到应用程序。 在这种情况下，角色分配会导致用户应用访问面板上显示应用程序磁贴。 此实体还可用于授予其他应用程序（建模为服务主体）以特定角色访问资源应用程序的权限。 您可以创建、读取、更新和删除角色分配。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 5a0b9faeb68e11f465e8b5ddb177351e9a0f44d6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508238"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="afe75-106">appRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="afe75-106">appRoleAssignment resource type</span></span>

<span data-ttu-id="afe75-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afe75-107">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afe75-108">用于记录用户或组何时被分配到应用程序。</span><span class="sxs-lookup"><span data-stu-id="afe75-108">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="afe75-109">在这种情况下，角色分配会导致用户应用访问面板上显示应用程序磁贴。</span><span class="sxs-lookup"><span data-stu-id="afe75-109">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="afe75-110">此实体还可用于授予其他应用程序（建模为服务主体）以特定角色访问资源应用程序的权限。</span><span class="sxs-lookup"><span data-stu-id="afe75-110">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="afe75-111">您可以创建、读取、更新和删除角色分配。</span><span class="sxs-lookup"><span data-stu-id="afe75-111">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="afe75-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afe75-112">JSON representation</span></span>

<span data-ttu-id="afe75-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afe75-113">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="afe75-114">属性</span><span class="sxs-lookup"><span data-stu-id="afe75-114">Properties</span></span>
| <span data-ttu-id="afe75-115">属性</span><span class="sxs-lookup"><span data-stu-id="afe75-115">Property</span></span>     | <span data-ttu-id="afe75-116">类型</span><span class="sxs-lookup"><span data-stu-id="afe75-116">Type</span></span>   |<span data-ttu-id="afe75-117">说明</span><span class="sxs-lookup"><span data-stu-id="afe75-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="afe75-118">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="afe75-118">creationTimestamp</span></span>|<span data-ttu-id="afe75-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afe75-119">DateTimeOffset</span></span>|<span data-ttu-id="afe75-120">创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：</span><span class="sxs-lookup"><span data-stu-id="afe75-120">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="afe75-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="afe75-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="afe75-122">id</span><span class="sxs-lookup"><span data-stu-id="afe75-122">id</span></span>|<span data-ttu-id="afe75-123">Guid</span><span class="sxs-lookup"><span data-stu-id="afe75-123">Guid</span></span>|<span data-ttu-id="afe75-124">向主体分配的角色 id。</span><span class="sxs-lookup"><span data-stu-id="afe75-124">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="afe75-125">此角色必须由目标资源应用程序 **resourceId** 在其 **appRoles** 属性中声明。</span><span class="sxs-lookup"><span data-stu-id="afe75-125">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="afe75-126">如果资源未声明任何权限，则必须指定默认 id (0 GUID)。</span><span class="sxs-lookup"><span data-stu-id="afe75-126">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="afe75-127">密钥。</span><span class="sxs-lookup"><span data-stu-id="afe75-127">Key.</span></span> <span data-ttu-id="afe75-128">不可为空。</span><span class="sxs-lookup"><span data-stu-id="afe75-128">Not nullable.</span></span> |
|<span data-ttu-id="afe75-129">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="afe75-129">principalDisplayName</span></span>|<span data-ttu-id="afe75-130">String</span><span class="sxs-lookup"><span data-stu-id="afe75-130">String</span></span>|<span data-ttu-id="afe75-131">已授权访问权限的主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="afe75-131">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="afe75-132">principalId</span><span class="sxs-lookup"><span data-stu-id="afe75-132">principalId</span></span>|<span data-ttu-id="afe75-133">Guid</span><span class="sxs-lookup"><span data-stu-id="afe75-133">Guid</span></span>|<span data-ttu-id="afe75-134">授予访问权限的主体的唯一标识符 (**id**)。</span><span class="sxs-lookup"><span data-stu-id="afe75-134">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="afe75-135">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="afe75-135">Required on create.</span></span>            |
|<span data-ttu-id="afe75-136">principalType</span><span class="sxs-lookup"><span data-stu-id="afe75-136">principalType</span></span>|<span data-ttu-id="afe75-137">String</span><span class="sxs-lookup"><span data-stu-id="afe75-137">String</span></span>|<span data-ttu-id="afe75-138">主体类型。</span><span class="sxs-lookup"><span data-stu-id="afe75-138">The type of principal.</span></span>  <span data-ttu-id="afe75-139">它可以是“User”、“Group”或“ServicePrincipal”。</span><span class="sxs-lookup"><span data-stu-id="afe75-139">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="afe75-140">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="afe75-140">resourceDisplayName</span></span>|<span data-ttu-id="afe75-141">String</span><span class="sxs-lookup"><span data-stu-id="afe75-141">String</span></span>|<span data-ttu-id="afe75-142">已对其进行分配的资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="afe75-142">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="afe75-143">resourceId</span><span class="sxs-lookup"><span data-stu-id="afe75-143">resourceId</span></span>|<span data-ttu-id="afe75-144">Guid</span><span class="sxs-lookup"><span data-stu-id="afe75-144">Guid</span></span>|<span data-ttu-id="afe75-145">已为其分配目标资源（服务主体）的唯一标识符 (**id**)。</span><span class="sxs-lookup"><span data-stu-id="afe75-145">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="afe75-146">关系</span><span class="sxs-lookup"><span data-stu-id="afe75-146">Relationships</span></span>
<span data-ttu-id="afe75-147">无</span><span class="sxs-lookup"><span data-stu-id="afe75-147">None</span></span>


## <a name="methods"></a><span data-ttu-id="afe75-148">方法</span><span class="sxs-lookup"><span data-stu-id="afe75-148">Methods</span></span>

| <span data-ttu-id="afe75-149">方法</span><span class="sxs-lookup"><span data-stu-id="afe75-149">Method</span></span>           | <span data-ttu-id="afe75-150">返回类型</span><span class="sxs-lookup"><span data-stu-id="afe75-150">Return Type</span></span>    |<span data-ttu-id="afe75-151">说明</span><span class="sxs-lookup"><span data-stu-id="afe75-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="afe75-152">获取 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="afe75-152">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="afe75-153">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="afe75-153">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="afe75-154">读取 appRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="afe75-154">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="afe75-155">更新</span><span class="sxs-lookup"><span data-stu-id="afe75-155">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="afe75-156">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="afe75-156">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="afe75-157">更新 appRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="afe75-157">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="afe75-158">删除</span><span class="sxs-lookup"><span data-stu-id="afe75-158">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="afe75-159">无</span><span class="sxs-lookup"><span data-stu-id="afe75-159">None</span></span> |<span data-ttu-id="afe75-160">删除 appRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="afe75-160">Delete appRoleAssignment object.</span></span> |

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
