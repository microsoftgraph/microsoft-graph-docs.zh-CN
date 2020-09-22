---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8edf9b9ab9b0513e77bbef6ce04dfcd5d4a1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019563"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="3b817-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="3b817-103">auditActor resource type</span></span>

<span data-ttu-id="3b817-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b817-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b817-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b817-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b817-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b817-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b817-107">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="3b817-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="3b817-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b817-108">Properties</span></span>
|<span data-ttu-id="3b817-109">属性</span><span class="sxs-lookup"><span data-stu-id="3b817-109">Property</span></span>|<span data-ttu-id="3b817-110">类型</span><span class="sxs-lookup"><span data-stu-id="3b817-110">Type</span></span>|<span data-ttu-id="3b817-111">说明</span><span class="sxs-lookup"><span data-stu-id="3b817-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b817-112">type</span><span class="sxs-lookup"><span data-stu-id="3b817-112">type</span></span>|<span data-ttu-id="3b817-113">String</span><span class="sxs-lookup"><span data-stu-id="3b817-113">String</span></span>|<span data-ttu-id="3b817-114">主角类型。</span><span class="sxs-lookup"><span data-stu-id="3b817-114">Actor Type.</span></span>|
|<span data-ttu-id="3b817-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="3b817-115">userPermissions</span></span>|<span data-ttu-id="3b817-116">String collection</span><span class="sxs-lookup"><span data-stu-id="3b817-116">String collection</span></span>|<span data-ttu-id="3b817-117">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="3b817-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="3b817-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="3b817-118">applicationId</span></span>|<span data-ttu-id="3b817-119">String</span><span class="sxs-lookup"><span data-stu-id="3b817-119">String</span></span>|<span data-ttu-id="3b817-120">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="3b817-120">AAD Application Id.</span></span>|
|<span data-ttu-id="3b817-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="3b817-121">applicationDisplayName</span></span>|<span data-ttu-id="3b817-122">String</span><span class="sxs-lookup"><span data-stu-id="3b817-122">String</span></span>|<span data-ttu-id="3b817-123">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="3b817-123">Name of the Application.</span></span>|
|<span data-ttu-id="3b817-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b817-124">userPrincipalName</span></span>|<span data-ttu-id="3b817-125">String</span><span class="sxs-lookup"><span data-stu-id="3b817-125">String</span></span>|<span data-ttu-id="3b817-126">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="3b817-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="3b817-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="3b817-127">servicePrincipalName</span></span>|<span data-ttu-id="3b817-128">String</span><span class="sxs-lookup"><span data-stu-id="3b817-128">String</span></span>|<span data-ttu-id="3b817-129">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="3b817-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="3b817-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="3b817-130">ipAddress</span></span>|<span data-ttu-id="3b817-131">String</span><span class="sxs-lookup"><span data-stu-id="3b817-131">String</span></span>|<span data-ttu-id="3b817-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="3b817-132">IPAddress.</span></span>|
|<span data-ttu-id="3b817-133">userId</span><span class="sxs-lookup"><span data-stu-id="3b817-133">userId</span></span>|<span data-ttu-id="3b817-134">String</span><span class="sxs-lookup"><span data-stu-id="3b817-134">String</span></span>|<span data-ttu-id="3b817-135">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="3b817-135">User Id.</span></span>|
|<span data-ttu-id="3b817-136">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="3b817-136">userRoleScopeTags</span></span>|<span data-ttu-id="3b817-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3b817-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="3b817-138">执行审核时的用户范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3b817-138">List of user scope tags when the audit was performed.</span></span>|
|<span data-ttu-id="3b817-139">remoteTenantId</span><span class="sxs-lookup"><span data-stu-id="3b817-139">remoteTenantId</span></span>|<span data-ttu-id="3b817-140">String</span><span class="sxs-lookup"><span data-stu-id="3b817-140">String</span></span>|<span data-ttu-id="3b817-141">远程租户 Id</span><span class="sxs-lookup"><span data-stu-id="3b817-141">Remote Tenant Id</span></span>|
|<span data-ttu-id="3b817-142">remoteUserId</span><span class="sxs-lookup"><span data-stu-id="3b817-142">remoteUserId</span></span>|<span data-ttu-id="3b817-143">String</span><span class="sxs-lookup"><span data-stu-id="3b817-143">String</span></span>|<span data-ttu-id="3b817-144">远程用户 Id</span><span class="sxs-lookup"><span data-stu-id="3b817-144">Remote User Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b817-145">关系</span><span class="sxs-lookup"><span data-stu-id="3b817-145">Relationships</span></span>
<span data-ttu-id="3b817-146">无</span><span class="sxs-lookup"><span data-stu-id="3b817-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b817-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3b817-147">JSON Representation</span></span>
<span data-ttu-id="3b817-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b817-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
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
      "@odata.type": "microsoft.graph.roleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```






