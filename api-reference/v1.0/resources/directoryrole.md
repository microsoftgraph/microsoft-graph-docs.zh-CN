---
title: directoryRole 资源类型
description: 表示 Azure AD Directory 角色。 Azure AD 目录角色也称作*管理员角色*。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d9b500e3f5a3768dd345d1e7e8df41c63b1aa54b
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450674"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="5f915-104">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f915-104">directoryRole resource type</span></span>

<span data-ttu-id="5f915-105">表示 Azure AD Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="5f915-105">Represents an Azure AD directory role.</span></span> <span data-ttu-id="5f915-106">Azure AD 目录角色也称作*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="5f915-106">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="5f915-107">有关这些目录（管理员）角色的详细信息，请参阅 [在 Azure AD 中分配管理员角色](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)</span><span class="sxs-lookup"><span data-stu-id="5f915-107">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="5f915-108">使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="5f915-108">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="5f915-109">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="5f915-109">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="5f915-110">默认情况下，仅激活公司管理员目录角色。</span><span class="sxs-lookup"><span data-stu-id="5f915-110">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="5f915-111">若要激活其他可用的目录角色，请发送具有此目录角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) ID 的 POST 请求。</span><span class="sxs-lookup"><span data-stu-id="5f915-111">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="5f915-112">[列出目录角色模板](../api/directoryroletemplate-list.md)，以获取其他所有可用目录角色。</span><span class="sxs-lookup"><span data-stu-id="5f915-112">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="5f915-113">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="5f915-113">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="5f915-114">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="5f915-114">This resource supports:</span></span>

- <span data-ttu-id="5f915-115">通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="5f915-115">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="5f915-116">方法</span><span class="sxs-lookup"><span data-stu-id="5f915-116">Methods</span></span>

| <span data-ttu-id="5f915-117">方法</span><span class="sxs-lookup"><span data-stu-id="5f915-117">Method</span></span>       | <span data-ttu-id="5f915-118">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f915-118">Return Type</span></span>  |<span data-ttu-id="5f915-119">说明</span><span class="sxs-lookup"><span data-stu-id="5f915-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5f915-120">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="5f915-120">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="5f915-121">directoryRole</span><span class="sxs-lookup"><span data-stu-id="5f915-121">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="5f915-122">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f915-122">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="5f915-123">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="5f915-123">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="5f915-124">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f915-124">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="5f915-125">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="5f915-125">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="5f915-126">添加成员</span><span class="sxs-lookup"><span data-stu-id="5f915-126">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="5f915-127">directoryObject</span><span class="sxs-lookup"><span data-stu-id="5f915-127">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="5f915-128">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="5f915-128">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="5f915-129">列出成员</span><span class="sxs-lookup"><span data-stu-id="5f915-129">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="5f915-130">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f915-130">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="5f915-131">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="5f915-131">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="5f915-132">删除成员</span><span class="sxs-lookup"><span data-stu-id="5f915-132">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="5f915-133">directoryObject</span><span class="sxs-lookup"><span data-stu-id="5f915-133">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="5f915-134">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="5f915-134">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="5f915-135">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="5f915-135">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="5f915-136">directoryRole</span><span class="sxs-lookup"><span data-stu-id="5f915-136">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="5f915-137">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="5f915-137">Activate a directory role.</span></span>|
|[<span data-ttu-id="5f915-138">delta</span><span class="sxs-lookup"><span data-stu-id="5f915-138">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="5f915-139">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="5f915-139">directoryRole collection</span></span>| <span data-ttu-id="5f915-140">获取目录角色的增量更改。</span><span class="sxs-lookup"><span data-stu-id="5f915-140">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="5f915-141">属性</span><span class="sxs-lookup"><span data-stu-id="5f915-141">Properties</span></span>
| <span data-ttu-id="5f915-142">属性</span><span class="sxs-lookup"><span data-stu-id="5f915-142">Property</span></span>   | <span data-ttu-id="5f915-143">类型</span><span class="sxs-lookup"><span data-stu-id="5f915-143">Type</span></span> | <span data-ttu-id="5f915-144">说明</span><span class="sxs-lookup"><span data-stu-id="5f915-144">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5f915-145">说明</span><span class="sxs-lookup"><span data-stu-id="5f915-145">description</span></span>|<span data-ttu-id="5f915-146">String</span><span class="sxs-lookup"><span data-stu-id="5f915-146">String</span></span>|<span data-ttu-id="5f915-p103">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="5f915-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="5f915-149">displayName</span><span class="sxs-lookup"><span data-stu-id="5f915-149">displayName</span></span>|<span data-ttu-id="5f915-150">String</span><span class="sxs-lookup"><span data-stu-id="5f915-150">String</span></span>|<span data-ttu-id="5f915-p104">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="5f915-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="5f915-153">id</span><span class="sxs-lookup"><span data-stu-id="5f915-153">id</span></span>|<span data-ttu-id="5f915-154">String</span><span class="sxs-lookup"><span data-stu-id="5f915-154">String</span></span>|<span data-ttu-id="5f915-p105">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="5f915-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="5f915-158">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="5f915-158">roleTemplateId</span></span>|<span data-ttu-id="5f915-159">String</span><span class="sxs-lookup"><span data-stu-id="5f915-159">String</span></span>| <span data-ttu-id="5f915-p106">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="5f915-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5f915-163">关系</span><span class="sxs-lookup"><span data-stu-id="5f915-163">Relationships</span></span>
| <span data-ttu-id="5f915-164">关系</span><span class="sxs-lookup"><span data-stu-id="5f915-164">Relationship</span></span> | <span data-ttu-id="5f915-165">类型</span><span class="sxs-lookup"><span data-stu-id="5f915-165">Type</span></span> |<span data-ttu-id="5f915-166">说明</span><span class="sxs-lookup"><span data-stu-id="5f915-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f915-167">成员</span><span class="sxs-lookup"><span data-stu-id="5f915-167">members</span></span>|<span data-ttu-id="5f915-168">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f915-168">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="5f915-p107">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5f915-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f915-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f915-173">JSON representation</span></span>

<span data-ttu-id="5f915-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f915-174">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "memberOf",
    "members",
    "ownedObjects",
    "owners"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRole",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
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
