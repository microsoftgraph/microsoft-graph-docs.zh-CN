---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: tfitzmac
ms.openlocfilehash: de2fc78bcc02565da102beb57c077646effc443b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325016"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="541ba-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="541ba-103">auditActor resource type</span></span>

> <span data-ttu-id="541ba-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="541ba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="541ba-105">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="541ba-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="541ba-106">属性</span><span class="sxs-lookup"><span data-stu-id="541ba-106">Properties</span></span>
|<span data-ttu-id="541ba-107">属性</span><span class="sxs-lookup"><span data-stu-id="541ba-107">Property</span></span>|<span data-ttu-id="541ba-108">类型</span><span class="sxs-lookup"><span data-stu-id="541ba-108">Type</span></span>|<span data-ttu-id="541ba-109">说明</span><span class="sxs-lookup"><span data-stu-id="541ba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="541ba-110">type</span><span class="sxs-lookup"><span data-stu-id="541ba-110">type</span></span>|<span data-ttu-id="541ba-111">String</span><span class="sxs-lookup"><span data-stu-id="541ba-111">String</span></span>|<span data-ttu-id="541ba-112">主角类型。</span><span class="sxs-lookup"><span data-stu-id="541ba-112">Actor Type.</span></span>|
|<span data-ttu-id="541ba-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="541ba-113">userPermissions</span></span>|<span data-ttu-id="541ba-114">String collection</span><span class="sxs-lookup"><span data-stu-id="541ba-114">String collection</span></span>|<span data-ttu-id="541ba-115">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="541ba-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="541ba-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="541ba-116">applicationId</span></span>|<span data-ttu-id="541ba-117">String</span><span class="sxs-lookup"><span data-stu-id="541ba-117">String</span></span>|<span data-ttu-id="541ba-118">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="541ba-118">AAD Application Id.</span></span>|
|<span data-ttu-id="541ba-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="541ba-119">applicationDisplayName</span></span>|<span data-ttu-id="541ba-120">String</span><span class="sxs-lookup"><span data-stu-id="541ba-120">String</span></span>|<span data-ttu-id="541ba-121">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="541ba-121">Name of the Application.</span></span>|
|<span data-ttu-id="541ba-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="541ba-122">userPrincipalName</span></span>|<span data-ttu-id="541ba-123">String</span><span class="sxs-lookup"><span data-stu-id="541ba-123">String</span></span>|<span data-ttu-id="541ba-124">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="541ba-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="541ba-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="541ba-125">servicePrincipalName</span></span>|<span data-ttu-id="541ba-126">String</span><span class="sxs-lookup"><span data-stu-id="541ba-126">String</span></span>|<span data-ttu-id="541ba-127">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="541ba-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="541ba-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="541ba-128">ipAddress</span></span>|<span data-ttu-id="541ba-129">String</span><span class="sxs-lookup"><span data-stu-id="541ba-129">String</span></span>|<span data-ttu-id="541ba-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="541ba-130">IPAddress.</span></span>|
|<span data-ttu-id="541ba-131">userId</span><span class="sxs-lookup"><span data-stu-id="541ba-131">userId</span></span>|<span data-ttu-id="541ba-132">String</span><span class="sxs-lookup"><span data-stu-id="541ba-132">String</span></span>|<span data-ttu-id="541ba-133">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="541ba-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="541ba-134">关系</span><span class="sxs-lookup"><span data-stu-id="541ba-134">Relationships</span></span>
<span data-ttu-id="541ba-135">无</span><span class="sxs-lookup"><span data-stu-id="541ba-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="541ba-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="541ba-136">JSON Representation</span></span>
<span data-ttu-id="541ba-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="541ba-137">Here is a JSON representation of the resource.</span></span>
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



