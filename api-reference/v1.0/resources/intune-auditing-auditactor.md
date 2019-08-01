---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b2aab468a6638b2e3bb525fd54c6554f5a5694a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032079"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="129c5-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="129c5-103">auditActor resource type</span></span>

> <span data-ttu-id="129c5-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="129c5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="129c5-105">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="129c5-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="129c5-106">属性</span><span class="sxs-lookup"><span data-stu-id="129c5-106">Properties</span></span>
|<span data-ttu-id="129c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="129c5-107">Property</span></span>|<span data-ttu-id="129c5-108">类型</span><span class="sxs-lookup"><span data-stu-id="129c5-108">Type</span></span>|<span data-ttu-id="129c5-109">说明</span><span class="sxs-lookup"><span data-stu-id="129c5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="129c5-110">type</span><span class="sxs-lookup"><span data-stu-id="129c5-110">type</span></span>|<span data-ttu-id="129c5-111">字符串</span><span class="sxs-lookup"><span data-stu-id="129c5-111">String</span></span>|<span data-ttu-id="129c5-112">主角类型。</span><span class="sxs-lookup"><span data-stu-id="129c5-112">Actor Type.</span></span>|
|<span data-ttu-id="129c5-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="129c5-113">userPermissions</span></span>|<span data-ttu-id="129c5-114">String collection</span><span class="sxs-lookup"><span data-stu-id="129c5-114">String collection</span></span>|<span data-ttu-id="129c5-115">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="129c5-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="129c5-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="129c5-116">applicationId</span></span>|<span data-ttu-id="129c5-117">String</span><span class="sxs-lookup"><span data-stu-id="129c5-117">String</span></span>|<span data-ttu-id="129c5-118">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="129c5-118">AAD Application Id.</span></span>|
|<span data-ttu-id="129c5-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="129c5-119">applicationDisplayName</span></span>|<span data-ttu-id="129c5-120">String</span><span class="sxs-lookup"><span data-stu-id="129c5-120">String</span></span>|<span data-ttu-id="129c5-121">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="129c5-121">Name of the Application.</span></span>|
|<span data-ttu-id="129c5-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="129c5-122">userPrincipalName</span></span>|<span data-ttu-id="129c5-123">字符串</span><span class="sxs-lookup"><span data-stu-id="129c5-123">String</span></span>|<span data-ttu-id="129c5-124">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="129c5-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="129c5-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="129c5-125">servicePrincipalName</span></span>|<span data-ttu-id="129c5-126">String</span><span class="sxs-lookup"><span data-stu-id="129c5-126">String</span></span>|<span data-ttu-id="129c5-127">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="129c5-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="129c5-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="129c5-128">ipAddress</span></span>|<span data-ttu-id="129c5-129">String</span><span class="sxs-lookup"><span data-stu-id="129c5-129">String</span></span>|<span data-ttu-id="129c5-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="129c5-130">IPAddress.</span></span>|
|<span data-ttu-id="129c5-131">userId</span><span class="sxs-lookup"><span data-stu-id="129c5-131">userId</span></span>|<span data-ttu-id="129c5-132">String</span><span class="sxs-lookup"><span data-stu-id="129c5-132">String</span></span>|<span data-ttu-id="129c5-133">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="129c5-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="129c5-134">关系</span><span class="sxs-lookup"><span data-stu-id="129c5-134">Relationships</span></span>
<span data-ttu-id="129c5-135">无</span><span class="sxs-lookup"><span data-stu-id="129c5-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="129c5-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="129c5-136">JSON Representation</span></span>
<span data-ttu-id="129c5-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="129c5-137">Here is a JSON representation of the resource.</span></span>
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



