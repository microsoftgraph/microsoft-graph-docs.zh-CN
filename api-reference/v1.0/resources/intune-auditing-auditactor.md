---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4365daebf50de210482132354c14199c850e384a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355993"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="99278-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="99278-103">auditActor resource type</span></span>

> <span data-ttu-id="99278-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99278-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99278-105">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="99278-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="99278-106">属性</span><span class="sxs-lookup"><span data-stu-id="99278-106">Properties</span></span>
|<span data-ttu-id="99278-107">属性</span><span class="sxs-lookup"><span data-stu-id="99278-107">Property</span></span>|<span data-ttu-id="99278-108">类型</span><span class="sxs-lookup"><span data-stu-id="99278-108">Type</span></span>|<span data-ttu-id="99278-109">说明</span><span class="sxs-lookup"><span data-stu-id="99278-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99278-110">type</span><span class="sxs-lookup"><span data-stu-id="99278-110">type</span></span>|<span data-ttu-id="99278-111">字符串</span><span class="sxs-lookup"><span data-stu-id="99278-111">String</span></span>|<span data-ttu-id="99278-112">主角类型。</span><span class="sxs-lookup"><span data-stu-id="99278-112">Actor Type.</span></span>|
|<span data-ttu-id="99278-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="99278-113">userPermissions</span></span>|<span data-ttu-id="99278-114">String collection</span><span class="sxs-lookup"><span data-stu-id="99278-114">String collection</span></span>|<span data-ttu-id="99278-115">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="99278-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="99278-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="99278-116">applicationId</span></span>|<span data-ttu-id="99278-117">String</span><span class="sxs-lookup"><span data-stu-id="99278-117">String</span></span>|<span data-ttu-id="99278-118">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="99278-118">AAD Application Id.</span></span>|
|<span data-ttu-id="99278-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="99278-119">applicationDisplayName</span></span>|<span data-ttu-id="99278-120">String</span><span class="sxs-lookup"><span data-stu-id="99278-120">String</span></span>|<span data-ttu-id="99278-121">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="99278-121">Name of the Application.</span></span>|
|<span data-ttu-id="99278-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="99278-122">userPrincipalName</span></span>|<span data-ttu-id="99278-123">字符串</span><span class="sxs-lookup"><span data-stu-id="99278-123">String</span></span>|<span data-ttu-id="99278-124">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="99278-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="99278-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="99278-125">servicePrincipalName</span></span>|<span data-ttu-id="99278-126">String</span><span class="sxs-lookup"><span data-stu-id="99278-126">String</span></span>|<span data-ttu-id="99278-127">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="99278-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="99278-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="99278-128">ipAddress</span></span>|<span data-ttu-id="99278-129">String</span><span class="sxs-lookup"><span data-stu-id="99278-129">String</span></span>|<span data-ttu-id="99278-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="99278-130">IPAddress.</span></span>|
|<span data-ttu-id="99278-131">userId</span><span class="sxs-lookup"><span data-stu-id="99278-131">userId</span></span>|<span data-ttu-id="99278-132">String</span><span class="sxs-lookup"><span data-stu-id="99278-132">String</span></span>|<span data-ttu-id="99278-133">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="99278-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99278-134">关系</span><span class="sxs-lookup"><span data-stu-id="99278-134">Relationships</span></span>
<span data-ttu-id="99278-135">无</span><span class="sxs-lookup"><span data-stu-id="99278-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99278-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99278-136">JSON Representation</span></span>
<span data-ttu-id="99278-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99278-137">Here is a JSON representation of the resource.</span></span>
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




