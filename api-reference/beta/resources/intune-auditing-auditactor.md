---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87cb4219df0d1b6026bee774576324eac7255377
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335247"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="1fb2c-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fb2c-103">auditActor resource type</span></span>

> <span data-ttu-id="1fb2c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fb2c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fb2c-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="1fb2c-107">属性</span><span class="sxs-lookup"><span data-stu-id="1fb2c-107">Properties</span></span>
|<span data-ttu-id="1fb2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="1fb2c-108">Property</span></span>|<span data-ttu-id="1fb2c-109">类型</span><span class="sxs-lookup"><span data-stu-id="1fb2c-109">Type</span></span>|<span data-ttu-id="1fb2c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1fb2c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fb2c-111">type</span><span class="sxs-lookup"><span data-stu-id="1fb2c-111">type</span></span>|<span data-ttu-id="1fb2c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1fb2c-112">String</span></span>|<span data-ttu-id="1fb2c-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-113">Actor Type.</span></span>|
|<span data-ttu-id="1fb2c-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="1fb2c-114">userPermissions</span></span>|<span data-ttu-id="1fb2c-115">String collection</span><span class="sxs-lookup"><span data-stu-id="1fb2c-115">String collection</span></span>|<span data-ttu-id="1fb2c-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="1fb2c-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="1fb2c-117">applicationId</span></span>|<span data-ttu-id="1fb2c-118">String</span><span class="sxs-lookup"><span data-stu-id="1fb2c-118">String</span></span>|<span data-ttu-id="1fb2c-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-119">AAD Application Id.</span></span>|
|<span data-ttu-id="1fb2c-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="1fb2c-120">applicationDisplayName</span></span>|<span data-ttu-id="1fb2c-121">String</span><span class="sxs-lookup"><span data-stu-id="1fb2c-121">String</span></span>|<span data-ttu-id="1fb2c-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-122">Name of the Application.</span></span>|
|<span data-ttu-id="1fb2c-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1fb2c-123">userPrincipalName</span></span>|<span data-ttu-id="1fb2c-124">字符串</span><span class="sxs-lookup"><span data-stu-id="1fb2c-124">String</span></span>|<span data-ttu-id="1fb2c-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="1fb2c-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="1fb2c-126">servicePrincipalName</span></span>|<span data-ttu-id="1fb2c-127">String</span><span class="sxs-lookup"><span data-stu-id="1fb2c-127">String</span></span>|<span data-ttu-id="1fb2c-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="1fb2c-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="1fb2c-129">ipAddress</span></span>|<span data-ttu-id="1fb2c-130">String</span><span class="sxs-lookup"><span data-stu-id="1fb2c-130">String</span></span>|<span data-ttu-id="1fb2c-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-131">IPAddress.</span></span>|
|<span data-ttu-id="1fb2c-132">userId</span><span class="sxs-lookup"><span data-stu-id="1fb2c-132">userId</span></span>|<span data-ttu-id="1fb2c-133">String</span><span class="sxs-lookup"><span data-stu-id="1fb2c-133">String</span></span>|<span data-ttu-id="1fb2c-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fb2c-135">关系</span><span class="sxs-lookup"><span data-stu-id="1fb2c-135">Relationships</span></span>
<span data-ttu-id="1fb2c-136">无</span><span class="sxs-lookup"><span data-stu-id="1fb2c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fb2c-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fb2c-137">JSON Representation</span></span>
<span data-ttu-id="1fb2c-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fb2c-138">Here is a JSON representation of the resource.</span></span>
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



