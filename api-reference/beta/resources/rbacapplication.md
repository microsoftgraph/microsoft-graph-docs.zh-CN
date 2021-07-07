---
title: rbacApplication 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9636f113222bbbe6a754c2977e08273d140a6086
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317194"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="5f37b-103">rbacApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f37b-103">rbacApplication resource type</span></span>

<span data-ttu-id="5f37b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f37b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f37b-105">用于统一角色定义的角色管理容器和用于 RBAC Microsoft 365角色分配。</span><span class="sxs-lookup"><span data-stu-id="5f37b-105">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="5f37b-106">目前，目录和权利管理是唯一受支持的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="5f37b-106">Currently directory and entitlement management are the only RBAC applications supported.</span></span>

## <a name="methods"></a><span data-ttu-id="5f37b-107">Methods</span><span class="sxs-lookup"><span data-stu-id="5f37b-107">Methods</span></span>

| <span data-ttu-id="5f37b-108">方法</span><span class="sxs-lookup"><span data-stu-id="5f37b-108">Method</span></span>       | <span data-ttu-id="5f37b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5f37b-109">Return Type</span></span> | <span data-ttu-id="5f37b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5f37b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5f37b-111">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f37b-111">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="5f37b-112">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="5f37b-112">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="5f37b-113">通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="5f37b-113">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="5f37b-114">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="5f37b-114">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="5f37b-115">[unifiedRoleAssignment](unifiedroleassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f37b-115">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="5f37b-116">获取 unifiedRoleAssignment 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f37b-116">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="5f37b-117">通过筛选 roleDefitionId 或 principalId，只能查询特定实例。</span><span class="sxs-lookup"><span data-stu-id="5f37b-117">Only specific instances can be queried, by filtering on roleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="5f37b-118">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5f37b-118">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="5f37b-119">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="5f37b-119">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="5f37b-120">通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="5f37b-120">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="5f37b-121">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="5f37b-121">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="5f37b-122">[unifiedRoleDefinition](unifiedroledefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5f37b-122">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="5f37b-123">获取 unifiedRoleDefinition 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f37b-123">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="5f37b-124">属性</span><span class="sxs-lookup"><span data-stu-id="5f37b-124">Properties</span></span>

<span data-ttu-id="5f37b-125">无</span><span class="sxs-lookup"><span data-stu-id="5f37b-125">None</span></span>

## <a name="relationships"></a><span data-ttu-id="5f37b-126">关系</span><span class="sxs-lookup"><span data-stu-id="5f37b-126">Relationships</span></span>

<span data-ttu-id="5f37b-127">无</span><span class="sxs-lookup"><span data-stu-id="5f37b-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f37b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f37b-128">JSON representation</span></span>

<span data-ttu-id="5f37b-129">无</span><span class="sxs-lookup"><span data-stu-id="5f37b-129">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


