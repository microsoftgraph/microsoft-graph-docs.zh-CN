---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 632e3018f606b62171461b4b1235ccdafc6b1b5a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254455"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="6c8ea-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="6c8ea-103">auditActor resource type</span></span>

> <span data-ttu-id="6c8ea-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c8ea-105">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="6c8ea-106">属性</span><span class="sxs-lookup"><span data-stu-id="6c8ea-106">Properties</span></span>
|<span data-ttu-id="6c8ea-107">属性</span><span class="sxs-lookup"><span data-stu-id="6c8ea-107">Property</span></span>|<span data-ttu-id="6c8ea-108">类型</span><span class="sxs-lookup"><span data-stu-id="6c8ea-108">Type</span></span>|<span data-ttu-id="6c8ea-109">说明</span><span class="sxs-lookup"><span data-stu-id="6c8ea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c8ea-110">type</span><span class="sxs-lookup"><span data-stu-id="6c8ea-110">type</span></span>|<span data-ttu-id="6c8ea-111">字符串</span><span class="sxs-lookup"><span data-stu-id="6c8ea-111">String</span></span>|<span data-ttu-id="6c8ea-112">主角类型。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-112">Actor Type.</span></span>|
|<span data-ttu-id="6c8ea-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="6c8ea-113">userPermissions</span></span>|<span data-ttu-id="6c8ea-114">String collection</span><span class="sxs-lookup"><span data-stu-id="6c8ea-114">String collection</span></span>|<span data-ttu-id="6c8ea-115">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="6c8ea-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="6c8ea-116">applicationId</span></span>|<span data-ttu-id="6c8ea-117">String</span><span class="sxs-lookup"><span data-stu-id="6c8ea-117">String</span></span>|<span data-ttu-id="6c8ea-118">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-118">AAD Application Id.</span></span>|
|<span data-ttu-id="6c8ea-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="6c8ea-119">applicationDisplayName</span></span>|<span data-ttu-id="6c8ea-120">String</span><span class="sxs-lookup"><span data-stu-id="6c8ea-120">String</span></span>|<span data-ttu-id="6c8ea-121">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-121">Name of the Application.</span></span>|
|<span data-ttu-id="6c8ea-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c8ea-122">userPrincipalName</span></span>|<span data-ttu-id="6c8ea-123">String</span><span class="sxs-lookup"><span data-stu-id="6c8ea-123">String</span></span>|<span data-ttu-id="6c8ea-124">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="6c8ea-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="6c8ea-125">servicePrincipalName</span></span>|<span data-ttu-id="6c8ea-126">String</span><span class="sxs-lookup"><span data-stu-id="6c8ea-126">String</span></span>|<span data-ttu-id="6c8ea-127">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="6c8ea-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="6c8ea-128">ipAddress</span></span>|<span data-ttu-id="6c8ea-129">String</span><span class="sxs-lookup"><span data-stu-id="6c8ea-129">String</span></span>|<span data-ttu-id="6c8ea-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-130">IPAddress.</span></span>|
|<span data-ttu-id="6c8ea-131">userId</span><span class="sxs-lookup"><span data-stu-id="6c8ea-131">userId</span></span>|<span data-ttu-id="6c8ea-132">String</span><span class="sxs-lookup"><span data-stu-id="6c8ea-132">String</span></span>|<span data-ttu-id="6c8ea-133">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c8ea-134">关系</span><span class="sxs-lookup"><span data-stu-id="6c8ea-134">Relationships</span></span>
<span data-ttu-id="6c8ea-135">无</span><span class="sxs-lookup"><span data-stu-id="6c8ea-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c8ea-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6c8ea-136">JSON Representation</span></span>
<span data-ttu-id="6c8ea-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6c8ea-137">Here is a JSON representation of the resource.</span></span>
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



