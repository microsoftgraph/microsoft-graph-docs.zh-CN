---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb9ededd9d1a2bb93f970f9f0da0c41a248e840
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425797"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="a47e0-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="a47e0-103">auditActor resource type</span></span>

> <span data-ttu-id="a47e0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a47e0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a47e0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a47e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a47e0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a47e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a47e0-107">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="a47e0-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="a47e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="a47e0-108">Properties</span></span>
|<span data-ttu-id="a47e0-109">属性</span><span class="sxs-lookup"><span data-stu-id="a47e0-109">Property</span></span>|<span data-ttu-id="a47e0-110">类型</span><span class="sxs-lookup"><span data-stu-id="a47e0-110">Type</span></span>|<span data-ttu-id="a47e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="a47e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a47e0-112">type</span><span class="sxs-lookup"><span data-stu-id="a47e0-112">type</span></span>|<span data-ttu-id="a47e0-113">String</span><span class="sxs-lookup"><span data-stu-id="a47e0-113">String</span></span>|<span data-ttu-id="a47e0-114">主角类型。</span><span class="sxs-lookup"><span data-stu-id="a47e0-114">Actor Type.</span></span>|
|<span data-ttu-id="a47e0-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="a47e0-115">userPermissions</span></span>|<span data-ttu-id="a47e0-116">String collection</span><span class="sxs-lookup"><span data-stu-id="a47e0-116">String collection</span></span>|<span data-ttu-id="a47e0-117">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="a47e0-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="a47e0-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="a47e0-118">applicationId</span></span>|<span data-ttu-id="a47e0-119">String</span><span class="sxs-lookup"><span data-stu-id="a47e0-119">String</span></span>|<span data-ttu-id="a47e0-120">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="a47e0-120">AAD Application Id.</span></span>|
|<span data-ttu-id="a47e0-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="a47e0-121">applicationDisplayName</span></span>|<span data-ttu-id="a47e0-122">String</span><span class="sxs-lookup"><span data-stu-id="a47e0-122">String</span></span>|<span data-ttu-id="a47e0-123">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="a47e0-123">Name of the Application.</span></span>|
|<span data-ttu-id="a47e0-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a47e0-124">userPrincipalName</span></span>|<span data-ttu-id="a47e0-125">String</span><span class="sxs-lookup"><span data-stu-id="a47e0-125">String</span></span>|<span data-ttu-id="a47e0-126">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="a47e0-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="a47e0-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="a47e0-127">servicePrincipalName</span></span>|<span data-ttu-id="a47e0-128">String</span><span class="sxs-lookup"><span data-stu-id="a47e0-128">String</span></span>|<span data-ttu-id="a47e0-129">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="a47e0-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="a47e0-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="a47e0-130">ipAddress</span></span>|<span data-ttu-id="a47e0-131">String</span><span class="sxs-lookup"><span data-stu-id="a47e0-131">String</span></span>|<span data-ttu-id="a47e0-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="a47e0-132">IPAddress.</span></span>|
|<span data-ttu-id="a47e0-133">userId</span><span class="sxs-lookup"><span data-stu-id="a47e0-133">userId</span></span>|<span data-ttu-id="a47e0-134">String</span><span class="sxs-lookup"><span data-stu-id="a47e0-134">String</span></span>|<span data-ttu-id="a47e0-135">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="a47e0-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a47e0-136">关系</span><span class="sxs-lookup"><span data-stu-id="a47e0-136">Relationships</span></span>
<span data-ttu-id="a47e0-137">无</span><span class="sxs-lookup"><span data-stu-id="a47e0-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a47e0-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a47e0-138">JSON Representation</span></span>
<span data-ttu-id="a47e0-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a47e0-139">Here is a JSON representation of the resource.</span></span>
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




