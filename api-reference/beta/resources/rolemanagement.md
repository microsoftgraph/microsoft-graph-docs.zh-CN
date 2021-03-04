---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 241de0b72a9ffad507975fca408fe49f0b0a90f0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440122"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="9d704-103">roleManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d704-103">roleManagement resource type</span></span>

<span data-ttu-id="9d704-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d704-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d704-105">代表 Microsoft 365 RBAC 角色管理实体。</span><span class="sxs-lookup"><span data-stu-id="9d704-105">Represents a Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="9d704-106">提供对 RBAC 提供程序中出现的角色定义和角色分配的访问权限。</span><span class="sxs-lookup"><span data-stu-id="9d704-106">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="9d704-107">目前， (支持 Azure AD) 和 deviceManagement (Intune) 目录。</span><span class="sxs-lookup"><span data-stu-id="9d704-107">Currently directory (Azure AD) and  deviceManagement (Intune) providers are supported.</span></span> 

<span data-ttu-id="9d704-108">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="9d704-108">For more information, see:</span></span> 
* <span data-ttu-id="9d704-109">[Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="9d704-109">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* [<span data-ttu-id="9d704-110">使用 Microsoft Intune (基于角色) RBAC</span><span class="sxs-lookup"><span data-stu-id="9d704-110">Role-based access control (RBAC) with Microsoft Intune</span></span>](/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a><span data-ttu-id="9d704-111">Methods</span><span class="sxs-lookup"><span data-stu-id="9d704-111">Methods</span></span>

<span data-ttu-id="9d704-112">无。</span><span class="sxs-lookup"><span data-stu-id="9d704-112">None.</span></span>

## <a name="properties"></a><span data-ttu-id="9d704-113">属性</span><span class="sxs-lookup"><span data-stu-id="9d704-113">Properties</span></span>

<span data-ttu-id="9d704-114">无。</span><span class="sxs-lookup"><span data-stu-id="9d704-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="9d704-115">关系</span><span class="sxs-lookup"><span data-stu-id="9d704-115">Relationships</span></span>

| <span data-ttu-id="9d704-116">关系</span><span class="sxs-lookup"><span data-stu-id="9d704-116">Relationship</span></span> | <span data-ttu-id="9d704-117">类型</span><span class="sxs-lookup"><span data-stu-id="9d704-117">Type</span></span>        | <span data-ttu-id="9d704-118">说明</span><span class="sxs-lookup"><span data-stu-id="9d704-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9d704-119">目录</span><span class="sxs-lookup"><span data-stu-id="9d704-119">directory</span></span>|[<span data-ttu-id="9d704-120">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="9d704-120">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="9d704-121">只读。</span><span class="sxs-lookup"><span data-stu-id="9d704-121">Read-only.</span></span> <span data-ttu-id="9d704-122">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9d704-122">Nullable.</span></span>|
|<span data-ttu-id="9d704-123">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="9d704-123">deviceManagement</span></span>|[<span data-ttu-id="9d704-124">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="9d704-124">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="9d704-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="9d704-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d704-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d704-127">JSON representation</span></span>

<span data-ttu-id="9d704-128">无。</span><span class="sxs-lookup"><span data-stu-id="9d704-128">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
