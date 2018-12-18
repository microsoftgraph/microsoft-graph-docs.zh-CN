---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: tfitzmac
ms.openlocfilehash: 1b1f3a182aa710564bdf5e134a4ceabf22f3fb71
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348928"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="eb23b-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb23b-103">auditActor resource type</span></span>

> <span data-ttu-id="eb23b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eb23b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb23b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb23b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb23b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb23b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb23b-107">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="eb23b-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="eb23b-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb23b-108">Properties</span></span>
|<span data-ttu-id="eb23b-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb23b-109">Property</span></span>|<span data-ttu-id="eb23b-110">类型</span><span class="sxs-lookup"><span data-stu-id="eb23b-110">Type</span></span>|<span data-ttu-id="eb23b-111">说明</span><span class="sxs-lookup"><span data-stu-id="eb23b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb23b-112">type</span><span class="sxs-lookup"><span data-stu-id="eb23b-112">type</span></span>|<span data-ttu-id="eb23b-113">String</span><span class="sxs-lookup"><span data-stu-id="eb23b-113">String</span></span>|<span data-ttu-id="eb23b-114">主角类型。</span><span class="sxs-lookup"><span data-stu-id="eb23b-114">Actor Type.</span></span>|
|<span data-ttu-id="eb23b-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="eb23b-115">userPermissions</span></span>|<span data-ttu-id="eb23b-116">String collection</span><span class="sxs-lookup"><span data-stu-id="eb23b-116">String collection</span></span>|<span data-ttu-id="eb23b-117">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="eb23b-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="eb23b-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="eb23b-118">applicationId</span></span>|<span data-ttu-id="eb23b-119">String</span><span class="sxs-lookup"><span data-stu-id="eb23b-119">String</span></span>|<span data-ttu-id="eb23b-120">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="eb23b-120">AAD Application Id.</span></span>|
|<span data-ttu-id="eb23b-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="eb23b-121">applicationDisplayName</span></span>|<span data-ttu-id="eb23b-122">String</span><span class="sxs-lookup"><span data-stu-id="eb23b-122">String</span></span>|<span data-ttu-id="eb23b-123">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="eb23b-123">Name of the Application.</span></span>|
|<span data-ttu-id="eb23b-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eb23b-124">userPrincipalName</span></span>|<span data-ttu-id="eb23b-125">String</span><span class="sxs-lookup"><span data-stu-id="eb23b-125">String</span></span>|<span data-ttu-id="eb23b-126">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="eb23b-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="eb23b-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="eb23b-127">servicePrincipalName</span></span>|<span data-ttu-id="eb23b-128">String</span><span class="sxs-lookup"><span data-stu-id="eb23b-128">String</span></span>|<span data-ttu-id="eb23b-129">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="eb23b-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="eb23b-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="eb23b-130">ipAddress</span></span>|<span data-ttu-id="eb23b-131">String</span><span class="sxs-lookup"><span data-stu-id="eb23b-131">String</span></span>|<span data-ttu-id="eb23b-132">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="eb23b-132">IPAddress.</span></span>|
|<span data-ttu-id="eb23b-133">userId</span><span class="sxs-lookup"><span data-stu-id="eb23b-133">userId</span></span>|<span data-ttu-id="eb23b-134">String</span><span class="sxs-lookup"><span data-stu-id="eb23b-134">String</span></span>|<span data-ttu-id="eb23b-135">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="eb23b-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb23b-136">关系</span><span class="sxs-lookup"><span data-stu-id="eb23b-136">Relationships</span></span>
<span data-ttu-id="eb23b-137">无</span><span class="sxs-lookup"><span data-stu-id="eb23b-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb23b-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb23b-138">JSON Representation</span></span>
<span data-ttu-id="eb23b-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb23b-139">Here is a JSON representation of the resource.</span></span>
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





