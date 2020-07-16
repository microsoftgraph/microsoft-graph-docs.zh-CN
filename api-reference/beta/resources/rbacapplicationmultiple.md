---
title: rbacApplicationMultiple 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e7f44133050a616cac190aee5c7eeac9904f8715
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44990265"
---
# <a name="rbacapplicationmultiple-resource-type"></a><span data-ttu-id="8f36d-103">rbacApplicationMultiple 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f36d-103">rbacApplicationMultiple resource type</span></span>

<span data-ttu-id="8f36d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f36d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8f36d-105">用于在单个角色分配中支持多个主体和多个作用域的 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。</span><span class="sxs-lookup"><span data-stu-id="8f36d-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="8f36d-106">这不同于[rbacApplication](rbacapplication.md)资源类型。</span><span class="sxs-lookup"><span data-stu-id="8f36d-106">This is different from [rbacApplication](rbacapplication.md) resource type.</span></span> <span data-ttu-id="8f36d-107">Microsoft Intune 是此类 RBAC 提供程序的一个示例。</span><span class="sxs-lookup"><span data-stu-id="8f36d-107">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="8f36d-108">Intune 中的角色分配可以具有主体阵列和作用域组的阵列。</span><span class="sxs-lookup"><span data-stu-id="8f36d-108">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span>

## <a name="methods"></a><span data-ttu-id="8f36d-109">方法</span><span class="sxs-lookup"><span data-stu-id="8f36d-109">Methods</span></span>

| <span data-ttu-id="8f36d-110">方法</span><span class="sxs-lookup"><span data-stu-id="8f36d-110">Method</span></span>       | <span data-ttu-id="8f36d-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="8f36d-111">Return Type</span></span> | <span data-ttu-id="8f36d-112">说明</span><span class="sxs-lookup"><span data-stu-id="8f36d-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="8f36d-113">创建 unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="8f36d-113">Create unifiedRoleAssignmentMultiple</span></span>](../api/unifiedroleassignmentmultiple-post.md) | [<span data-ttu-id="8f36d-114">unifiedRoleAssignmentMultiple</span><span class="sxs-lookup"><span data-stu-id="8f36d-114">unifiedRoleAssignmentMultiple</span></span>](unifiedroleassignmentmultiple.md) | <span data-ttu-id="8f36d-115">通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignmentMultiple。</span><span class="sxs-lookup"><span data-stu-id="8f36d-115">Create a new unifiedRoleAssignmentMultiple by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="8f36d-116">列出 roleAssignmentsMultiple</span><span class="sxs-lookup"><span data-stu-id="8f36d-116">List roleAssignmentsMultiple</span></span>](../api/unifiedroleassignmentmultiple-list.md) | <span data-ttu-id="8f36d-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f36d-117">[unifiedRoleAssignmentMultiple](unifiedroleassignmentmultiple.md) collection</span></span> | <span data-ttu-id="8f36d-118">获取 unifiedRoleAssignmentMultiple 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8f36d-118">Get unifiedRoleAssignmentMultiple object collection.</span></span> |
| [<span data-ttu-id="8f36d-119">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8f36d-119">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="8f36d-120">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="8f36d-120">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="8f36d-121">通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="8f36d-121">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="8f36d-122">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="8f36d-122">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="8f36d-123">[unifiedRoleDefinition](unifiedroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f36d-123">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="8f36d-124">获取 unifiedRoleDefinition 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8f36d-124">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="8f36d-125">属性</span><span class="sxs-lookup"><span data-stu-id="8f36d-125">Properties</span></span>

<span data-ttu-id="8f36d-126">无</span><span class="sxs-lookup"><span data-stu-id="8f36d-126">None</span></span>

## <a name="relationships"></a><span data-ttu-id="8f36d-127">关系</span><span class="sxs-lookup"><span data-stu-id="8f36d-127">Relationships</span></span>

<span data-ttu-id="8f36d-128">无</span><span class="sxs-lookup"><span data-stu-id="8f36d-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f36d-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f36d-129">JSON representation</span></span>

<span data-ttu-id="8f36d-130">无</span><span class="sxs-lookup"><span data-stu-id="8f36d-130">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplicationMultiple resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
