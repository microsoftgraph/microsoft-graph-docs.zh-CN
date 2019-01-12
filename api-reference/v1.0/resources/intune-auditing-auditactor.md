---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba63fd04d917a464933e749622a5abf959c2859e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948700"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="f8a4a-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="f8a4a-103">auditActor resource type</span></span>

> <span data-ttu-id="f8a4a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8a4a-105">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="f8a4a-106">属性</span><span class="sxs-lookup"><span data-stu-id="f8a4a-106">Properties</span></span>
|<span data-ttu-id="f8a4a-107">属性</span><span class="sxs-lookup"><span data-stu-id="f8a4a-107">Property</span></span>|<span data-ttu-id="f8a4a-108">类型</span><span class="sxs-lookup"><span data-stu-id="f8a4a-108">Type</span></span>|<span data-ttu-id="f8a4a-109">说明</span><span class="sxs-lookup"><span data-stu-id="f8a4a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8a4a-110">type</span><span class="sxs-lookup"><span data-stu-id="f8a4a-110">type</span></span>|<span data-ttu-id="f8a4a-111">String</span><span class="sxs-lookup"><span data-stu-id="f8a4a-111">String</span></span>|<span data-ttu-id="f8a4a-112">主角类型。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-112">Actor Type.</span></span>|
|<span data-ttu-id="f8a4a-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="f8a4a-113">userPermissions</span></span>|<span data-ttu-id="f8a4a-114">String collection</span><span class="sxs-lookup"><span data-stu-id="f8a4a-114">String collection</span></span>|<span data-ttu-id="f8a4a-115">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="f8a4a-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="f8a4a-116">applicationId</span></span>|<span data-ttu-id="f8a4a-117">String</span><span class="sxs-lookup"><span data-stu-id="f8a4a-117">String</span></span>|<span data-ttu-id="f8a4a-118">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-118">AAD Application Id.</span></span>|
|<span data-ttu-id="f8a4a-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f8a4a-119">applicationDisplayName</span></span>|<span data-ttu-id="f8a4a-120">String</span><span class="sxs-lookup"><span data-stu-id="f8a4a-120">String</span></span>|<span data-ttu-id="f8a4a-121">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-121">Name of the Application.</span></span>|
|<span data-ttu-id="f8a4a-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8a4a-122">userPrincipalName</span></span>|<span data-ttu-id="f8a4a-123">String</span><span class="sxs-lookup"><span data-stu-id="f8a4a-123">String</span></span>|<span data-ttu-id="f8a4a-124">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="f8a4a-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f8a4a-125">servicePrincipalName</span></span>|<span data-ttu-id="f8a4a-126">String</span><span class="sxs-lookup"><span data-stu-id="f8a4a-126">String</span></span>|<span data-ttu-id="f8a4a-127">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="f8a4a-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f8a4a-128">ipAddress</span></span>|<span data-ttu-id="f8a4a-129">String</span><span class="sxs-lookup"><span data-stu-id="f8a4a-129">String</span></span>|<span data-ttu-id="f8a4a-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-130">IPAddress.</span></span>|
|<span data-ttu-id="f8a4a-131">userId</span><span class="sxs-lookup"><span data-stu-id="f8a4a-131">userId</span></span>|<span data-ttu-id="f8a4a-132">String</span><span class="sxs-lookup"><span data-stu-id="f8a4a-132">String</span></span>|<span data-ttu-id="f8a4a-133">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f8a4a-134">关系</span><span class="sxs-lookup"><span data-stu-id="f8a4a-134">Relationships</span></span>
<span data-ttu-id="f8a4a-135">无</span><span class="sxs-lookup"><span data-stu-id="f8a4a-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f8a4a-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8a4a-136">JSON Representation</span></span>
<span data-ttu-id="f8a4a-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8a4a-137">Here is a JSON representation of the resource.</span></span>
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



