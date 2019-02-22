---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b748eaea907bc2f763bb5567d7963c33b31bddd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141123"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="5ee09-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ee09-103">auditActor resource type</span></span>

> <span data-ttu-id="5ee09-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5ee09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ee09-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ee09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee09-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="5ee09-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="5ee09-107">属性</span><span class="sxs-lookup"><span data-stu-id="5ee09-107">Properties</span></span>
|<span data-ttu-id="5ee09-108">属性</span><span class="sxs-lookup"><span data-stu-id="5ee09-108">Property</span></span>|<span data-ttu-id="5ee09-109">类型</span><span class="sxs-lookup"><span data-stu-id="5ee09-109">Type</span></span>|<span data-ttu-id="5ee09-110">说明</span><span class="sxs-lookup"><span data-stu-id="5ee09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee09-111">type</span><span class="sxs-lookup"><span data-stu-id="5ee09-111">type</span></span>|<span data-ttu-id="5ee09-112">字符串</span><span class="sxs-lookup"><span data-stu-id="5ee09-112">String</span></span>|<span data-ttu-id="5ee09-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="5ee09-113">Actor Type.</span></span>|
|<span data-ttu-id="5ee09-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="5ee09-114">userPermissions</span></span>|<span data-ttu-id="5ee09-115">String collection</span><span class="sxs-lookup"><span data-stu-id="5ee09-115">String collection</span></span>|<span data-ttu-id="5ee09-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="5ee09-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="5ee09-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="5ee09-117">applicationId</span></span>|<span data-ttu-id="5ee09-118">字符串</span><span class="sxs-lookup"><span data-stu-id="5ee09-118">String</span></span>|<span data-ttu-id="5ee09-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="5ee09-119">AAD Application Id.</span></span>|
|<span data-ttu-id="5ee09-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="5ee09-120">applicationDisplayName</span></span>|<span data-ttu-id="5ee09-121">字符串</span><span class="sxs-lookup"><span data-stu-id="5ee09-121">String</span></span>|<span data-ttu-id="5ee09-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="5ee09-122">Name of the Application.</span></span>|
|<span data-ttu-id="5ee09-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ee09-123">userPrincipalName</span></span>|<span data-ttu-id="5ee09-124">字符串</span><span class="sxs-lookup"><span data-stu-id="5ee09-124">String</span></span>|<span data-ttu-id="5ee09-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="5ee09-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="5ee09-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="5ee09-126">servicePrincipalName</span></span>|<span data-ttu-id="5ee09-127">字符串</span><span class="sxs-lookup"><span data-stu-id="5ee09-127">String</span></span>|<span data-ttu-id="5ee09-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="5ee09-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="5ee09-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="5ee09-129">ipAddress</span></span>|<span data-ttu-id="5ee09-130">String</span><span class="sxs-lookup"><span data-stu-id="5ee09-130">String</span></span>|<span data-ttu-id="5ee09-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="5ee09-131">IPAddress.</span></span>|
|<span data-ttu-id="5ee09-132">userId</span><span class="sxs-lookup"><span data-stu-id="5ee09-132">userId</span></span>|<span data-ttu-id="5ee09-133">String</span><span class="sxs-lookup"><span data-stu-id="5ee09-133">String</span></span>|<span data-ttu-id="5ee09-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="5ee09-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ee09-135">关系</span><span class="sxs-lookup"><span data-stu-id="5ee09-135">Relationships</span></span>
<span data-ttu-id="5ee09-136">无</span><span class="sxs-lookup"><span data-stu-id="5ee09-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ee09-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ee09-137">JSON Representation</span></span>
<span data-ttu-id="5ee09-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ee09-138">Here is a JSON representation of the resource.</span></span>
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




