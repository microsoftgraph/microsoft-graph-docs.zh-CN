---
title: directoryRole 资源类型
description: 表示 Azure AD 目录角色。 Azure AD 目录角色也称为是*管理员角色*。 有关目录 （管理员） 角色的详细信息，请参阅 Azure AD 中分配管理员角色。 使用 Microsoft Graph 中，可以将用户分配到目录角色授予他们的目标角色的权限。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下已激活公司管理员的目录角色。 要激活其他可用的目录角色，您发送一个 POST 请求 directoryRoleTemplate 目录角色所基于的 id。 继承自 directoryObject。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e6753369be070ab04419cab0c870aec7e96b1fb2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927742"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="6b6f1-110">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b6f1-110">directoryRole resource type</span></span>

> <span data-ttu-id="6b6f1-111">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-111">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b6f1-112">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-112">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b6f1-113">表示 Azure AD 目录角色。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-113">Represents an Azure AD directory role.</span></span> <span data-ttu-id="6b6f1-114">Azure AD 目录角色也称为是*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-114">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="6b6f1-115">有关目录 （管理员） 角色的详细信息，请参阅[Azure AD 中的分配管理员角色](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-115">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="6b6f1-116">使用 Microsoft Graph 中，可以将用户分配到目录角色授予他们的目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-116">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="6b6f1-117">若要读取目录角色或更新其成员，它必须首先激活在租户中。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-117">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="6b6f1-118">默认情况下已激活公司管理员的目录角色。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-118">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="6b6f1-119">若要激活其他可用的目录角色，请将发送一个 POST 请求[directoryRoleTemplate](directoryroletemplate.md)目录角色所基于的 id。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-119">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="6b6f1-120">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-120">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="6b6f1-121">默认情况下，范围是目录角色为租户范围。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-121">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="6b6f1-122">但是，也可能为[管理单位](administrativeunit.md)范围目录角色 （当前仅*用户帐户管理员*和*技术支持管理员*）。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-122">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="6b6f1-123">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="6b6f1-123">This resource supports:</span></span>

- <span data-ttu-id="6b6f1-124">通过提供 [delta](../api/directoryrole-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-124">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="6b6f1-125">方法</span><span class="sxs-lookup"><span data-stu-id="6b6f1-125">Methods</span></span>

| <span data-ttu-id="6b6f1-126">方法</span><span class="sxs-lookup"><span data-stu-id="6b6f1-126">Method</span></span>       | <span data-ttu-id="6b6f1-127">返回类型</span><span class="sxs-lookup"><span data-stu-id="6b6f1-127">Return Type</span></span>  |<span data-ttu-id="6b6f1-128">说明</span><span class="sxs-lookup"><span data-stu-id="6b6f1-128">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b6f1-129">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b6f1-129">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="6b6f1-130">directoryRole</span><span class="sxs-lookup"><span data-stu-id="6b6f1-130">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="6b6f1-131">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-131">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="6b6f1-132">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="6b6f1-132">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="6b6f1-133">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6f1-133">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="6b6f1-134">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-134">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="6b6f1-135">添加成员</span><span class="sxs-lookup"><span data-stu-id="6b6f1-135">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="6b6f1-136">directoryObject</span><span class="sxs-lookup"><span data-stu-id="6b6f1-136">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="6b6f1-137">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-137">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="6b6f1-138">列出成员</span><span class="sxs-lookup"><span data-stu-id="6b6f1-138">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="6b6f1-139">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6f1-139">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="6b6f1-140">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-140">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="6b6f1-141">删除成员</span><span class="sxs-lookup"><span data-stu-id="6b6f1-141">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="6b6f1-142">directoryObject</span><span class="sxs-lookup"><span data-stu-id="6b6f1-142">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="6b6f1-143">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-143">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="6b6f1-144">列表范围内的角色成员</span><span class="sxs-lookup"><span data-stu-id="6b6f1-144">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="6b6f1-145">[scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="6b6f1-145">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="6b6f1-146">列出的范围为[管理单元](administrativeunit.md)，通过 scopedRoleMembership 资源集合此目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-146">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="6b6f1-147">delta</span><span class="sxs-lookup"><span data-stu-id="6b6f1-147">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="6b6f1-148">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="6b6f1-148">directoryRole collection</span></span>| <span data-ttu-id="6b6f1-149">获得目录角色增量更改。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-149">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="6b6f1-150">属性</span><span class="sxs-lookup"><span data-stu-id="6b6f1-150">Properties</span></span>
| <span data-ttu-id="6b6f1-151">属性</span><span class="sxs-lookup"><span data-stu-id="6b6f1-151">Property</span></span>   | <span data-ttu-id="6b6f1-152">类型</span><span class="sxs-lookup"><span data-stu-id="6b6f1-152">Type</span></span> |<span data-ttu-id="6b6f1-153">说明</span><span class="sxs-lookup"><span data-stu-id="6b6f1-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b6f1-154">说明</span><span class="sxs-lookup"><span data-stu-id="6b6f1-154">description</span></span>|<span data-ttu-id="6b6f1-155">String</span><span class="sxs-lookup"><span data-stu-id="6b6f1-155">String</span></span>|<span data-ttu-id="6b6f1-p105">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-p105">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="6b6f1-158">displayName</span><span class="sxs-lookup"><span data-stu-id="6b6f1-158">displayName</span></span>|<span data-ttu-id="6b6f1-159">String</span><span class="sxs-lookup"><span data-stu-id="6b6f1-159">String</span></span>|<span data-ttu-id="6b6f1-p106">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-p106">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="6b6f1-162">id</span><span class="sxs-lookup"><span data-stu-id="6b6f1-162">id</span></span>|<span data-ttu-id="6b6f1-163">String</span><span class="sxs-lookup"><span data-stu-id="6b6f1-163">String</span></span>|<span data-ttu-id="6b6f1-p107">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-p107">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="6b6f1-167">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="6b6f1-167">roleTemplateId</span></span>|<span data-ttu-id="6b6f1-168">String</span><span class="sxs-lookup"><span data-stu-id="6b6f1-168">String</span></span>| <span data-ttu-id="6b6f1-p108">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-p108">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6b6f1-172">关系</span><span class="sxs-lookup"><span data-stu-id="6b6f1-172">Relationships</span></span>
| <span data-ttu-id="6b6f1-173">关系</span><span class="sxs-lookup"><span data-stu-id="6b6f1-173">Relationship</span></span> | <span data-ttu-id="6b6f1-174">类型</span><span class="sxs-lookup"><span data-stu-id="6b6f1-174">Type</span></span> |<span data-ttu-id="6b6f1-175">说明</span><span class="sxs-lookup"><span data-stu-id="6b6f1-175">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b6f1-176">members</span><span class="sxs-lookup"><span data-stu-id="6b6f1-176">members</span></span>|<span data-ttu-id="6b6f1-177">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6b6f1-177">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="6b6f1-p109">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-p109">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="6b6f1-182">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="6b6f1-182">scopedMembers</span></span>|<span data-ttu-id="6b6f1-183">[scopedRoleMembership](scopedrolemembership.md)</span><span class="sxs-lookup"><span data-stu-id="6b6f1-183">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="6b6f1-184">为[管理单位](administrativeunit.md)范围此目录角色的成员。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-184">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="6b6f1-185">只读。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-185">Read-only.</span></span> <span data-ttu-id="6b6f1-186">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-186">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b6f1-187">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b6f1-187">JSON representation</span></span>

<span data-ttu-id="6b6f1-188">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b6f1-188">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "roleTemplateId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
