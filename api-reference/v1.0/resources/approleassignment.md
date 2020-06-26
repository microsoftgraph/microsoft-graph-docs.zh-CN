---
title: appRoleAssignment 资源类型
description: 用于在将用户、组或服务主体分配给应用程序的服务主体上的应用程序角色时进行记录。 您可以创建、读取和删除应用程序角色分配。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ae7c770d97640f6af63dcb594b7f624fb119f1e6
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896789"
---
# <a name="approleassignment-resource-type"></a><span data-ttu-id="036b7-104">appRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="036b7-104">appRoleAssignment resource type</span></span>

<span data-ttu-id="036b7-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="036b7-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="036b7-106">用于记录何时向用户、组或服务主体分配应用程序的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="036b7-106">Used to record when a user, group, or service principal is assigned an app role for an app.</span></span>

<span data-ttu-id="036b7-107">应用程序角色分配是分配的主体（用户、组或服务主体）、资源应用程序（应用程序的服务主体）和在资源应用程序上定义的应用程序角色之间的关系。</span><span class="sxs-lookup"><span data-stu-id="036b7-107">An app role assignment is a relationship between the assigned principal (a user, a group, or a service principal), a resource application (the app's service principal) and an app role defined on the resource application.</span></span>

<span data-ttu-id="036b7-108">如果已分配给主体的[应用程序角色](approle.md)具有非空**值**属性，则会将其包含在使用者是分配主体的标记的**角色**声明中（例如，SAML 响应、ID 令牌、标识登录用户的访问令牌或标识服务主体的访问令牌）。</span><span class="sxs-lookup"><span data-stu-id="036b7-108">When the [app role](approle.md) which has been assigned to a principal has a non-empty **value** property, this will be included in the **roles** claim of tokens where the subject is the  assigned principal (e.g. SAML responses, ID tokens, access tokens identifying a signed-in user, or an access token identifying a service principal).</span></span> <span data-ttu-id="036b7-109">应用程序和 Api 将这些声明用作其授权逻辑的一部分。</span><span class="sxs-lookup"><span data-stu-id="036b7-109">Applications and APIs use these claims as part of their authorization logic.</span></span>

<span data-ttu-id="036b7-110">可以直接向用户分配应用角色。</span><span class="sxs-lookup"><span data-stu-id="036b7-110">A user can be assigned an app role directly.</span></span> <span data-ttu-id="036b7-111">如果将某个应用程序角色分配给某个组，则会将该组的直接成员视为已分配应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="036b7-111">If an app role is assigned to a group, direct members of the group are also considered to have been assigned the app role.</span></span> <span data-ttu-id="036b7-112">为用户分配应用程序的应用程序角色时，将在用户的[MyApps 门户](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)和[Microsoft 365 应用启动器](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a)中显示该应用程序的图块。</span><span class="sxs-lookup"><span data-stu-id="036b7-112">When a user is assigned an app role for an application, a tile for that application is displayed in the user's [MyApps portal](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access) and [Microsoft 365 app launcher](https://support.office.com/article/meet-the-office-365-app-launcher-79f12104-6fed-442f-96a0-eb089a3f476a).</span></span>

<span data-ttu-id="036b7-113">分配的主体是服务主体的应用程序角色分配是[仅限应用的权限](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types)授予。</span><span class="sxs-lookup"><span data-stu-id="036b7-113">An app role assignment where the assigned principal is a service principal is an [app-only permission](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#permission-types) grant.</span></span> <span data-ttu-id="036b7-114">当用户或管理员同意到仅应用程序的权限时，将创建一个应用程序角色分配，其中分配的主体是客户端应用程序的服务主体，而资源是目标 API 的服务主体。</span><span class="sxs-lookup"><span data-stu-id="036b7-114">When a user or admin consents to an app-only permission, an app role assignment is created where the assigned principal is the service principal for the client application, and the resource is the target API's service principal.</span></span>

## <a name="properties"></a><span data-ttu-id="036b7-115">属性</span><span class="sxs-lookup"><span data-stu-id="036b7-115">Properties</span></span>

| <span data-ttu-id="036b7-116">属性</span><span class="sxs-lookup"><span data-stu-id="036b7-116">Property</span></span> | <span data-ttu-id="036b7-117">类型</span><span class="sxs-lookup"><span data-stu-id="036b7-117">Type</span></span> | <span data-ttu-id="036b7-118">说明</span><span class="sxs-lookup"><span data-stu-id="036b7-118">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="036b7-119">id</span><span class="sxs-lookup"><span data-stu-id="036b7-119">id</span></span> | <span data-ttu-id="036b7-120">字符串</span><span class="sxs-lookup"><span data-stu-id="036b7-120">String</span></span> | <span data-ttu-id="036b7-121">**AppRoleAssignment**项的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="036b7-121">A unique identifier for the **appRoleAssignment** Key.</span></span> <span data-ttu-id="036b7-122">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="036b7-122">Not nullable.</span></span> <span data-ttu-id="036b7-123">只读。</span><span class="sxs-lookup"><span data-stu-id="036b7-123">Read-only.</span></span> |
| <span data-ttu-id="036b7-124">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="036b7-124">creationTimestamp</span></span> | <span data-ttu-id="036b7-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="036b7-125">DateTimeOffset</span></span> | <span data-ttu-id="036b7-126">应用程序角色分配的创建时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="036b7-126">The time when the app role assignment was created.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="036b7-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="036b7-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="036b7-128">只读。</span><span class="sxs-lookup"><span data-stu-id="036b7-128">Read-only.</span></span> <span data-ttu-id="036b7-129">不支持 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="036b7-129">Does not support `$filter`.</span></span> |
| <span data-ttu-id="036b7-130">principalId</span><span class="sxs-lookup"><span data-stu-id="036b7-130">principalId</span></span> | <span data-ttu-id="036b7-131">Guid</span><span class="sxs-lookup"><span data-stu-id="036b7-131">Guid</span></span> | <span data-ttu-id="036b7-132">为其授予应用程序角色的[用户](user.md)、[组](group.md)或[服务主体](serviceprincipal.md)的唯一标识符（**id**）。</span><span class="sxs-lookup"><span data-stu-id="036b7-132">The unique identifier (**id**) for the [user](user.md), [group](group.md) or [service principal](serviceprincipal.md) being granted the app role.</span></span> <span data-ttu-id="036b7-133">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="036b7-133">Required on create.</span></span> <span data-ttu-id="036b7-134">不支持 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="036b7-134">Does not support `$filter`.</span></span> |
| <span data-ttu-id="036b7-135">principalType</span><span class="sxs-lookup"><span data-stu-id="036b7-135">principalType</span></span> | <span data-ttu-id="036b7-136">String</span><span class="sxs-lookup"><span data-stu-id="036b7-136">String</span></span> | <span data-ttu-id="036b7-137">分配的主体的类型。</span><span class="sxs-lookup"><span data-stu-id="036b7-137">The type of the assigned principal.</span></span> <span data-ttu-id="036b7-138">它可以是“User”、“Group”或“ServicePrincipal”。</span><span class="sxs-lookup"><span data-stu-id="036b7-138">This can either be "User", "Group" or "ServicePrincipal".</span></span> <span data-ttu-id="036b7-139">只读。</span><span class="sxs-lookup"><span data-stu-id="036b7-139">Read-only.</span></span> <span data-ttu-id="036b7-140">不支持 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="036b7-140">Does not support `$filter`.</span></span> |
| <span data-ttu-id="036b7-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="036b7-141">principalDisplayName</span></span> | <span data-ttu-id="036b7-142">String</span><span class="sxs-lookup"><span data-stu-id="036b7-142">String</span></span> |<span data-ttu-id="036b7-143">向其授予应用程序角色分配的用户、组或服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="036b7-143">The display name of the user, group, or service principal that was granted the app role assignment.</span></span> <span data-ttu-id="036b7-144">只读。</span><span class="sxs-lookup"><span data-stu-id="036b7-144">Read-only.</span></span> <span data-ttu-id="036b7-145">支持 `$filter` （ `eq` 和 `startswith` ）。</span><span class="sxs-lookup"><span data-stu-id="036b7-145">Supports `$filter` (`eq` and `startswith`).</span></span> |
| <span data-ttu-id="036b7-146">resourceId</span><span class="sxs-lookup"><span data-stu-id="036b7-146">resourceId</span></span> | <span data-ttu-id="036b7-147">Guid</span><span class="sxs-lookup"><span data-stu-id="036b7-147">Guid</span></span> |<span data-ttu-id="036b7-148">为其进行分配的资源[服务主体](serviceprincipal.md)的唯一标识符（**id**）。</span><span class="sxs-lookup"><span data-stu-id="036b7-148">The unique identifier (**id**) for the resource [service principal](serviceprincipal.md) for which the assignment is made.</span></span> <span data-ttu-id="036b7-149">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="036b7-149">Required on create.</span></span> <span data-ttu-id="036b7-150">支持 `$filter` （ `eq` 仅限）。</span><span class="sxs-lookup"><span data-stu-id="036b7-150">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="036b7-151">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="036b7-151">resourceDisplayName</span></span> | <span data-ttu-id="036b7-152">String</span><span class="sxs-lookup"><span data-stu-id="036b7-152">String</span></span> | <span data-ttu-id="036b7-153">为其创建工作分配的资源应用程序的服务主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="036b7-153">The display name of the resource app's service principal to which the assignment is made.</span></span> <span data-ttu-id="036b7-154">不支持 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="036b7-154">Does not support `$filter`.</span></span> |
| <span data-ttu-id="036b7-155">appRoleId</span><span class="sxs-lookup"><span data-stu-id="036b7-155">appRoleId</span></span> | <span data-ttu-id="036b7-156">Guid</span><span class="sxs-lookup"><span data-stu-id="036b7-156">Guid</span></span> | <span data-ttu-id="036b7-157">分配给主体的[应用程序角色](approle.md)的标识符（**id**）。</span><span class="sxs-lookup"><span data-stu-id="036b7-157">The identifier (**id**) for the [app role](approle.md) which is assigned to the principal.</span></span> <span data-ttu-id="036b7-158">此应用程序角色必须在资源应用程序的服务主体（**resourceId**）的**appRoles**属性中公开。</span><span class="sxs-lookup"><span data-stu-id="036b7-158">This app role must be exposed in the **appRoles** property on the resource application's service principal (**resourceId**).</span></span> <span data-ttu-id="036b7-159">如果资源应用程序尚未声明任何应用角色，则可以指定一个默认的应用程序角色 ID，以指示将 `00000000-0000-0000-0000-000000000000` 主体分配给没有任何特定应用程序角色的资源应用程序。</span><span class="sxs-lookup"><span data-stu-id="036b7-159">If the resource application has not declared any app roles, a default app role ID of `00000000-0000-0000-0000-000000000000` can be specified to signal that the principal is assigned to the resource app without any specific app roles.</span></span> <span data-ttu-id="036b7-160">创建时为必需项。</span><span class="sxs-lookup"><span data-stu-id="036b7-160">Required on create.</span></span> <span data-ttu-id="036b7-161">不支持 `$filter` 。</span><span class="sxs-lookup"><span data-stu-id="036b7-161">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="036b7-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="036b7-162">JSON representation</span></span>

<span data-ttu-id="036b7-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="036b7-163">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRoleAssignment"
}-->

```json
{
  "id": "string",
  "creationTimestamp": "String (timestamp)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid",
  "appRoleId": "guid"
}
```

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
