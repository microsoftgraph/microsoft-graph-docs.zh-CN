---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c10ac0a18f5bfcf68be56edc402c83d9882a8ff
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532737"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="ed7b1-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed7b1-103">auditActor resource type</span></span>

<span data-ttu-id="ed7b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed7b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed7b1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed7b1-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="ed7b1-107">属性</span><span class="sxs-lookup"><span data-stu-id="ed7b1-107">Properties</span></span>
|<span data-ttu-id="ed7b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed7b1-108">Property</span></span>|<span data-ttu-id="ed7b1-109">类型</span><span class="sxs-lookup"><span data-stu-id="ed7b1-109">Type</span></span>|<span data-ttu-id="ed7b1-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed7b1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed7b1-111">type</span><span class="sxs-lookup"><span data-stu-id="ed7b1-111">type</span></span>|<span data-ttu-id="ed7b1-112">字符串</span><span class="sxs-lookup"><span data-stu-id="ed7b1-112">String</span></span>|<span data-ttu-id="ed7b1-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-113">Actor Type.</span></span>|
|<span data-ttu-id="ed7b1-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="ed7b1-114">userPermissions</span></span>|<span data-ttu-id="ed7b1-115">String collection</span><span class="sxs-lookup"><span data-stu-id="ed7b1-115">String collection</span></span>|<span data-ttu-id="ed7b1-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="ed7b1-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="ed7b1-117">applicationId</span></span>|<span data-ttu-id="ed7b1-118">字符串</span><span class="sxs-lookup"><span data-stu-id="ed7b1-118">String</span></span>|<span data-ttu-id="ed7b1-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-119">AAD Application Id.</span></span>|
|<span data-ttu-id="ed7b1-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="ed7b1-120">applicationDisplayName</span></span>|<span data-ttu-id="ed7b1-121">字符串</span><span class="sxs-lookup"><span data-stu-id="ed7b1-121">String</span></span>|<span data-ttu-id="ed7b1-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-122">Name of the Application.</span></span>|
|<span data-ttu-id="ed7b1-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed7b1-123">userPrincipalName</span></span>|<span data-ttu-id="ed7b1-124">字符串</span><span class="sxs-lookup"><span data-stu-id="ed7b1-124">String</span></span>|<span data-ttu-id="ed7b1-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="ed7b1-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="ed7b1-126">servicePrincipalName</span></span>|<span data-ttu-id="ed7b1-127">字符串</span><span class="sxs-lookup"><span data-stu-id="ed7b1-127">String</span></span>|<span data-ttu-id="ed7b1-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="ed7b1-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="ed7b1-129">ipAddress</span></span>|<span data-ttu-id="ed7b1-130">String</span><span class="sxs-lookup"><span data-stu-id="ed7b1-130">String</span></span>|<span data-ttu-id="ed7b1-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-131">IPAddress.</span></span>|
|<span data-ttu-id="ed7b1-132">userId</span><span class="sxs-lookup"><span data-stu-id="ed7b1-132">userId</span></span>|<span data-ttu-id="ed7b1-133">String</span><span class="sxs-lookup"><span data-stu-id="ed7b1-133">String</span></span>|<span data-ttu-id="ed7b1-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed7b1-135">关系</span><span class="sxs-lookup"><span data-stu-id="ed7b1-135">Relationships</span></span>
<span data-ttu-id="ed7b1-136">无</span><span class="sxs-lookup"><span data-stu-id="ed7b1-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ed7b1-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed7b1-137">JSON Representation</span></span>
<span data-ttu-id="ed7b1-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed7b1-138">Here is a JSON representation of the resource.</span></span>
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




