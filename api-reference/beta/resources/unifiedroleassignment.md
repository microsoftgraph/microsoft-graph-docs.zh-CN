---
title: unifiedRoleAssignment 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接, 目的是为了授予访问权限。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cfc0c00add243b98c852a00f0a4ab990c3ca5173
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437788"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="105e1-103">unifiedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="105e1-103">unifiedRoleAssignment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="105e1-104">UnifiedRoleAssignment 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="105e1-104">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="105e1-105">它表示分配给特定范围内的主体 (通常为用户) 的角色定义。</span><span class="sxs-lookup"><span data-stu-id="105e1-105">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

## <a name="methods"></a><span data-ttu-id="105e1-106">方法</span><span class="sxs-lookup"><span data-stu-id="105e1-106">Methods</span></span>

| <span data-ttu-id="105e1-107">方法</span><span class="sxs-lookup"><span data-stu-id="105e1-107">Method</span></span>       | <span data-ttu-id="105e1-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="105e1-108">Return Type</span></span> | <span data-ttu-id="105e1-109">说明</span><span class="sxs-lookup"><span data-stu-id="105e1-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="105e1-110">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="105e1-110">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="105e1-111">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="105e1-111">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="105e1-112">读取 unifiedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="105e1-112">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="105e1-113">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="105e1-113">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="105e1-114">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="105e1-114">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="105e1-115">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="105e1-115">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="105e1-116">删除</span><span class="sxs-lookup"><span data-stu-id="105e1-116">Delete</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="105e1-117">无</span><span class="sxs-lookup"><span data-stu-id="105e1-117">None</span></span> | <span data-ttu-id="105e1-118">删除 unifiedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="105e1-118">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="105e1-119">属性</span><span class="sxs-lookup"><span data-stu-id="105e1-119">Properties</span></span>

| <span data-ttu-id="105e1-120">属性</span><span class="sxs-lookup"><span data-stu-id="105e1-120">Property</span></span>     | <span data-ttu-id="105e1-121">类型</span><span class="sxs-lookup"><span data-stu-id="105e1-121">Type</span></span>        | <span data-ttu-id="105e1-122">说明</span><span class="sxs-lookup"><span data-stu-id="105e1-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="105e1-123">id</span><span class="sxs-lookup"><span data-stu-id="105e1-123">id</span></span>|<span data-ttu-id="105e1-124">String</span><span class="sxs-lookup"><span data-stu-id="105e1-124">String</span></span>| <span data-ttu-id="105e1-125">UnifiedRoleAssignment 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="105e1-125">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="105e1-126">键, 不可为 null, 只读。</span><span class="sxs-lookup"><span data-stu-id="105e1-126">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="105e1-127">principalId</span><span class="sxs-lookup"><span data-stu-id="105e1-127">principalId</span></span>|<span data-ttu-id="105e1-128">String</span><span class="sxs-lookup"><span data-stu-id="105e1-128">String</span></span>| <span data-ttu-id="105e1-129">向其授予分配的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="105e1-129">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="105e1-130">resourceScope</span><span class="sxs-lookup"><span data-stu-id="105e1-130">resourceScope</span></span>|<span data-ttu-id="105e1-131">String</span><span class="sxs-lookup"><span data-stu-id="105e1-131">String</span></span>| <span data-ttu-id="105e1-132">应用 unifiedRoleAssignment 的范围。</span><span class="sxs-lookup"><span data-stu-id="105e1-132">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="105e1-133">对于服务范围, 这是 "/"。</span><span class="sxs-lookup"><span data-stu-id="105e1-133">This is "/" for service-wide.</span></span> |
|<span data-ttu-id="105e1-134">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="105e1-134">roleDefinitionId</span></span>|<span data-ttu-id="105e1-135">String</span><span class="sxs-lookup"><span data-stu-id="105e1-135">String</span></span>| <span data-ttu-id="105e1-136">工作分配的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="105e1-136">The unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="105e1-137">只读。</span><span class="sxs-lookup"><span data-stu-id="105e1-137">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="105e1-138">关系</span><span class="sxs-lookup"><span data-stu-id="105e1-138">Relationships</span></span>

<span data-ttu-id="105e1-139">无</span><span class="sxs-lookup"><span data-stu-id="105e1-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="105e1-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="105e1-140">JSON representation</span></span>

<span data-ttu-id="105e1-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="105e1-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "principalId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "unifiedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
