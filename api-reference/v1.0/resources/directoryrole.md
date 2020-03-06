---
title: directoryRole 资源类型
description: 表示 Azure AD Directory 角色。 Azure AD 目录角色也称作*管理员角色*。
localization_priority: Priority
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0b4ba56eafd3ff8ac0e8902019816cb4b752761f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531637"
---
# <a name="directoryrole-resource-type"></a><span data-ttu-id="f973b-104">directoryRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="f973b-104">directoryRole resource type</span></span>

<span data-ttu-id="f973b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f973b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f973b-106">表示 Azure AD Directory 角色。</span><span class="sxs-lookup"><span data-stu-id="f973b-106">Represents an Azure AD directory role.</span></span> <span data-ttu-id="f973b-107">Azure AD 目录角色也称作*管理员角色*。</span><span class="sxs-lookup"><span data-stu-id="f973b-107">Azure AD directory roles are also known as *administrator roles*.</span></span> <span data-ttu-id="f973b-108">有关这些目录（管理员）角色的详细信息，请参阅 [在 Azure AD 中分配管理员角色](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/)</span><span class="sxs-lookup"><span data-stu-id="f973b-108">For more information about directory (administrator) roles, see [Assigning administrator roles in Azure AD](http://azure.microsoft.com/documentation/articles/active-directory-assign-admin-roles/).</span></span> <span data-ttu-id="f973b-109">使用 Microsoft Graph，可以将用户分配给目录角色，使其具有目标角色的权限。</span><span class="sxs-lookup"><span data-stu-id="f973b-109">With the Microsoft Graph, you can assign users to directory roles to grant them the permissions of the target role.</span></span> <span data-ttu-id="f973b-110">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="f973b-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="f973b-111">默认情况下，仅激活公司管理员目录角色。</span><span class="sxs-lookup"><span data-stu-id="f973b-111">Only the Company Administrators directory role is activated by default.</span></span> <span data-ttu-id="f973b-112">若要激活其他可用的目录角色，请发送具有此目录角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) ID 的 POST 请求。</span><span class="sxs-lookup"><span data-stu-id="f973b-112">To activate other available directory roles you send a POST request with the ID of the [directoryRoleTemplate](directoryroletemplate.md) on which the directory role is based.</span></span> <span data-ttu-id="f973b-113">[列出目录角色模板](../api/directoryroletemplate-list.md)，以获取其他所有可用目录角色。</span><span class="sxs-lookup"><span data-stu-id="f973b-113">[List directory role templates](../api/directoryroletemplate-list.md) to get all the other available directory roles.</span></span> <span data-ttu-id="f973b-114">继承自 [directoryObject](directoryobject.md)。</span><span class="sxs-lookup"><span data-stu-id="f973b-114">Inherits from [directoryObject](directoryobject.md).</span></span>

<span data-ttu-id="f973b-115">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="f973b-115">This resource supports:</span></span>

- <span data-ttu-id="f973b-116">通过提供 [delta](../api/directoryrole-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="f973b-116">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/directoryrole-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="f973b-117">方法</span><span class="sxs-lookup"><span data-stu-id="f973b-117">Methods</span></span>

| <span data-ttu-id="f973b-118">方法</span><span class="sxs-lookup"><span data-stu-id="f973b-118">Method</span></span>       | <span data-ttu-id="f973b-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="f973b-119">Return Type</span></span>  |<span data-ttu-id="f973b-120">说明</span><span class="sxs-lookup"><span data-stu-id="f973b-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f973b-121">获取 directoryRole</span><span class="sxs-lookup"><span data-stu-id="f973b-121">Get directoryRole</span></span>](../api/directoryrole-get.md) | [<span data-ttu-id="f973b-122">directoryRole</span><span class="sxs-lookup"><span data-stu-id="f973b-122">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="f973b-123">读取 directoryRol 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f973b-123">Read properties and relationships of directoryRole object.</span></span> |
|[<span data-ttu-id="f973b-124">列出 directoryRoles</span><span class="sxs-lookup"><span data-stu-id="f973b-124">List directoryRoles</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="f973b-125">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f973b-125">[directoryRole](directoryrole.md) collection</span></span> | <span data-ttu-id="f973b-126">列出租户中激活的目录角色。</span><span class="sxs-lookup"><span data-stu-id="f973b-126">List the directory roles that are activated in the tenant.</span></span> |
|[<span data-ttu-id="f973b-127">添加成员</span><span class="sxs-lookup"><span data-stu-id="f973b-127">Add member</span></span>](../api/directoryrole-post-members.md) |[<span data-ttu-id="f973b-128">directoryObject</span><span class="sxs-lookup"><span data-stu-id="f973b-128">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="f973b-129">通过发布到成员导航属性将用户添加到目录角色。</span><span class="sxs-lookup"><span data-stu-id="f973b-129">Add a user to the directory role by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="f973b-130">列出成员</span><span class="sxs-lookup"><span data-stu-id="f973b-130">List members</span></span>](../api/directoryrole-list-members.md) |<span data-ttu-id="f973b-131">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f973b-131">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="f973b-132">从成员导航属性获取该目录角色成员的用户。</span><span class="sxs-lookup"><span data-stu-id="f973b-132">Get the users that are members of the directory role from the members navigation property.</span></span>|
|[<span data-ttu-id="f973b-133">删除成员</span><span class="sxs-lookup"><span data-stu-id="f973b-133">Remove a member</span></span>](../api/directoryrole-delete-member.md) |[<span data-ttu-id="f973b-134">directoryObject</span><span class="sxs-lookup"><span data-stu-id="f973b-134">directoryObject</span></span>](directoryobject.md)| <span data-ttu-id="f973b-135">删除目录角色中的用户。</span><span class="sxs-lookup"><span data-stu-id="f973b-135">Remove a user from the directory role.</span></span>|
|[<span data-ttu-id="f973b-136">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="f973b-136">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) |[<span data-ttu-id="f973b-137">directoryRole</span><span class="sxs-lookup"><span data-stu-id="f973b-137">directoryRole</span></span>](directoryrole.md) | <span data-ttu-id="f973b-138">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="f973b-138">Activate a directory role.</span></span>|
|[<span data-ttu-id="f973b-139">delta</span><span class="sxs-lookup"><span data-stu-id="f973b-139">delta</span></span>](../api/directoryrole-delta.md)|<span data-ttu-id="f973b-140">directoryRole 集合</span><span class="sxs-lookup"><span data-stu-id="f973b-140">directoryRole collection</span></span>| <span data-ttu-id="f973b-141">获取目录角色的增量更改。</span><span class="sxs-lookup"><span data-stu-id="f973b-141">Get incremental changes for directory roles.</span></span> |

## <a name="properties"></a><span data-ttu-id="f973b-142">属性</span><span class="sxs-lookup"><span data-stu-id="f973b-142">Properties</span></span>
| <span data-ttu-id="f973b-143">属性</span><span class="sxs-lookup"><span data-stu-id="f973b-143">Property</span></span>   | <span data-ttu-id="f973b-144">类型</span><span class="sxs-lookup"><span data-stu-id="f973b-144">Type</span></span> | <span data-ttu-id="f973b-145">说明</span><span class="sxs-lookup"><span data-stu-id="f973b-145">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f973b-146">说明</span><span class="sxs-lookup"><span data-stu-id="f973b-146">description</span></span>|<span data-ttu-id="f973b-147">String</span><span class="sxs-lookup"><span data-stu-id="f973b-147">String</span></span>|<span data-ttu-id="f973b-p103">目录角色说明。只读。</span><span class="sxs-lookup"><span data-stu-id="f973b-p103">The description for the directory role. Read-only.</span></span> |
|<span data-ttu-id="f973b-150">displayName</span><span class="sxs-lookup"><span data-stu-id="f973b-150">displayName</span></span>|<span data-ttu-id="f973b-151">String</span><span class="sxs-lookup"><span data-stu-id="f973b-151">String</span></span>|<span data-ttu-id="f973b-p104">目录角色的显示名称。只读。</span><span class="sxs-lookup"><span data-stu-id="f973b-p104">The display name for the directory role. Read-only.</span></span> |
|<span data-ttu-id="f973b-154">id</span><span class="sxs-lookup"><span data-stu-id="f973b-154">id</span></span>|<span data-ttu-id="f973b-155">String</span><span class="sxs-lookup"><span data-stu-id="f973b-155">String</span></span>|<span data-ttu-id="f973b-p105">目录角色唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL，只读。</span><span class="sxs-lookup"><span data-stu-id="f973b-p105">The unique identifier for the directory role. Inherited from [directoryObject](directoryobject.md). Key, Not nullable, Read-only.</span></span>|
|<span data-ttu-id="f973b-159">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="f973b-159">roleTemplateId</span></span>|<span data-ttu-id="f973b-160">String</span><span class="sxs-lookup"><span data-stu-id="f973b-160">String</span></span>| <span data-ttu-id="f973b-p106">此角色所基于的 [directoryRoleTemplate](directoryroletemplate.md) 的 **id**。使用 POST 操作在租户中激活目录角色时，必须指定其属性。激活目录角色后，其属性为只读。</span><span class="sxs-lookup"><span data-stu-id="f973b-p106">The **id** of the [directoryRoleTemplate](directoryroletemplate.md) that this role is based on. The property must be specified when activating a directory role in a tenant with a POST operation. After the directory role has been activated, the property is read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f973b-164">关系</span><span class="sxs-lookup"><span data-stu-id="f973b-164">Relationships</span></span>
| <span data-ttu-id="f973b-165">关系</span><span class="sxs-lookup"><span data-stu-id="f973b-165">Relationship</span></span> | <span data-ttu-id="f973b-166">类型</span><span class="sxs-lookup"><span data-stu-id="f973b-166">Type</span></span> |<span data-ttu-id="f973b-167">说明</span><span class="sxs-lookup"><span data-stu-id="f973b-167">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f973b-168">成员</span><span class="sxs-lookup"><span data-stu-id="f973b-168">members</span></span>|<span data-ttu-id="f973b-169">[directoryObject](directoryobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f973b-169">[directoryObject](directoryobject.md) collection</span></span>|<span data-ttu-id="f973b-p107">是此目录角色成员的用户。HTTP 方法：GET、POST、DELETE。只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="f973b-p107">Users that are members of this directory role. HTTP Methods: GET, POST, DELETE. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f973b-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f973b-174">JSON representation</span></span>

<span data-ttu-id="f973b-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f973b-175">Here is a JSON representation of the resource</span></span>

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
