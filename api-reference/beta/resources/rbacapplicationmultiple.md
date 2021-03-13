---
title: rbacApplicationMultiple 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ba6c4973dd79f328c1d04ea26803a6b2aec39c7f
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760916"
---
# <a name="rbacapplicationmultiple-resource-type"></a><span data-ttu-id="24d84-103">rbacApplicationMultiple 资源类型</span><span class="sxs-lookup"><span data-stu-id="24d84-103">rbacApplicationMultiple resource type</span></span>

<span data-ttu-id="24d84-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24d84-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24d84-105">用于统一角色定义的角色管理容器，以及支持单个作用域中的多个主体和多个作用域的 Microsoft 365 RBAC 提供程序角色分配。</span><span class="sxs-lookup"><span data-stu-id="24d84-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="24d84-106">这不同于 [rbacApplication](rbacapplication.md) 资源类型。</span><span class="sxs-lookup"><span data-stu-id="24d84-106">This is different from [rbacApplication](rbacapplication.md) resource type.</span></span> <span data-ttu-id="24d84-107">Microsoft Intune 是此类 RBAC 提供程序的一个示例。</span><span class="sxs-lookup"><span data-stu-id="24d84-107">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="24d84-108">Intune 角色分配可以有一个主体数组和一组作用域组。</span><span class="sxs-lookup"><span data-stu-id="24d84-108">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span>

## <a name="methods"></a><span data-ttu-id="24d84-109">方法</span><span class="sxs-lookup"><span data-stu-id="24d84-109">Methods</span></span>

| <span data-ttu-id="24d84-110">方法</span><span class="sxs-lookup"><span data-stu-id="24d84-110">Method</span></span>       | <span data-ttu-id="24d84-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="24d84-111">Return Type</span></span> | <span data-ttu-id="24d84-112">说明</span><span class="sxs-lookup"><span data-stu-id="24d84-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="24d84-113">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="24d84-113">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="24d84-114">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="24d84-114">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="24d84-115">通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignmentMultiple。</span><span class="sxs-lookup"><span data-stu-id="24d84-115">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="24d84-116">列出 roleAssignmentsMultiple</span><span class="sxs-lookup"><span data-stu-id="24d84-116">List roleAssignmentsMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | <span data-ttu-id="24d84-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24d84-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) collection</span></span> | <span data-ttu-id="24d84-118">获取 unifiedRoleAssignmentMultiple 对象集合。</span><span class="sxs-lookup"><span data-stu-id="24d84-118">Get unifiedRoleAssignmentMultiple object collection.</span></span> |
| [<span data-ttu-id="24d84-119">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="24d84-119">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="24d84-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="24d84-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="24d84-121">通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="24d84-121">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="24d84-122">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="24d84-122">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="24d84-123">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24d84-123">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="24d84-124">获取 unifiedRoleDefinition 对象集合。</span><span class="sxs-lookup"><span data-stu-id="24d84-124">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="24d84-125">属性</span><span class="sxs-lookup"><span data-stu-id="24d84-125">Properties</span></span>

<span data-ttu-id="24d84-126">无</span><span class="sxs-lookup"><span data-stu-id="24d84-126">None</span></span>

## <a name="relationships"></a><span data-ttu-id="24d84-127">关系</span><span class="sxs-lookup"><span data-stu-id="24d84-127">Relationships</span></span>

<span data-ttu-id="24d84-128">无</span><span class="sxs-lookup"><span data-stu-id="24d84-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24d84-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24d84-129">JSON representation</span></span>

<span data-ttu-id="24d84-130">无</span><span class="sxs-lookup"><span data-stu-id="24d84-130">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


