---
title: rbacApplication 资源类型
description: 角色管理导航属性
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: afcef3766e4df80a3856ab59684ba826c3a78d14
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437823"
---
# <a name="rbacapplication-resource-type"></a><span data-ttu-id="48fb3-103">rbacApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="48fb3-103">rbacApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48fb3-104">适用于 Microsoft 365 RBAC 提供程序的统一角色定义和角色分配的角色管理容器。</span><span class="sxs-lookup"><span data-stu-id="48fb3-104">Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers.</span></span> <span data-ttu-id="48fb3-105">当前 "目录" 是唯一受支持的 RBAC 应用程序。</span><span class="sxs-lookup"><span data-stu-id="48fb3-105">Currently "directory" is the only RBAC application supported.</span></span>

## <a name="methods"></a><span data-ttu-id="48fb3-106">方法</span><span class="sxs-lookup"><span data-stu-id="48fb3-106">Methods</span></span>

| <span data-ttu-id="48fb3-107">方法</span><span class="sxs-lookup"><span data-stu-id="48fb3-107">Method</span></span>       | <span data-ttu-id="48fb3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="48fb3-108">Return Type</span></span> | <span data-ttu-id="48fb3-109">说明</span><span class="sxs-lookup"><span data-stu-id="48fb3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="48fb3-110">创建 unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="48fb3-110">Create unifiedRoleAssignment</span></span>](../api/rbacapplication-post-roleassignments.md) | [<span data-ttu-id="48fb3-111">unifiedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="48fb3-111">unifiedRoleAssignment</span></span>](unifiedroleassignment.md) | <span data-ttu-id="48fb3-112">通过发布到 roleAssignments 集合创建新的 unifiedRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="48fb3-112">Create a new unifiedRoleAssignment by posting to the roleAssignments collection.</span></span> |
| [<span data-ttu-id="48fb3-113">List roleAssignments</span><span class="sxs-lookup"><span data-stu-id="48fb3-113">List roleAssignments</span></span>](../api/rbacapplication-list-roleassignments.md) | <span data-ttu-id="48fb3-114">[unifiedRoleAssignment](unifiedroleassignment.md)集合</span><span class="sxs-lookup"><span data-stu-id="48fb3-114">[unifiedRoleAssignment](unifiedroleassignment.md) collection</span></span> | <span data-ttu-id="48fb3-115">获取 unifiedRoleAssignment 对象集合。</span><span class="sxs-lookup"><span data-stu-id="48fb3-115">Get a unifiedRoleAssignment object collection.</span></span> <span data-ttu-id="48fb3-116">通过在 unifiedRoleDefitionId 或 principalId 上进行筛选, 只能查询特定的实例。</span><span class="sxs-lookup"><span data-stu-id="48fb3-116">Only specific instances can be queried, by filtering on unifiedRoleDefitionId or principalId.</span></span> |
| [<span data-ttu-id="48fb3-117">创建 unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="48fb3-117">Create unifiedRoleDefinition</span></span>](../api/rbacapplication-post-roledefinitions.md) | [<span data-ttu-id="48fb3-118">unifiedRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="48fb3-118">unifiedRoleDefinition</span></span>](unifiedroledefinition.md) | <span data-ttu-id="48fb3-119">通过发布到 roleDefinitions 集合创建新的 unifiedRoleDefinition。</span><span class="sxs-lookup"><span data-stu-id="48fb3-119">Create a new unifiedRoleDefinition by posting to the roleDefinitions collection.</span></span> |
| [<span data-ttu-id="48fb3-120">List roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="48fb3-120">List roleDefinitions</span></span>](../api/rbacapplication-list-roledefinitions.md) | <span data-ttu-id="48fb3-121">[unifiedRoleDefinition](unifiedroledefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="48fb3-121">[unifiedRoleDefinition](unifiedroledefinition.md) collection</span></span> | <span data-ttu-id="48fb3-122">获取 unifiedRoleDefinition 对象集合。</span><span class="sxs-lookup"><span data-stu-id="48fb3-122">Get a unifiedRoleDefinition object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="48fb3-123">属性</span><span class="sxs-lookup"><span data-stu-id="48fb3-123">Properties</span></span>

<span data-ttu-id="48fb3-124">无</span><span class="sxs-lookup"><span data-stu-id="48fb3-124">None</span></span>

## <a name="relationships"></a><span data-ttu-id="48fb3-125">关系</span><span class="sxs-lookup"><span data-stu-id="48fb3-125">Relationships</span></span>

<span data-ttu-id="48fb3-126">无</span><span class="sxs-lookup"><span data-stu-id="48fb3-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="48fb3-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="48fb3-127">JSON representation</span></span>

<span data-ttu-id="48fb3-128">无</span><span class="sxs-lookup"><span data-stu-id="48fb3-128">None</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
