---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 77150c7a2b883acc6857cd0866459fb9423dfa6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558326"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="1b6da-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b6da-103">auditActor resource type</span></span>

> <span data-ttu-id="1b6da-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b6da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b6da-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b6da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b6da-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="1b6da-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="1b6da-107">属性</span><span class="sxs-lookup"><span data-stu-id="1b6da-107">Properties</span></span>
|<span data-ttu-id="1b6da-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b6da-108">Property</span></span>|<span data-ttu-id="1b6da-109">类型</span><span class="sxs-lookup"><span data-stu-id="1b6da-109">Type</span></span>|<span data-ttu-id="1b6da-110">说明</span><span class="sxs-lookup"><span data-stu-id="1b6da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b6da-111">类型</span><span class="sxs-lookup"><span data-stu-id="1b6da-111">type</span></span>|<span data-ttu-id="1b6da-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1b6da-112">String</span></span>|<span data-ttu-id="1b6da-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="1b6da-113">Actor Type.</span></span>|
|<span data-ttu-id="1b6da-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="1b6da-114">userPermissions</span></span>|<span data-ttu-id="1b6da-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1b6da-115">String collection</span></span>|<span data-ttu-id="1b6da-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="1b6da-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="1b6da-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="1b6da-117">applicationId</span></span>|<span data-ttu-id="1b6da-118">String</span><span class="sxs-lookup"><span data-stu-id="1b6da-118">String</span></span>|<span data-ttu-id="1b6da-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="1b6da-119">AAD Application Id.</span></span>|
|<span data-ttu-id="1b6da-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="1b6da-120">applicationDisplayName</span></span>|<span data-ttu-id="1b6da-121">String</span><span class="sxs-lookup"><span data-stu-id="1b6da-121">String</span></span>|<span data-ttu-id="1b6da-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="1b6da-122">Name of the Application.</span></span>|
|<span data-ttu-id="1b6da-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b6da-123">userPrincipalName</span></span>|<span data-ttu-id="1b6da-124">String</span><span class="sxs-lookup"><span data-stu-id="1b6da-124">String</span></span>|<span data-ttu-id="1b6da-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="1b6da-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="1b6da-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b6da-126">servicePrincipalName</span></span>|<span data-ttu-id="1b6da-127">String</span><span class="sxs-lookup"><span data-stu-id="1b6da-127">String</span></span>|<span data-ttu-id="1b6da-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="1b6da-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="1b6da-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1b6da-129">ipAddress</span></span>|<span data-ttu-id="1b6da-130">String</span><span class="sxs-lookup"><span data-stu-id="1b6da-130">String</span></span>|<span data-ttu-id="1b6da-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="1b6da-131">IPAddress.</span></span>|
|<span data-ttu-id="1b6da-132">userId</span><span class="sxs-lookup"><span data-stu-id="1b6da-132">userId</span></span>|<span data-ttu-id="1b6da-133">String</span><span class="sxs-lookup"><span data-stu-id="1b6da-133">String</span></span>|<span data-ttu-id="1b6da-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="1b6da-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b6da-135">关系</span><span class="sxs-lookup"><span data-stu-id="1b6da-135">Relationships</span></span>
<span data-ttu-id="1b6da-136">无</span><span class="sxs-lookup"><span data-stu-id="1b6da-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b6da-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b6da-137">JSON Representation</span></span>
<span data-ttu-id="1b6da-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b6da-138">Here is a JSON representation of the resource.</span></span>
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





