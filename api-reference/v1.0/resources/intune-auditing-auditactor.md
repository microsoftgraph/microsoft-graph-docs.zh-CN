---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 97707795907665ffe65cfee94a53b5d36238c297
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032472"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="9c96e-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c96e-103">auditActor resource type</span></span>

<span data-ttu-id="9c96e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c96e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9c96e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c96e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c96e-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="9c96e-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="9c96e-107">属性</span><span class="sxs-lookup"><span data-stu-id="9c96e-107">Properties</span></span>
|<span data-ttu-id="9c96e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c96e-108">Property</span></span>|<span data-ttu-id="9c96e-109">类型</span><span class="sxs-lookup"><span data-stu-id="9c96e-109">Type</span></span>|<span data-ttu-id="9c96e-110">说明</span><span class="sxs-lookup"><span data-stu-id="9c96e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c96e-111">type</span><span class="sxs-lookup"><span data-stu-id="9c96e-111">type</span></span>|<span data-ttu-id="9c96e-112">String</span><span class="sxs-lookup"><span data-stu-id="9c96e-112">String</span></span>|<span data-ttu-id="9c96e-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="9c96e-113">Actor Type.</span></span>|
|<span data-ttu-id="9c96e-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="9c96e-114">userPermissions</span></span>|<span data-ttu-id="9c96e-115">String collection</span><span class="sxs-lookup"><span data-stu-id="9c96e-115">String collection</span></span>|<span data-ttu-id="9c96e-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="9c96e-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="9c96e-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="9c96e-117">applicationId</span></span>|<span data-ttu-id="9c96e-118">String</span><span class="sxs-lookup"><span data-stu-id="9c96e-118">String</span></span>|<span data-ttu-id="9c96e-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="9c96e-119">AAD Application Id.</span></span>|
|<span data-ttu-id="9c96e-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="9c96e-120">applicationDisplayName</span></span>|<span data-ttu-id="9c96e-121">String</span><span class="sxs-lookup"><span data-stu-id="9c96e-121">String</span></span>|<span data-ttu-id="9c96e-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="9c96e-122">Name of the Application.</span></span>|
|<span data-ttu-id="9c96e-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c96e-123">userPrincipalName</span></span>|<span data-ttu-id="9c96e-124">String</span><span class="sxs-lookup"><span data-stu-id="9c96e-124">String</span></span>|<span data-ttu-id="9c96e-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="9c96e-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="9c96e-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="9c96e-126">servicePrincipalName</span></span>|<span data-ttu-id="9c96e-127">String</span><span class="sxs-lookup"><span data-stu-id="9c96e-127">String</span></span>|<span data-ttu-id="9c96e-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="9c96e-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="9c96e-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="9c96e-129">ipAddress</span></span>|<span data-ttu-id="9c96e-130">String</span><span class="sxs-lookup"><span data-stu-id="9c96e-130">String</span></span>|<span data-ttu-id="9c96e-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="9c96e-131">IPAddress.</span></span>|
|<span data-ttu-id="9c96e-132">userId</span><span class="sxs-lookup"><span data-stu-id="9c96e-132">userId</span></span>|<span data-ttu-id="9c96e-133">String</span><span class="sxs-lookup"><span data-stu-id="9c96e-133">String</span></span>|<span data-ttu-id="9c96e-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="9c96e-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c96e-135">关系</span><span class="sxs-lookup"><span data-stu-id="9c96e-135">Relationships</span></span>
<span data-ttu-id="9c96e-136">无</span><span class="sxs-lookup"><span data-stu-id="9c96e-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c96e-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c96e-137">JSON Representation</span></span>
<span data-ttu-id="9c96e-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c96e-138">Here is a JSON representation of the resource.</span></span>
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
  "userId": "String"
}
```









