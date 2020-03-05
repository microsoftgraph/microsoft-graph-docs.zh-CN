---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40aa3d256da1d7a1c50fc898c6755a82185897ac
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489487"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="21d14-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="21d14-103">auditActor resource type</span></span>

<span data-ttu-id="21d14-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="21d14-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21d14-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21d14-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21d14-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21d14-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d14-107">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="21d14-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="21d14-108">属性</span><span class="sxs-lookup"><span data-stu-id="21d14-108">Properties</span></span>
|<span data-ttu-id="21d14-109">属性</span><span class="sxs-lookup"><span data-stu-id="21d14-109">Property</span></span>|<span data-ttu-id="21d14-110">类型</span><span class="sxs-lookup"><span data-stu-id="21d14-110">Type</span></span>|<span data-ttu-id="21d14-111">说明</span><span class="sxs-lookup"><span data-stu-id="21d14-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21d14-112">type</span><span class="sxs-lookup"><span data-stu-id="21d14-112">type</span></span>|<span data-ttu-id="21d14-113">字符串</span><span class="sxs-lookup"><span data-stu-id="21d14-113">String</span></span>|<span data-ttu-id="21d14-114">主角类型。</span><span class="sxs-lookup"><span data-stu-id="21d14-114">Actor Type.</span></span>|
|<span data-ttu-id="21d14-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="21d14-115">userPermissions</span></span>|<span data-ttu-id="21d14-116">String collection</span><span class="sxs-lookup"><span data-stu-id="21d14-116">String collection</span></span>|<span data-ttu-id="21d14-117">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="21d14-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="21d14-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="21d14-118">applicationId</span></span>|<span data-ttu-id="21d14-119">String</span><span class="sxs-lookup"><span data-stu-id="21d14-119">String</span></span>|<span data-ttu-id="21d14-120">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="21d14-120">AAD Application Id.</span></span>|
|<span data-ttu-id="21d14-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="21d14-121">applicationDisplayName</span></span>|<span data-ttu-id="21d14-122">String</span><span class="sxs-lookup"><span data-stu-id="21d14-122">String</span></span>|<span data-ttu-id="21d14-123">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="21d14-123">Name of the Application.</span></span>|
|<span data-ttu-id="21d14-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="21d14-124">userPrincipalName</span></span>|<span data-ttu-id="21d14-125">字符串</span><span class="sxs-lookup"><span data-stu-id="21d14-125">String</span></span>|<span data-ttu-id="21d14-126">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="21d14-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="21d14-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="21d14-127">servicePrincipalName</span></span>|<span data-ttu-id="21d14-128">String</span><span class="sxs-lookup"><span data-stu-id="21d14-128">String</span></span>|<span data-ttu-id="21d14-129">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="21d14-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="21d14-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="21d14-130">ipAddress</span></span>|<span data-ttu-id="21d14-131">String</span><span class="sxs-lookup"><span data-stu-id="21d14-131">String</span></span>|<span data-ttu-id="21d14-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="21d14-132">IPAddress.</span></span>|
|<span data-ttu-id="21d14-133">userId</span><span class="sxs-lookup"><span data-stu-id="21d14-133">userId</span></span>|<span data-ttu-id="21d14-134">String</span><span class="sxs-lookup"><span data-stu-id="21d14-134">String</span></span>|<span data-ttu-id="21d14-135">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="21d14-135">User Id.</span></span>|
|<span data-ttu-id="21d14-136">userRoleScopeTags</span><span class="sxs-lookup"><span data-stu-id="21d14-136">userRoleScopeTags</span></span>|<span data-ttu-id="21d14-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="21d14-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="21d14-138">执行审核时的用户范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="21d14-138">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21d14-139">关系</span><span class="sxs-lookup"><span data-stu-id="21d14-139">Relationships</span></span>
<span data-ttu-id="21d14-140">无</span><span class="sxs-lookup"><span data-stu-id="21d14-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21d14-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21d14-141">JSON Representation</span></span>
<span data-ttu-id="21d14-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21d14-142">Here is a JSON representation of the resource.</span></span>
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



