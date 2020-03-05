---
title: unifiedRoleAssignment 资源类型
description: 角色分配是角色定义和特定作用域的主体之间的链接，目的是为了授予访问权限。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c51c3cd7c706cf154db8c1de21c04aaa098c3efb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519615"
---
# <a name="unifiedroleassignment-resource-type"></a><span data-ttu-id="75d5b-103">unifiedRoleAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="75d5b-103">unifiedRoleAssignment resource type</span></span>

<span data-ttu-id="75d5b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="75d5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75d5b-105">UnifiedRoleAssignment 用于授予对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="75d5b-105">A unifiedRoleAssignment is used to grant access to resources.</span></span> <span data-ttu-id="75d5b-106">它表示分配给特定范围内的主体（通常为用户）的角色定义。</span><span class="sxs-lookup"><span data-stu-id="75d5b-106">It represents a role definition assigned to a principal (typically a user) at a particular scope.</span></span>

## <a name="methods"></a><span data-ttu-id="75d5b-107">方法</span><span class="sxs-lookup"><span data-stu-id="75d5b-107">Methods</span></span>

| <span data-ttu-id="75d5b-108">方法</span><span class="sxs-lookup"><span data-stu-id="75d5b-108">Method</span></span>       | <span data-ttu-id="75d5b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="75d5b-109">Return Type</span></span> | <span data-ttu-id="75d5b-110">说明</span><span class="sxs-lookup"><span data-stu-id="75d5b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="75d5b-111">获取 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75d5b-111">Get unifiedRoleAssignment</span></span>](../api/unifiedroleassignment-get.md) | [<span data-ttu-id="75d5b-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75d5b-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="75d5b-113">读取 unifiedRoleAssignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="75d5b-113">Read properties and relationships of unifiedRoleAssignment object.</span></span> |
| [<span data-ttu-id="75d5b-114">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75d5b-114">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="75d5b-115">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="75d5b-115">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="75d5b-116">通过发布到 roleAssignment 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="75d5b-116">Create a new unifiedRoleAssignment by posting to the roleAssignment collection.</span></span> |
| [<span data-ttu-id="75d5b-117">删除</span><span class="sxs-lookup"><span data-stu-id="75d5b-117">Delete</span></span>](../api/unifiedroleassignment-delete.md) | <span data-ttu-id="75d5b-118">无</span><span class="sxs-lookup"><span data-stu-id="75d5b-118">None</span></span> | <span data-ttu-id="75d5b-119">删除 unifiedRoleAssignment 对象。</span><span class="sxs-lookup"><span data-stu-id="75d5b-119">Delete unifiedRoleAssignment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="75d5b-120">属性</span><span class="sxs-lookup"><span data-stu-id="75d5b-120">Properties</span></span>

| <span data-ttu-id="75d5b-121">属性</span><span class="sxs-lookup"><span data-stu-id="75d5b-121">Property</span></span>     | <span data-ttu-id="75d5b-122">类型</span><span class="sxs-lookup"><span data-stu-id="75d5b-122">Type</span></span>        | <span data-ttu-id="75d5b-123">说明</span><span class="sxs-lookup"><span data-stu-id="75d5b-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="75d5b-124">id</span><span class="sxs-lookup"><span data-stu-id="75d5b-124">id</span></span>|<span data-ttu-id="75d5b-125">String</span><span class="sxs-lookup"><span data-stu-id="75d5b-125">String</span></span>| <span data-ttu-id="75d5b-126">UnifiedRoleAssignment 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="75d5b-126">The unique identifier for the unifiedRoleAssignment.</span></span> <span data-ttu-id="75d5b-127">键，不可为 null，只读。</span><span class="sxs-lookup"><span data-stu-id="75d5b-127">Key, not nullable, Read-only.</span></span> |
|<span data-ttu-id="75d5b-128">principalId</span><span class="sxs-lookup"><span data-stu-id="75d5b-128">principalId</span></span>|<span data-ttu-id="75d5b-129">String</span><span class="sxs-lookup"><span data-stu-id="75d5b-129">String</span></span>| <span data-ttu-id="75d5b-130">向其授予分配的主体的 Objectid。</span><span class="sxs-lookup"><span data-stu-id="75d5b-130">Objectid of the principal to which the assignment is granted.</span></span> |
|<span data-ttu-id="75d5b-131">resourceScope</span><span class="sxs-lookup"><span data-stu-id="75d5b-131">resourceScope</span></span>|<span data-ttu-id="75d5b-132">String</span><span class="sxs-lookup"><span data-stu-id="75d5b-132">String</span></span>| <span data-ttu-id="75d5b-133">应用 unifiedRoleAssignment 的范围。</span><span class="sxs-lookup"><span data-stu-id="75d5b-133">The scope at which the unifiedRoleAssignment applies.</span></span> <span data-ttu-id="75d5b-134">对于服务范围，这是 "/"。</span><span class="sxs-lookup"><span data-stu-id="75d5b-134">This is "/" for service-wide.</span></span> |
|<span data-ttu-id="75d5b-135">roleDefinitionId</span><span class="sxs-lookup"><span data-stu-id="75d5b-135">roleDefinitionId</span></span>|<span data-ttu-id="75d5b-136">String</span><span class="sxs-lookup"><span data-stu-id="75d5b-136">String</span></span>| <span data-ttu-id="75d5b-137">工作分配的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="75d5b-137">The unifiedRoleDefinition the assignment is for.</span></span> <span data-ttu-id="75d5b-138">只读。</span><span class="sxs-lookup"><span data-stu-id="75d5b-138">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="75d5b-139">关系</span><span class="sxs-lookup"><span data-stu-id="75d5b-139">Relationships</span></span>

<span data-ttu-id="75d5b-140">无</span><span class="sxs-lookup"><span data-stu-id="75d5b-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75d5b-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="75d5b-141">JSON representation</span></span>

<span data-ttu-id="75d5b-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="75d5b-142">The following is a JSON representation of the resource.</span></span>

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
