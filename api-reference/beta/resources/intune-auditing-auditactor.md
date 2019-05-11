---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 16d2aed7e2c72d56340af97936f43984822718e7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949428"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="e9f50-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9f50-103">auditActor resource type</span></span>

> <span data-ttu-id="e9f50-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9f50-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9f50-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9f50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9f50-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="e9f50-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="e9f50-107">属性</span><span class="sxs-lookup"><span data-stu-id="e9f50-107">Properties</span></span>
|<span data-ttu-id="e9f50-108">属性</span><span class="sxs-lookup"><span data-stu-id="e9f50-108">Property</span></span>|<span data-ttu-id="e9f50-109">类型</span><span class="sxs-lookup"><span data-stu-id="e9f50-109">Type</span></span>|<span data-ttu-id="e9f50-110">说明</span><span class="sxs-lookup"><span data-stu-id="e9f50-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f50-111">type</span><span class="sxs-lookup"><span data-stu-id="e9f50-111">type</span></span>|<span data-ttu-id="e9f50-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e9f50-112">String</span></span>|<span data-ttu-id="e9f50-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="e9f50-113">Actor Type.</span></span>|
|<span data-ttu-id="e9f50-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="e9f50-114">userPermissions</span></span>|<span data-ttu-id="e9f50-115">String collection</span><span class="sxs-lookup"><span data-stu-id="e9f50-115">String collection</span></span>|<span data-ttu-id="e9f50-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="e9f50-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="e9f50-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="e9f50-117">applicationId</span></span>|<span data-ttu-id="e9f50-118">String</span><span class="sxs-lookup"><span data-stu-id="e9f50-118">String</span></span>|<span data-ttu-id="e9f50-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="e9f50-119">AAD Application Id.</span></span>|
|<span data-ttu-id="e9f50-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="e9f50-120">applicationDisplayName</span></span>|<span data-ttu-id="e9f50-121">String</span><span class="sxs-lookup"><span data-stu-id="e9f50-121">String</span></span>|<span data-ttu-id="e9f50-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="e9f50-122">Name of the Application.</span></span>|
|<span data-ttu-id="e9f50-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9f50-123">userPrincipalName</span></span>|<span data-ttu-id="e9f50-124">字符串</span><span class="sxs-lookup"><span data-stu-id="e9f50-124">String</span></span>|<span data-ttu-id="e9f50-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="e9f50-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="e9f50-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9f50-126">servicePrincipalName</span></span>|<span data-ttu-id="e9f50-127">String</span><span class="sxs-lookup"><span data-stu-id="e9f50-127">String</span></span>|<span data-ttu-id="e9f50-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="e9f50-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="e9f50-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e9f50-129">ipAddress</span></span>|<span data-ttu-id="e9f50-130">String</span><span class="sxs-lookup"><span data-stu-id="e9f50-130">String</span></span>|<span data-ttu-id="e9f50-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="e9f50-131">IPAddress.</span></span>|
|<span data-ttu-id="e9f50-132">userId</span><span class="sxs-lookup"><span data-stu-id="e9f50-132">userId</span></span>|<span data-ttu-id="e9f50-133">String</span><span class="sxs-lookup"><span data-stu-id="e9f50-133">String</span></span>|<span data-ttu-id="e9f50-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="e9f50-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9f50-135">关系</span><span class="sxs-lookup"><span data-stu-id="e9f50-135">Relationships</span></span>
<span data-ttu-id="e9f50-136">无</span><span class="sxs-lookup"><span data-stu-id="e9f50-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9f50-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9f50-137">JSON Representation</span></span>
<span data-ttu-id="e9f50-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9f50-138">Here is a JSON representation of the resource.</span></span>
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




