---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05fdb86a13c7984975f9a3076909c06fcc5ecbe7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706077"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="6616b-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="6616b-103">auditActor resource type</span></span>

<span data-ttu-id="6616b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6616b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6616b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6616b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6616b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6616b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6616b-107">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="6616b-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="6616b-108">属性</span><span class="sxs-lookup"><span data-stu-id="6616b-108">Properties</span></span>
|<span data-ttu-id="6616b-109">属性</span><span class="sxs-lookup"><span data-stu-id="6616b-109">Property</span></span>|<span data-ttu-id="6616b-110">类型</span><span class="sxs-lookup"><span data-stu-id="6616b-110">Type</span></span>|<span data-ttu-id="6616b-111">说明</span><span class="sxs-lookup"><span data-stu-id="6616b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6616b-112">type</span><span class="sxs-lookup"><span data-stu-id="6616b-112">type</span></span>|<span data-ttu-id="6616b-113">String</span><span class="sxs-lookup"><span data-stu-id="6616b-113">String</span></span>|<span data-ttu-id="6616b-114">主角类型。</span><span class="sxs-lookup"><span data-stu-id="6616b-114">Actor Type.</span></span>|
|<span data-ttu-id="6616b-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="6616b-115">userPermissions</span></span>|<span data-ttu-id="6616b-116">String collection</span><span class="sxs-lookup"><span data-stu-id="6616b-116">String collection</span></span>|<span data-ttu-id="6616b-117">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="6616b-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="6616b-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="6616b-118">applicationId</span></span>|<span data-ttu-id="6616b-119">String</span><span class="sxs-lookup"><span data-stu-id="6616b-119">String</span></span>|<span data-ttu-id="6616b-120">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="6616b-120">AAD Application Id.</span></span>|
|<span data-ttu-id="6616b-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6616b-121">applicationDisplayName</span></span>|<span data-ttu-id="6616b-122">String</span><span class="sxs-lookup"><span data-stu-id="6616b-122">String</span></span>|<span data-ttu-id="6616b-123">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="6616b-123">Name of the Application.</span></span>|
|<span data-ttu-id="6616b-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6616b-124">userPrincipalName</span></span>|<span data-ttu-id="6616b-125">String</span><span class="sxs-lookup"><span data-stu-id="6616b-125">String</span></span>|<span data-ttu-id="6616b-126">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="6616b-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="6616b-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="6616b-127">servicePrincipalName</span></span>|<span data-ttu-id="6616b-128">String</span><span class="sxs-lookup"><span data-stu-id="6616b-128">String</span></span>|<span data-ttu-id="6616b-129">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="6616b-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="6616b-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6616b-130">ipAddress</span></span>|<span data-ttu-id="6616b-131">String</span><span class="sxs-lookup"><span data-stu-id="6616b-131">String</span></span>|<span data-ttu-id="6616b-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="6616b-132">IPAddress.</span></span>|
|<span data-ttu-id="6616b-133">userId</span><span class="sxs-lookup"><span data-stu-id="6616b-133">userId</span></span>|<span data-ttu-id="6616b-134">String</span><span class="sxs-lookup"><span data-stu-id="6616b-134">String</span></span>|<span data-ttu-id="6616b-135">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6616b-135">User Id.</span></span>|
|<span data-ttu-id="6616b-136">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="6616b-136">userRoleScopeTags</span></span>|<span data-ttu-id="6616b-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6616b-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="6616b-138">执行审核时的用户范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6616b-138">List of user scope tags when the audit was performed.</span></span>|
|<span data-ttu-id="6616b-139">remoteTenantId</span><span class="sxs-lookup"><span data-stu-id="6616b-139">remoteTenantId</span></span>|<span data-ttu-id="6616b-140">String</span><span class="sxs-lookup"><span data-stu-id="6616b-140">String</span></span>|<span data-ttu-id="6616b-141">远程租户 Id</span><span class="sxs-lookup"><span data-stu-id="6616b-141">Remote Tenant Id</span></span>|
|<span data-ttu-id="6616b-142">remoteUserId</span><span class="sxs-lookup"><span data-stu-id="6616b-142">remoteUserId</span></span>|<span data-ttu-id="6616b-143">String</span><span class="sxs-lookup"><span data-stu-id="6616b-143">String</span></span>|<span data-ttu-id="6616b-144">远程用户 Id</span><span class="sxs-lookup"><span data-stu-id="6616b-144">Remote User Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="6616b-145">关系</span><span class="sxs-lookup"><span data-stu-id="6616b-145">Relationships</span></span>
<span data-ttu-id="6616b-146">无</span><span class="sxs-lookup"><span data-stu-id="6616b-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6616b-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6616b-147">JSON Representation</span></span>
<span data-ttu-id="6616b-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6616b-148">Here is a JSON representation of the resource.</span></span>
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





