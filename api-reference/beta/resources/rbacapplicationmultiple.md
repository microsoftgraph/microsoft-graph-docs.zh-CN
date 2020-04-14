---
title: rbacApplicationMultiple 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6450852f63b08b6413681579e77850488106e3c4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462225"
---
# <a name="rbacapplicationmultiple-resource-type"></a><span data-ttu-id="990ac-103">rbacApplicationMultiple 资源类型</span><span class="sxs-lookup"><span data-stu-id="990ac-103">rbacApplicationMultiple resource type</span></span>

<span data-ttu-id="990ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="990ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="990ac-105">用于在单个角色分配中支持多个主体和多个作用域的 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。</span><span class="sxs-lookup"><span data-stu-id="990ac-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="990ac-106">这不同于[rbacApplication](rbacapplication.md)资源类型。</span><span class="sxs-lookup"><span data-stu-id="990ac-106">This is different from [rbacApplication](rbacapplication.md) resource type.</span></span> <span data-ttu-id="990ac-107">Microsoft Intune 是此类 RBAC 提供程序的一个示例。</span><span class="sxs-lookup"><span data-stu-id="990ac-107">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="990ac-108">Intune 中的角色分配可以具有主体阵列和作用域组的阵列。</span><span class="sxs-lookup"><span data-stu-id="990ac-108">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span>

## <a name="methods"></a><span data-ttu-id="990ac-109">方法</span><span class="sxs-lookup"><span data-stu-id="990ac-109">Methods</span></span>

| <span data-ttu-id="990ac-110">方法</span><span class="sxs-lookup"><span data-stu-id="990ac-110">Method</span></span>       | <span data-ttu-id="990ac-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="990ac-111">Return Type</span></span> | <span data-ttu-id="990ac-112">说明</span><span class="sxs-lookup"><span data-stu-id="990ac-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="990ac-113">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="990ac-113">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="990ac-114">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="990ac-114">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="990ac-115">通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignmentMultiple。</span><span class="sxs-lookup"><span data-stu-id="990ac-115">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="990ac-116">列出 roleAssignmentsMultiple</span><span class="sxs-lookup"><span data-stu-id="990ac-116">List roleAssignmentsMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | <span data-ttu-id="990ac-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md)集合</span><span class="sxs-lookup"><span data-stu-id="990ac-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) collection</span></span> | <span data-ttu-id="990ac-118">获取 unifiedRoleAssignmentMultiple 对象集合。</span><span class="sxs-lookup"><span data-stu-id="990ac-118">Get unifiedRoleAssignmentMultiple object collection.</span></span> <span data-ttu-id="990ac-119">通过在 unifiedRoleDefitionId 或 principalId 上进行筛选，只能查询特定的实例。</span><span class="sxs-lookup"><span data-stu-id="990ac-119">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="990ac-120">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="990ac-120">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="990ac-121">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="990ac-121">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="990ac-122">通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="990ac-122">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="990ac-123">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="990ac-123">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="990ac-124">[unifiedRoleDefinition](unifiedroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="990ac-124">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="990ac-125">获取 unifiedRoleDefinition 对象集合。</span><span class="sxs-lookup"><span data-stu-id="990ac-125">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="990ac-126">属性</span><span class="sxs-lookup"><span data-stu-id="990ac-126">Properties</span></span>

<span data-ttu-id="990ac-127">无</span><span class="sxs-lookup"><span data-stu-id="990ac-127">None</span></span>

## <a name="relationships"></a><span data-ttu-id="990ac-128">关系</span><span class="sxs-lookup"><span data-stu-id="990ac-128">Relationships</span></span>

<span data-ttu-id="990ac-129">无</span><span class="sxs-lookup"><span data-stu-id="990ac-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="990ac-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="990ac-130">JSON representation</span></span>

<span data-ttu-id="990ac-131">无</span><span class="sxs-lookup"><span data-stu-id="990ac-131">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->