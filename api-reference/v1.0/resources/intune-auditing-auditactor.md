---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
ms.openlocfilehash: ae784e5ad16b54c553dadaa75ed5a849b692211f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008536"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="cba4e-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="cba4e-103">auditActor resource type</span></span>

> <span data-ttu-id="cba4e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cba4e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cba4e-105">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="cba4e-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="cba4e-106">属性</span><span class="sxs-lookup"><span data-stu-id="cba4e-106">Properties</span></span>
|<span data-ttu-id="cba4e-107">属性</span><span class="sxs-lookup"><span data-stu-id="cba4e-107">Property</span></span>|<span data-ttu-id="cba4e-108">类型</span><span class="sxs-lookup"><span data-stu-id="cba4e-108">Type</span></span>|<span data-ttu-id="cba4e-109">说明</span><span class="sxs-lookup"><span data-stu-id="cba4e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba4e-110">type</span><span class="sxs-lookup"><span data-stu-id="cba4e-110">type</span></span>|<span data-ttu-id="cba4e-111">String</span><span class="sxs-lookup"><span data-stu-id="cba4e-111">String</span></span>|<span data-ttu-id="cba4e-112">主角类型。</span><span class="sxs-lookup"><span data-stu-id="cba4e-112">Actor Type.</span></span>|
|<span data-ttu-id="cba4e-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="cba4e-113">userPermissions</span></span>|<span data-ttu-id="cba4e-114">String collection</span><span class="sxs-lookup"><span data-stu-id="cba4e-114">String collection</span></span>|<span data-ttu-id="cba4e-115">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="cba4e-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="cba4e-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="cba4e-116">applicationId</span></span>|<span data-ttu-id="cba4e-117">String</span><span class="sxs-lookup"><span data-stu-id="cba4e-117">String</span></span>|<span data-ttu-id="cba4e-118">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="cba4e-118">AAD Application Id.</span></span>|
|<span data-ttu-id="cba4e-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="cba4e-119">applicationDisplayName</span></span>|<span data-ttu-id="cba4e-120">String</span><span class="sxs-lookup"><span data-stu-id="cba4e-120">String</span></span>|<span data-ttu-id="cba4e-121">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="cba4e-121">Name of the Application.</span></span>|
|<span data-ttu-id="cba4e-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cba4e-122">userPrincipalName</span></span>|<span data-ttu-id="cba4e-123">String</span><span class="sxs-lookup"><span data-stu-id="cba4e-123">String</span></span>|<span data-ttu-id="cba4e-124">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="cba4e-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="cba4e-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="cba4e-125">servicePrincipalName</span></span>|<span data-ttu-id="cba4e-126">String</span><span class="sxs-lookup"><span data-stu-id="cba4e-126">String</span></span>|<span data-ttu-id="cba4e-127">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="cba4e-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="cba4e-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="cba4e-128">ipAddress</span></span>|<span data-ttu-id="cba4e-129">String</span><span class="sxs-lookup"><span data-stu-id="cba4e-129">String</span></span>|<span data-ttu-id="cba4e-130">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="cba4e-130">IPAddress.</span></span>|
|<span data-ttu-id="cba4e-131">userId</span><span class="sxs-lookup"><span data-stu-id="cba4e-131">userId</span></span>|<span data-ttu-id="cba4e-132">String</span><span class="sxs-lookup"><span data-stu-id="cba4e-132">String</span></span>|<span data-ttu-id="cba4e-133">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="cba4e-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cba4e-134">关系</span><span class="sxs-lookup"><span data-stu-id="cba4e-134">Relationships</span></span>
<span data-ttu-id="cba4e-135">无</span><span class="sxs-lookup"><span data-stu-id="cba4e-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cba4e-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cba4e-136">JSON Representation</span></span>
<span data-ttu-id="cba4e-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cba4e-137">Here is a JSON representation of the resource.</span></span>
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



