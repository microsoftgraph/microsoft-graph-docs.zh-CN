---
title: directoryRole 资源类型
description: 表示 Azure AD 目录角色。 Azure AD 目录角色也称为*管理员角色*。 有关目录 (管理员) 角色的详细信息, 请参阅在 Azure AD 中分配管理员角色。 使用 Microsoft Graph, 可以将用户分配到目录角色, 以向他们授予目标角色的权限。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下仅激活公司管理员目录角色。 若要激活其他可用的目录角色, 请使用目录角色所基于的 directoryRoleTemplate 的 ID 发送 POST 请求。 继承自 directoryObject。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 30b22313da70c33bffc0b759f9b474f4deac2ac1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535264"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="9e2c9-110">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e2c9-110">directoryRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e2c9-111">表示 Azure AD 目录角色。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-111">Represents an Azure AD directory role.</span></span> <span data-ttu-id="9e2c9-112">Azure AD 目录角色也称为*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-112">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="9e2c9-113">有关目录 (管理员) 角色的详细信息, 请参阅[在 Azure AD 中分配管理员角色](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-113">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="9e2c9-114">使用 Microsoft Graph, 可以将用户分配到目录角色, 以向他们授予目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-114">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="9e2c9-115">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-115">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="9e2c9-116">默认情况下仅激活公司管理员目录角色。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-116">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="9e2c9-117">若要激活其他可用的目录角色, 请使用目录角色所基于的[directoryRoleTemplate](directoryroletemplate.md)的 ID 发送 POST 请求。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-117">To activate other available directory roles, you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="9e2c9-118">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-118">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="9e2c9-119">默认情况下, 目录角色的作用域为 "租户范围"。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-119">By default, directory roles are scoped to be tenant-wide.</span></span>  <span data-ttu-id="9e2c9-120">但是, 目录角色 (目前只有*用户帐户管理员*和*支持人员管理员*) 也可能作用于[管理单元](administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-120">However, directory roles (currently only the *user account admin* and *helpdesk admin*) may also be scoped to [administrative units](administrativeunit.md).</span></span>

<span data-ttu-id="9e2c9-121">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="9e2c9-121">This resource supports:</span></span>

- <span data-ttu-id="9e2c9-122">通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-122">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="9e2c9-123">方法</span><span class="sxs-lookup"><span data-stu-id="9e2c9-123">Methods</span></span>

| <span data-ttu-id="9e2c9-124">方法</span><span class="sxs-lookup"><span data-stu-id="9e2c9-124">Method</span></span>       | <span data-ttu-id="9e2c9-125">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e2c9-125">Return Type</span></span>  |<span data-ttu-id="9e2c9-126">说明</span><span class="sxs-lookup"><span data-stu-id="9e2c9-126">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9e2c9-127">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="9e2c9-127">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="9e2c9-128">directoryRole</span><span class="sxs-lookup"><span data-stu-id="9e2c9-128">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="9e2c9-129">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-129">Read properties and relationships of directoryRole object.</span></span>|
|[<span data-ttu-id="9e2c9-130">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="9e2c9-130">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="9e2c9-131">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2c9-131">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="9e2c9-132">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-132">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="9e2c9-133">Add member</span><span class="sxs-lookup"><span data-stu-id="9e2c9-133">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="9e2c9-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9e2c9-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9e2c9-135">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-135">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="9e2c9-136">列出成员</span><span class="sxs-lookup"><span data-stu-id="9e2c9-136">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9e2c9-137">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="9e2c9-137">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="9e2c9-138">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-138">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="9e2c9-139">删除成员</span><span class="sxs-lookup"><span data-stu-id="9e2c9-139">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="9e2c9-140">directoryObject</span><span class="sxs-lookup"><span data-stu-id="9e2c9-140">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="9e2c9-141">从目录角色中删除用户。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-141">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="9e2c9-142">列出作用域内的角色成员</span><span class="sxs-lookup"><span data-stu-id="9e2c9-142">List scoped-role members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="9e2c9-143">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2c9-143">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9e2c9-144">通过 scopedRoleMembership 资源集合列出此目录角色的范围限定为[管理单元](administrativeunit.md)的成员。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-144">List the members of this directory role that are scoped to [administrative units](administrativeunit.md), through the scopedRoleMembership resource collection.</span></span>|
|[<span data-ttu-id="9e2c9-145">delta</span><span class="sxs-lookup"><span data-stu-id="9e2c9-145">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="9e2c9-146">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="9e2c9-146">directoryRole collection</span></span>| <span data-ttu-id="9e2c9-147">获取目录角色的增量更改。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-147">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e2c9-148">属性</span><span class="sxs-lookup"><span data-stu-id="9e2c9-148">Properties</span></span>
| <span data-ttu-id="9e2c9-149">属性</span><span class="sxs-lookup"><span data-stu-id="9e2c9-149">Property</span></span>   | <span data-ttu-id="9e2c9-150">类型</span><span class="sxs-lookup"><span data-stu-id="9e2c9-150">Type</span></span> |<span data-ttu-id="9e2c9-151">说明</span><span class="sxs-lookup"><span data-stu-id="9e2c9-151">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e2c9-152">说明</span><span class="sxs-lookup"><span data-stu-id="9e2c9-152">description</span></span>|<span data-ttu-id="9e2c9-153">String</span><span class="sxs-lookup"><span data-stu-id="9e2c9-153">String</span></span>|<span data-ttu-id="9e2c9-p104">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-p104">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9e2c9-156">displayName</span><span class="sxs-lookup"><span data-stu-id="9e2c9-156">displayName</span></span>|<span data-ttu-id="9e2c9-157">字符串</span><span class="sxs-lookup"><span data-stu-id="9e2c9-157">String</span></span>|<span data-ttu-id="9e2c9-p105">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-p105">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="9e2c9-160">id</span><span class="sxs-lookup"><span data-stu-id="9e2c9-160">id</span></span>|<span data-ttu-id="9e2c9-161">字符串</span><span class="sxs-lookup"><span data-stu-id="9e2c9-161">String</span></span>|<span data-ttu-id="9e2c9-p106">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-p106">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="9e2c9-165">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="9e2c9-165">roleTemplateId</span></span>|<span data-ttu-id="9e2c9-166">String</span><span class="sxs-lookup"><span data-stu-id="9e2c9-166">String</span></span>| <span data-ttu-id="9e2c9-p107">此角色所基于的 **directoryRoleTemplate** 的 [id](directoryroletemplate.md)。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-p107">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9e2c9-170">关系</span><span class="sxs-lookup"><span data-stu-id="9e2c9-170">Relationships</span></span>
| <span data-ttu-id="9e2c9-171">关系</span><span class="sxs-lookup"><span data-stu-id="9e2c9-171">Relationship</span></span> | <span data-ttu-id="9e2c9-172">类型</span><span class="sxs-lookup"><span data-stu-id="9e2c9-172">Type</span></span> |<span data-ttu-id="9e2c9-173">说明</span><span class="sxs-lookup"><span data-stu-id="9e2c9-173">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e2c9-174">members</span><span class="sxs-lookup"><span data-stu-id="9e2c9-174">members</span></span>|<span data-ttu-id="9e2c9-175">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2c9-175">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="9e2c9-p108">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-p108">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|
|<span data-ttu-id="9e2c9-180">scopedMembers</span><span class="sxs-lookup"><span data-stu-id="9e2c9-180">scopedMembers</span></span>|<span data-ttu-id="9e2c9-181">[scopedRoleMembership](scopedrolemembership.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e2c9-181">[scopedRoleMembership](scopedrolemembership.md) collection</span></span>| <span data-ttu-id="9e2c9-182">此目录角色的作用域为 "[管理单元](administrativeunit.md)" 的成员。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-182">Members of this directory role that are scoped to [administrative units](administrativeunit.md).</span></span> <span data-ttu-id="9e2c9-183">只读。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-183">Read-only.</span></span> <span data-ttu-id="9e2c9-184">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-184">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e2c9-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e2c9-185">JSON representation</span></span>

<span data-ttu-id="9e2c9-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e2c9-186">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "directoryRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/directoryrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
