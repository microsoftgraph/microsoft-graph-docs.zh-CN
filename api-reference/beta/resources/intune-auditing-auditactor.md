---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
ms.openlocfilehash: f8a2858854a8efb07cd710c5bccb718dd504a81e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041233"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="000c9-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="000c9-103">auditActor resource type</span></span>

> <span data-ttu-id="000c9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="000c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="000c9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="000c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="000c9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="000c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="000c9-107">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="000c9-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="000c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="000c9-108">Properties</span></span>
|<span data-ttu-id="000c9-109">属性</span><span class="sxs-lookup"><span data-stu-id="000c9-109">Property</span></span>|<span data-ttu-id="000c9-110">类型</span><span class="sxs-lookup"><span data-stu-id="000c9-110">Type</span></span>|<span data-ttu-id="000c9-111">说明</span><span class="sxs-lookup"><span data-stu-id="000c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="000c9-112">type</span><span class="sxs-lookup"><span data-stu-id="000c9-112">type</span></span>|<span data-ttu-id="000c9-113">String</span><span class="sxs-lookup"><span data-stu-id="000c9-113">String</span></span>|<span data-ttu-id="000c9-114">主角类型。</span><span class="sxs-lookup"><span data-stu-id="000c9-114">Actor Type.</span></span>|
|<span data-ttu-id="000c9-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="000c9-115">userPermissions</span></span>|<span data-ttu-id="000c9-116">String collection</span><span class="sxs-lookup"><span data-stu-id="000c9-116">String collection</span></span>|<span data-ttu-id="000c9-117">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="000c9-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="000c9-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="000c9-118">applicationId</span></span>|<span data-ttu-id="000c9-119">String</span><span class="sxs-lookup"><span data-stu-id="000c9-119">String</span></span>|<span data-ttu-id="000c9-120">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="000c9-120">AAD Application Id.</span></span>|
|<span data-ttu-id="000c9-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="000c9-121">applicationDisplayName</span></span>|<span data-ttu-id="000c9-122">String</span><span class="sxs-lookup"><span data-stu-id="000c9-122">String</span></span>|<span data-ttu-id="000c9-123">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="000c9-123">Name of the Application.</span></span>|
|<span data-ttu-id="000c9-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="000c9-124">userPrincipalName</span></span>|<span data-ttu-id="000c9-125">String</span><span class="sxs-lookup"><span data-stu-id="000c9-125">String</span></span>|<span data-ttu-id="000c9-126">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="000c9-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="000c9-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="000c9-127">servicePrincipalName</span></span>|<span data-ttu-id="000c9-128">String</span><span class="sxs-lookup"><span data-stu-id="000c9-128">String</span></span>|<span data-ttu-id="000c9-129">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="000c9-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="000c9-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="000c9-130">ipAddress</span></span>|<span data-ttu-id="000c9-131">String</span><span class="sxs-lookup"><span data-stu-id="000c9-131">String</span></span>|<span data-ttu-id="000c9-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="000c9-132">IPAddress.</span></span>|
|<span data-ttu-id="000c9-133">userId</span><span class="sxs-lookup"><span data-stu-id="000c9-133">userId</span></span>|<span data-ttu-id="000c9-134">String</span><span class="sxs-lookup"><span data-stu-id="000c9-134">String</span></span>|<span data-ttu-id="000c9-135">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="000c9-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="000c9-136">关系</span><span class="sxs-lookup"><span data-stu-id="000c9-136">Relationships</span></span>
<span data-ttu-id="000c9-137">无</span><span class="sxs-lookup"><span data-stu-id="000c9-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="000c9-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="000c9-138">JSON Representation</span></span>
<span data-ttu-id="000c9-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="000c9-139">Here is a JSON representation of the resource.</span></span>
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





