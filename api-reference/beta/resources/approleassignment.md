---
title: appRoleAssignment 资源类型
description: 用于记录时用户或组分配给应用程序。 在这种情况下，该角色分配将导致应用程序图块显示安装在用户的应用程序访问面板上。 此实体还可能用于授予对特定的角色中的资源应用程序的另一个应用程序 （作为服务主体建模） 访问权限。 您可以创建、 读取、 更新和删除角色分配。
ms.openlocfilehash: 97155bde12735ebd8a7674e0dbf20dae30e53f14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042934"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="5f66b-106">appRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f66b-106">appRoleAssignment resource type</span></span>

> <span data-ttu-id="5f66b-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5f66b-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f66b-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f66b-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f66b-109">用于记录时用户或组分配给应用程序。</span><span class="sxs-lookup"><span data-stu-id="5f66b-109">Used to record when a user or group is assigned to an application.</span></span> <span data-ttu-id="5f66b-110">在这种情况下，该角色分配将导致应用程序图块显示安装在用户的应用程序访问面板上。</span><span class="sxs-lookup"><span data-stu-id="5f66b-110">In this case, the role assignment will result in an application tile showing up on the user's app access panel.</span></span> <span data-ttu-id="5f66b-111">此实体还可能用于授予对特定的角色中的资源应用程序的另一个应用程序 （作为服务主体建模） 访问权限。</span><span class="sxs-lookup"><span data-stu-id="5f66b-111">This entity may also be used to grant another application (modeled as a service principal) access to a resource application in a particular role.</span></span> <span data-ttu-id="5f66b-112">您可以创建、 读取、 更新和删除角色分配。</span><span class="sxs-lookup"><span data-stu-id="5f66b-112">You can create, read, update, and delete role assignments.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5f66b-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f66b-113">JSON representation</span></span>

<span data-ttu-id="5f66b-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f66b-114">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
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
## <a name="properties"></a><span data-ttu-id="5f66b-115">属性</span><span class="sxs-lookup"><span data-stu-id="5f66b-115">Properties</span></span>
| <span data-ttu-id="5f66b-116">属性</span><span class="sxs-lookup"><span data-stu-id="5f66b-116">Property</span></span>     | <span data-ttu-id="5f66b-117">类型</span><span class="sxs-lookup"><span data-stu-id="5f66b-117">Type</span></span>   |<span data-ttu-id="5f66b-118">说明</span><span class="sxs-lookup"><span data-stu-id="5f66b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f66b-119">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="5f66b-119">creationTimestamp</span></span>|<span data-ttu-id="5f66b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f66b-120">DateTimeOffset</span></span>|<span data-ttu-id="5f66b-121">授予创建时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="5f66b-121">The time when the grant was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5f66b-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5f66b-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5f66b-123">id</span><span class="sxs-lookup"><span data-stu-id="5f66b-123">id</span></span>|<span data-ttu-id="5f66b-124">Guid</span><span class="sxs-lookup"><span data-stu-id="5f66b-124">Guid</span></span>|<span data-ttu-id="5f66b-125">已分配给主体角色 id。</span><span class="sxs-lookup"><span data-stu-id="5f66b-125">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="5f66b-126">必须由其**appRoles**属性中目标资源应用程序**resourceId**声明此角色。</span><span class="sxs-lookup"><span data-stu-id="5f66b-126">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="5f66b-127">如果资源没有声明任何权限，必须指定默认 id (零 GUID)。</span><span class="sxs-lookup"><span data-stu-id="5f66b-127">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span> <span data-ttu-id="5f66b-128">键。</span><span class="sxs-lookup"><span data-stu-id="5f66b-128">Key.</span></span> <span data-ttu-id="5f66b-129">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="5f66b-129">Not nullable.</span></span> |
|<span data-ttu-id="5f66b-130">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="5f66b-130">principalDisplayName</span></span>|<span data-ttu-id="5f66b-131">字符串</span><span class="sxs-lookup"><span data-stu-id="5f66b-131">String</span></span>|<span data-ttu-id="5f66b-132">已授予访问权限的主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5f66b-132">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="5f66b-133">principalId</span><span class="sxs-lookup"><span data-stu-id="5f66b-133">principalId</span></span>|<span data-ttu-id="5f66b-134">Guid</span><span class="sxs-lookup"><span data-stu-id="5f66b-134">Guid</span></span>|<span data-ttu-id="5f66b-135">要授予访问权限的主体的唯一标识符 (**id**)。</span><span class="sxs-lookup"><span data-stu-id="5f66b-135">The unique identifier (**id**) for the principal being granted the access.</span></span> <span data-ttu-id="5f66b-136">所需在创建。</span><span class="sxs-lookup"><span data-stu-id="5f66b-136">Required on create.</span></span>            |
|<span data-ttu-id="5f66b-137">principalType</span><span class="sxs-lookup"><span data-stu-id="5f66b-137">principalType</span></span>|<span data-ttu-id="5f66b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="5f66b-138">String</span></span>|<span data-ttu-id="5f66b-139">主体的类型。</span><span class="sxs-lookup"><span data-stu-id="5f66b-139">The type of principal.</span></span>  <span data-ttu-id="5f66b-140">这可以是"User"，"组"或"ServicePrincipal"。</span><span class="sxs-lookup"><span data-stu-id="5f66b-140">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="5f66b-141">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5f66b-141">resourceDisplayName</span></span>|<span data-ttu-id="5f66b-142">字符串</span><span class="sxs-lookup"><span data-stu-id="5f66b-142">String</span></span>|<span data-ttu-id="5f66b-143">对其进行分配资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5f66b-143">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="5f66b-144">resourceId</span><span class="sxs-lookup"><span data-stu-id="5f66b-144">resourceId</span></span>|<span data-ttu-id="5f66b-145">Guid</span><span class="sxs-lookup"><span data-stu-id="5f66b-145">Guid</span></span>|<span data-ttu-id="5f66b-146">唯一标识符 (**id**) 为其进行工作分配的目标资源 （服务主体）。</span><span class="sxs-lookup"><span data-stu-id="5f66b-146">The unique identifier (**id**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f66b-147">Relationships</span><span class="sxs-lookup"><span data-stu-id="5f66b-147">Relationships</span></span>
<span data-ttu-id="5f66b-148">无</span><span class="sxs-lookup"><span data-stu-id="5f66b-148">None</span></span>


## <a name="methods"></a><span data-ttu-id="5f66b-149">方法</span><span class="sxs-lookup"><span data-stu-id="5f66b-149">Methods</span></span>

| <span data-ttu-id="5f66b-150">方法</span><span class="sxs-lookup"><span data-stu-id="5f66b-150">Method</span></span>           | <span data-ttu-id="5f66b-151">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f66b-151">Return Type</span></span>    |<span data-ttu-id="5f66b-152">说明</span><span class="sxs-lookup"><span data-stu-id="5f66b-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f66b-153">获取 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f66b-153">Get appRoleAssignment</span></span>](../api/approleassignment-get.md) | [<span data-ttu-id="5f66b-154">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f66b-154">appRoleAssignment</span></span>](approleassignment.md) |<span data-ttu-id="5f66b-155">读取属性和 appRoleAssignment 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="5f66b-155">Read properties and relationships of appRoleAssignment object.</span></span>|
|[<span data-ttu-id="5f66b-156">Update</span><span class="sxs-lookup"><span data-stu-id="5f66b-156">Update</span></span>](../api/approleassignment-update.md) | [<span data-ttu-id="5f66b-157">appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f66b-157">appRoleAssignment</span></span>](approleassignment.md)   |<span data-ttu-id="5f66b-158">更新 appRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="5f66b-158">Update appRoleAssignment object.</span></span> |
|[<span data-ttu-id="5f66b-159">删除</span><span class="sxs-lookup"><span data-stu-id="5f66b-159">Delete</span></span>](../api/approleassignment-delete.md) | <span data-ttu-id="5f66b-160">无</span><span class="sxs-lookup"><span data-stu-id="5f66b-160">None</span></span> |<span data-ttu-id="5f66b-161">删除 appRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="5f66b-161">Delete appRoleAssignment object.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->