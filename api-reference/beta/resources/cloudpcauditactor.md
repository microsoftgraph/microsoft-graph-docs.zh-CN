---
title: cloudPcAuditActor 资源类型
description: 由 Azure AD 用户和与审核事件关联的应用程序表示的审核参与者。
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c0c63e9e9d0db7a5227f0ab7b818c8ab3d3944d9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211224"
---
# <a name="cloudpcauditactor-resource-type"></a><span data-ttu-id="e5332-103">cloudPcAuditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5332-103">cloudPcAuditActor resource type</span></span>

<span data-ttu-id="e5332-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5332-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5332-105">由 Azure AD 用户和与审核事件关联的应用程序表示的审核参与者。</span><span class="sxs-lookup"><span data-stu-id="e5332-105">The audit actor represented by the Azure AD user and application associated with the audit event.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="e5332-106">属性</span><span class="sxs-lookup"><span data-stu-id="e5332-106">Properties</span></span>

|<span data-ttu-id="e5332-107">属性</span><span class="sxs-lookup"><span data-stu-id="e5332-107">Property</span></span>|<span data-ttu-id="e5332-108">类型</span><span class="sxs-lookup"><span data-stu-id="e5332-108">Type</span></span>|<span data-ttu-id="e5332-109">说明</span><span class="sxs-lookup"><span data-stu-id="e5332-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5332-110">类型</span><span class="sxs-lookup"><span data-stu-id="e5332-110">type</span></span>|[<span data-ttu-id="e5332-111">cloudPcAuditActorType</span><span class="sxs-lookup"><span data-stu-id="e5332-111">cloudPcAuditActorType</span></span>](#cloudpcauditactortype-values)|<span data-ttu-id="e5332-112">主角类型。</span><span class="sxs-lookup"><span data-stu-id="e5332-112">The actor type.</span></span> <span data-ttu-id="e5332-113">可能的值包括 `ItPro` 、 `Application` 和 `Partner` `Unknown` 。</span><span class="sxs-lookup"><span data-stu-id="e5332-113">Possible values include `ItPro`, `Application`, `Partner` and `Unknown`.</span></span>|
|<span data-ttu-id="e5332-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="e5332-114">userPermissions</span></span>|<span data-ttu-id="e5332-115">String collection</span><span class="sxs-lookup"><span data-stu-id="e5332-115">String collection</span></span>|<span data-ttu-id="e5332-116">执行审核事件时的用户权限和应用程序权限列表。</span><span class="sxs-lookup"><span data-stu-id="e5332-116">List of user permissions and application permissions when the audit event was performed.</span></span>|
|<span data-ttu-id="e5332-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="e5332-117">applicationId</span></span>|<span data-ttu-id="e5332-118">String</span><span class="sxs-lookup"><span data-stu-id="e5332-118">String</span></span>|<span data-ttu-id="e5332-119">Azure AD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="e5332-119">Azure AD application ID.</span></span>|
|<span data-ttu-id="e5332-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="e5332-120">applicationDisplayName</span></span>|<span data-ttu-id="e5332-121">String</span><span class="sxs-lookup"><span data-stu-id="e5332-121">String</span></span>|<span data-ttu-id="e5332-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="e5332-122">Name of the application.</span></span>|
|<span data-ttu-id="e5332-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e5332-123">userPrincipalName</span></span>|<span data-ttu-id="e5332-124">String</span><span class="sxs-lookup"><span data-stu-id="e5332-124">String</span></span>|<span data-ttu-id="e5332-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="e5332-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="e5332-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="e5332-126">servicePrincipalName</span></span>|<span data-ttu-id="e5332-127">String</span><span class="sxs-lookup"><span data-stu-id="e5332-127">String</span></span>|<span data-ttu-id="e5332-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="e5332-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="e5332-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e5332-129">ipAddress</span></span>|<span data-ttu-id="e5332-130">String</span><span class="sxs-lookup"><span data-stu-id="e5332-130">String</span></span>|<span data-ttu-id="e5332-131">IP 地址。</span><span class="sxs-lookup"><span data-stu-id="e5332-131">IP address.</span></span>|
|<span data-ttu-id="e5332-132">userId</span><span class="sxs-lookup"><span data-stu-id="e5332-132">userId</span></span>|<span data-ttu-id="e5332-133">String</span><span class="sxs-lookup"><span data-stu-id="e5332-133">String</span></span>|<span data-ttu-id="e5332-134">Azure AD 用户 ID。</span><span class="sxs-lookup"><span data-stu-id="e5332-134">Azure AD user ID.</span></span>|
|<span data-ttu-id="e5332-135">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="e5332-135">userRoleScopeTags</span></span>|<span data-ttu-id="e5332-136">[cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e5332-136">[cloudPcUserRoleScopeTagInfo](../resources/cloudpcuserrolescopetaginfo.md) collection</span></span>|<span data-ttu-id="e5332-137">角色范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="e5332-137">List of role scope tags.</span></span>|
|<span data-ttu-id="e5332-138">remoteTenantId</span><span class="sxs-lookup"><span data-stu-id="e5332-138">remoteTenantId</span></span>|<span data-ttu-id="e5332-139">String</span><span class="sxs-lookup"><span data-stu-id="e5332-139">String</span></span>|<span data-ttu-id="e5332-140">委派的合作伙伴租户 ID。</span><span class="sxs-lookup"><span data-stu-id="e5332-140">The delegated partner tenant ID.</span></span>|
|<span data-ttu-id="e5332-141">remoteUserId</span><span class="sxs-lookup"><span data-stu-id="e5332-141">remoteUserId</span></span>|<span data-ttu-id="e5332-142">String</span><span class="sxs-lookup"><span data-stu-id="e5332-142">String</span></span>|<span data-ttu-id="e5332-143">委派的合作伙伴用户 ID。</span><span class="sxs-lookup"><span data-stu-id="e5332-143">The delegated partner user ID.</span></span>|

### <a name="cloudpcauditactortype-values"></a><span data-ttu-id="e5332-144">cloudPcAuditActorType 值</span><span class="sxs-lookup"><span data-stu-id="e5332-144">cloudPcAuditActorType values</span></span>

|<span data-ttu-id="e5332-145">成员</span><span class="sxs-lookup"><span data-stu-id="e5332-145">Member</span></span>|<span data-ttu-id="e5332-146">说明</span><span class="sxs-lookup"><span data-stu-id="e5332-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e5332-147">itPro</span><span class="sxs-lookup"><span data-stu-id="e5332-147">itPro</span></span>|<span data-ttu-id="e5332-148">该操作由 IT 专业人员执行。</span><span class="sxs-lookup"><span data-stu-id="e5332-148">The operation was performed by an IT pro.</span></span>|
|<span data-ttu-id="e5332-149">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5332-149">application</span></span>|<span data-ttu-id="e5332-150">操作由应用程序执行。</span><span class="sxs-lookup"><span data-stu-id="e5332-150">The operation was performed by the application.</span></span>|
|<span data-ttu-id="e5332-151">partner</span><span class="sxs-lookup"><span data-stu-id="e5332-151">partner</span></span>|<span data-ttu-id="e5332-152">操作由合作伙伴执行。</span><span class="sxs-lookup"><span data-stu-id="e5332-152">The operation was performed by a partner.</span></span>|
|<span data-ttu-id="e5332-153">unknown</span><span class="sxs-lookup"><span data-stu-id="e5332-153">unknown</span></span>|<span data-ttu-id="e5332-154">未知主角。</span><span class="sxs-lookup"><span data-stu-id="e5332-154">Unknown actor.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5332-155">关系</span><span class="sxs-lookup"><span data-stu-id="e5332-155">Relationships</span></span>

<span data-ttu-id="e5332-156">无。</span><span class="sxs-lookup"><span data-stu-id="e5332-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5332-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5332-157">JSON Representation</span></span>

<span data-ttu-id="e5332-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5332-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditActor"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.cloudPcUserRoleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```
