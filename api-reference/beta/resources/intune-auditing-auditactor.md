---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c2aba128e4c781dab30f226e25f5240e1f95db17
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38078334"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="6aaf3-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="6aaf3-103">auditActor resource type</span></span>

> <span data-ttu-id="6aaf3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6aaf3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6aaf3-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="6aaf3-107">属性</span><span class="sxs-lookup"><span data-stu-id="6aaf3-107">Properties</span></span>
|<span data-ttu-id="6aaf3-108">属性</span><span class="sxs-lookup"><span data-stu-id="6aaf3-108">Property</span></span>|<span data-ttu-id="6aaf3-109">类型</span><span class="sxs-lookup"><span data-stu-id="6aaf3-109">Type</span></span>|<span data-ttu-id="6aaf3-110">描述</span><span class="sxs-lookup"><span data-stu-id="6aaf3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6aaf3-111">type</span><span class="sxs-lookup"><span data-stu-id="6aaf3-111">type</span></span>|<span data-ttu-id="6aaf3-112">字符串</span><span class="sxs-lookup"><span data-stu-id="6aaf3-112">String</span></span>|<span data-ttu-id="6aaf3-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-113">Actor Type.</span></span>|
|<span data-ttu-id="6aaf3-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="6aaf3-114">userPermissions</span></span>|<span data-ttu-id="6aaf3-115">String collection</span><span class="sxs-lookup"><span data-stu-id="6aaf3-115">String collection</span></span>|<span data-ttu-id="6aaf3-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="6aaf3-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="6aaf3-117">applicationId</span></span>|<span data-ttu-id="6aaf3-118">String</span><span class="sxs-lookup"><span data-stu-id="6aaf3-118">String</span></span>|<span data-ttu-id="6aaf3-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-119">AAD Application Id.</span></span>|
|<span data-ttu-id="6aaf3-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6aaf3-120">applicationDisplayName</span></span>|<span data-ttu-id="6aaf3-121">String</span><span class="sxs-lookup"><span data-stu-id="6aaf3-121">String</span></span>|<span data-ttu-id="6aaf3-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-122">Name of the Application.</span></span>|
|<span data-ttu-id="6aaf3-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6aaf3-123">userPrincipalName</span></span>|<span data-ttu-id="6aaf3-124">字符串</span><span class="sxs-lookup"><span data-stu-id="6aaf3-124">String</span></span>|<span data-ttu-id="6aaf3-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="6aaf3-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="6aaf3-126">servicePrincipalName</span></span>|<span data-ttu-id="6aaf3-127">String</span><span class="sxs-lookup"><span data-stu-id="6aaf3-127">String</span></span>|<span data-ttu-id="6aaf3-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="6aaf3-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6aaf3-129">ipAddress</span></span>|<span data-ttu-id="6aaf3-130">String</span><span class="sxs-lookup"><span data-stu-id="6aaf3-130">String</span></span>|<span data-ttu-id="6aaf3-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-131">IPAddress.</span></span>|
|<span data-ttu-id="6aaf3-132">userId</span><span class="sxs-lookup"><span data-stu-id="6aaf3-132">userId</span></span>|<span data-ttu-id="6aaf3-133">String</span><span class="sxs-lookup"><span data-stu-id="6aaf3-133">String</span></span>|<span data-ttu-id="6aaf3-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-134">User Id.</span></span>|
|<span data-ttu-id="6aaf3-135">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="6aaf3-135">userRoleScopeTags</span></span>|<span data-ttu-id="6aaf3-136">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="6aaf3-136">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="6aaf3-137">执行审核时的用户范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-137">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6aaf3-138">关系</span><span class="sxs-lookup"><span data-stu-id="6aaf3-138">Relationships</span></span>
<span data-ttu-id="6aaf3-139">无</span><span class="sxs-lookup"><span data-stu-id="6aaf3-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6aaf3-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6aaf3-140">JSON Representation</span></span>
<span data-ttu-id="6aaf3-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6aaf3-141">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```



