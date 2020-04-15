---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2c6a51d99d712305292e17d19487d829bd2e09af
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439530"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="f2136-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2136-103">auditActor resource type</span></span>

<span data-ttu-id="f2136-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2136-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2136-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2136-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2136-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="f2136-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="f2136-107">属性</span><span class="sxs-lookup"><span data-stu-id="f2136-107">Properties</span></span>
|<span data-ttu-id="f2136-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2136-108">Property</span></span>|<span data-ttu-id="f2136-109">类型</span><span class="sxs-lookup"><span data-stu-id="f2136-109">Type</span></span>|<span data-ttu-id="f2136-110">说明</span><span class="sxs-lookup"><span data-stu-id="f2136-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2136-111">type</span><span class="sxs-lookup"><span data-stu-id="f2136-111">type</span></span>|<span data-ttu-id="f2136-112">字符串</span><span class="sxs-lookup"><span data-stu-id="f2136-112">String</span></span>|<span data-ttu-id="f2136-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="f2136-113">Actor Type.</span></span>|
|<span data-ttu-id="f2136-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="f2136-114">userPermissions</span></span>|<span data-ttu-id="f2136-115">String collection</span><span class="sxs-lookup"><span data-stu-id="f2136-115">String collection</span></span>|<span data-ttu-id="f2136-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="f2136-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="f2136-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="f2136-117">applicationId</span></span>|<span data-ttu-id="f2136-118">String</span><span class="sxs-lookup"><span data-stu-id="f2136-118">String</span></span>|<span data-ttu-id="f2136-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="f2136-119">AAD Application Id.</span></span>|
|<span data-ttu-id="f2136-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2136-120">applicationDisplayName</span></span>|<span data-ttu-id="f2136-121">String</span><span class="sxs-lookup"><span data-stu-id="f2136-121">String</span></span>|<span data-ttu-id="f2136-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="f2136-122">Name of the Application.</span></span>|
|<span data-ttu-id="f2136-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2136-123">userPrincipalName</span></span>|<span data-ttu-id="f2136-124">字符串</span><span class="sxs-lookup"><span data-stu-id="f2136-124">String</span></span>|<span data-ttu-id="f2136-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="f2136-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="f2136-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2136-126">servicePrincipalName</span></span>|<span data-ttu-id="f2136-127">String</span><span class="sxs-lookup"><span data-stu-id="f2136-127">String</span></span>|<span data-ttu-id="f2136-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="f2136-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="f2136-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f2136-129">ipAddress</span></span>|<span data-ttu-id="f2136-130">String</span><span class="sxs-lookup"><span data-stu-id="f2136-130">String</span></span>|<span data-ttu-id="f2136-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="f2136-131">IPAddress.</span></span>|
|<span data-ttu-id="f2136-132">userId</span><span class="sxs-lookup"><span data-stu-id="f2136-132">userId</span></span>|<span data-ttu-id="f2136-133">String</span><span class="sxs-lookup"><span data-stu-id="f2136-133">String</span></span>|<span data-ttu-id="f2136-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="f2136-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2136-135">关系</span><span class="sxs-lookup"><span data-stu-id="f2136-135">Relationships</span></span>
<span data-ttu-id="f2136-136">无</span><span class="sxs-lookup"><span data-stu-id="f2136-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2136-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2136-137">JSON Representation</span></span>
<span data-ttu-id="f2136-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2136-138">Here is a JSON representation of the resource.</span></span>
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







