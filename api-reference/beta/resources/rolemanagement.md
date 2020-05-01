---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 71c59c1e44123b60dd46b2c72e71aabfc7a64c25
ms.sourcegitcommit: feebe30e62aa19ce5cb8e8338e043326e464ed9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991780"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="3ad3f-103">roleManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ad3f-103">roleManagement resource type</span></span>

<span data-ttu-id="3ad3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ad3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ad3f-105">表示 Microsoft 365 RBAC 角色管理实体。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-105">Represents a Microsoft 365 RBAC role management entity.</span></span> <span data-ttu-id="3ad3f-106">提供对在 RBAC 提供程序中呈现的角色定义和角色分配的访问权限。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-106">Provides access to role definitions and role assignments surfaced from RBAC providers.</span></span> <span data-ttu-id="3ad3f-107">支持当前目录（Azure AD）和 deviceManagement （Intune）提供程序。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-107">Currently directory (Azure AD) and  deviceManagement (Intune) providers are supported.</span></span> 

<span data-ttu-id="3ad3f-108">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="3ad3f-108">For more information, see:</span></span> 
* <span data-ttu-id="3ad3f-109">[Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-109">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* [<span data-ttu-id="3ad3f-110">使用 Microsoft Intune 的基于角色的访问控制（RBAC）</span><span class="sxs-lookup"><span data-stu-id="3ad3f-110">Role-based access control (RBAC) with Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/role-based-access-control)

## <a name="methods"></a><span data-ttu-id="3ad3f-111">方法</span><span class="sxs-lookup"><span data-stu-id="3ad3f-111">Methods</span></span>

<span data-ttu-id="3ad3f-112">无。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-112">None.</span></span>

## <a name="properties"></a><span data-ttu-id="3ad3f-113">属性</span><span class="sxs-lookup"><span data-stu-id="3ad3f-113">Properties</span></span>

<span data-ttu-id="3ad3f-114">无。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="3ad3f-115">关系</span><span class="sxs-lookup"><span data-stu-id="3ad3f-115">Relationships</span></span>

| <span data-ttu-id="3ad3f-116">关系</span><span class="sxs-lookup"><span data-stu-id="3ad3f-116">Relationship</span></span> | <span data-ttu-id="3ad3f-117">类型</span><span class="sxs-lookup"><span data-stu-id="3ad3f-117">Type</span></span>        | <span data-ttu-id="3ad3f-118">说明</span><span class="sxs-lookup"><span data-stu-id="3ad3f-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ad3f-119">文件夹</span><span class="sxs-lookup"><span data-stu-id="3ad3f-119">directory</span></span>|[<span data-ttu-id="3ad3f-120">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="3ad3f-120">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="3ad3f-121">只读。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-121">Read-only.</span></span> <span data-ttu-id="3ad3f-122">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-122">Nullable.</span></span>|
|<span data-ttu-id="3ad3f-123">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="3ad3f-123">deviceManagement</span></span>|[<span data-ttu-id="3ad3f-124">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="3ad3f-124">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="3ad3f-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ad3f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ad3f-127">JSON representation</span></span>

<span data-ttu-id="3ad3f-128">无。</span><span class="sxs-lookup"><span data-stu-id="3ad3f-128">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
