---
title: roleManagement 资源类型
description: RBAC 角色管理资源
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 42cad38bf690b6bb6958cfde99282f049a1a1d10
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317019"
---
# <a name="rolemanagement-resource-type"></a><span data-ttu-id="a2a23-103">roleManagement 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2a23-103">roleManagement resource type</span></span>

<span data-ttu-id="a2a23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2a23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2a23-105">表示一Microsoft 365 RBAC 角色管理实体，该实体提供对各种 RBAC 提供程序显示的角色定义和角色分配的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a2a23-105">Represents a Microsoft 365 RBAC role management entity that provides access to role definitions and role assignments surfaced from various RBAC providers.</span></span> 

<span data-ttu-id="a2a23-106">统一角色管理 API 当前支持以下 RBAC Microsoft 365：</span><span class="sxs-lookup"><span data-stu-id="a2a23-106">The unified role management API currently supports the following RBAC providers in Microsoft 365:</span></span>
- <span data-ttu-id="a2a23-107">云电脑</span><span class="sxs-lookup"><span data-stu-id="a2a23-107">cloud PC</span></span> 
- <span data-ttu-id="a2a23-108">Intune (设备) </span><span class="sxs-lookup"><span data-stu-id="a2a23-108">device management (Intune)</span></span>
- <span data-ttu-id="a2a23-109">directory (Azure AD directory roles) </span><span class="sxs-lookup"><span data-stu-id="a2a23-109">directory (Azure AD directory roles)</span></span>
- <span data-ttu-id="a2a23-110">授权管理 (Azure AD 权利管理) </span><span class="sxs-lookup"><span data-stu-id="a2a23-110">entitlement management (Azure AD entitlement management)</span></span>
 
<span data-ttu-id="a2a23-111">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="a2a23-111">For more information, see:</span></span> 
* [<span data-ttu-id="a2a23-112">Microsoft 365中的角色，包括 Azure AD、特定于服务和跨服务的角色</span><span class="sxs-lookup"><span data-stu-id="a2a23-112">Roles in Microsoft 365, including Azure AD, service-specific and cross-service roles</span></span>](/azure/active-directory/roles/concept-understand-roles#how-azure-ad-roles-are-different-from-other-microsoft-365-roles) 
* <span data-ttu-id="a2a23-113">[Azure Active Directory 中的管理员角色权限](/azure/active-directory/users-groups-roles/directory-assign-admin-roles)。</span><span class="sxs-lookup"><span data-stu-id="a2a23-113">[Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>
* <span data-ttu-id="a2a23-114">[Azure AD 权利管理中的委派和角色](/azure/active-directory/governance/entitlement-management-delegate)。</span><span class="sxs-lookup"><span data-stu-id="a2a23-114">[Delegation and roles in Azure AD entitlement management](/azure/active-directory/governance/entitlement-management-delegate).</span></span>
* <span data-ttu-id="a2a23-115">[Microsoft Intune 中的基于角色的访问控制 (RBAC)](/mem/intune/fundamentals/role-based-access-control)。</span><span class="sxs-lookup"><span data-stu-id="a2a23-115">[Role-based access control (RBAC) with Microsoft Intune](/mem/intune/fundamentals/role-based-access-control)</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a><span data-ttu-id="a2a23-116">Methods</span><span class="sxs-lookup"><span data-stu-id="a2a23-116">Methods</span></span>

<span data-ttu-id="a2a23-117">无。</span><span class="sxs-lookup"><span data-stu-id="a2a23-117">None.</span></span>

## <a name="properties"></a><span data-ttu-id="a2a23-118">属性</span><span class="sxs-lookup"><span data-stu-id="a2a23-118">Properties</span></span>

<span data-ttu-id="a2a23-119">无。</span><span class="sxs-lookup"><span data-stu-id="a2a23-119">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="a2a23-120">关系</span><span class="sxs-lookup"><span data-stu-id="a2a23-120">Relationships</span></span>

| <span data-ttu-id="a2a23-121">关系</span><span class="sxs-lookup"><span data-stu-id="a2a23-121">Relationship</span></span> | <span data-ttu-id="a2a23-122">类型</span><span class="sxs-lookup"><span data-stu-id="a2a23-122">Type</span></span>        | <span data-ttu-id="a2a23-123">说明</span><span class="sxs-lookup"><span data-stu-id="a2a23-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2a23-124">cloudPC</span><span class="sxs-lookup"><span data-stu-id="a2a23-124">cloudPC</span></span>|[<span data-ttu-id="a2a23-125">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="a2a23-125">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)|<span data-ttu-id="a2a23-126">提供对云电脑 RBAC 提供程序的角色定义和角色分配的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a2a23-126">Provides access to role definitions and role assignments of a cloud PC RBAC provider.</span></span> <span data-ttu-id="a2a23-127">只读。</span><span class="sxs-lookup"><span data-stu-id="a2a23-127">Read-only.</span></span> <span data-ttu-id="a2a23-128">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a2a23-128">Nullable.</span></span>|
|<span data-ttu-id="a2a23-129">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="a2a23-129">deviceManagement</span></span>|[<span data-ttu-id="a2a23-130">rbacApplicationMultiple</span><span class="sxs-lookup"><span data-stu-id="a2a23-130">rbacApplicationMultiple</span></span>](rbacapplicationmultiple.md)| <span data-ttu-id="a2a23-131">提供对 Intune RBAC 提供程序的角色定义和角色分配的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a2a23-131">Provides access to role definitions and role assignments of an Intune RBAC provider.</span></span> <span data-ttu-id="a2a23-132">只读。</span><span class="sxs-lookup"><span data-stu-id="a2a23-132">Read-only.</span></span> <span data-ttu-id="a2a23-133">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a2a23-133">Nullable.</span></span>|
|<span data-ttu-id="a2a23-134">directory</span><span class="sxs-lookup"><span data-stu-id="a2a23-134">directory</span></span>|[<span data-ttu-id="a2a23-135">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="a2a23-135">rbacApplication</span></span>](rbacapplication.md)|<span data-ttu-id="a2a23-136">提供对 Azure AD RBAC 提供程序的角色定义和角色分配的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a2a23-136">Provides access to role definitions and role assignments of an Azure AD RBAC provider.</span></span> <span data-ttu-id="a2a23-137">只读。</span><span class="sxs-lookup"><span data-stu-id="a2a23-137">Read-only.</span></span> <span data-ttu-id="a2a23-138">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a2a23-138">Nullable.</span></span>|
|<span data-ttu-id="a2a23-139">entitlementManagement</span><span class="sxs-lookup"><span data-stu-id="a2a23-139">entitlementManagement</span></span>|[<span data-ttu-id="a2a23-140">rbacApplication</span><span class="sxs-lookup"><span data-stu-id="a2a23-140">rbacApplication</span></span>](rbacapplication.md)| <span data-ttu-id="a2a23-141">提供对 Azure AD 权利管理的角色定义和角色分配的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a2a23-141">Provides access to role definitions and role assignments of Azure AD entitlement management.</span></span> <span data-ttu-id="a2a23-142">只读。</span><span class="sxs-lookup"><span data-stu-id="a2a23-142">Read-only.</span></span> <span data-ttu-id="a2a23-143">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="a2a23-143">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2a23-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2a23-144">JSON representation</span></span>

<span data-ttu-id="a2a23-145">无。</span><span class="sxs-lookup"><span data-stu-id="a2a23-145">None.</span></span>

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
