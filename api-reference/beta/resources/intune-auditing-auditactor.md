---
title: auditActor 资源类型
description: 包含审核主角的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5fdb804dc293214fbcd7d937adb9ebdf959ea5fa
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538516"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="23c59-103">auditActor 资源类型</span><span class="sxs-lookup"><span data-stu-id="23c59-103">auditActor resource type</span></span>

> <span data-ttu-id="23c59-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23c59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23c59-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23c59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23c59-106">包含审核主角的属性的类。</span><span class="sxs-lookup"><span data-stu-id="23c59-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="23c59-107">属性</span><span class="sxs-lookup"><span data-stu-id="23c59-107">Properties</span></span>
|<span data-ttu-id="23c59-108">属性</span><span class="sxs-lookup"><span data-stu-id="23c59-108">Property</span></span>|<span data-ttu-id="23c59-109">类型</span><span class="sxs-lookup"><span data-stu-id="23c59-109">Type</span></span>|<span data-ttu-id="23c59-110">说明</span><span class="sxs-lookup"><span data-stu-id="23c59-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23c59-111">type</span><span class="sxs-lookup"><span data-stu-id="23c59-111">type</span></span>|<span data-ttu-id="23c59-112">字符串</span><span class="sxs-lookup"><span data-stu-id="23c59-112">String</span></span>|<span data-ttu-id="23c59-113">主角类型。</span><span class="sxs-lookup"><span data-stu-id="23c59-113">Actor Type.</span></span>|
|<span data-ttu-id="23c59-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="23c59-114">userPermissions</span></span>|<span data-ttu-id="23c59-115">String collection</span><span class="sxs-lookup"><span data-stu-id="23c59-115">String collection</span></span>|<span data-ttu-id="23c59-116">执行审核时的用户权限列表。</span><span class="sxs-lookup"><span data-stu-id="23c59-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="23c59-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="23c59-117">applicationId</span></span>|<span data-ttu-id="23c59-118">字符串</span><span class="sxs-lookup"><span data-stu-id="23c59-118">String</span></span>|<span data-ttu-id="23c59-119">AAD 应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="23c59-119">AAD Application Id.</span></span>|
|<span data-ttu-id="23c59-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="23c59-120">applicationDisplayName</span></span>|<span data-ttu-id="23c59-121">字符串</span><span class="sxs-lookup"><span data-stu-id="23c59-121">String</span></span>|<span data-ttu-id="23c59-122">应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="23c59-122">Name of the Application.</span></span>|
|<span data-ttu-id="23c59-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="23c59-123">userPrincipalName</span></span>|<span data-ttu-id="23c59-124">字符串</span><span class="sxs-lookup"><span data-stu-id="23c59-124">String</span></span>|<span data-ttu-id="23c59-125">用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="23c59-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="23c59-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="23c59-126">servicePrincipalName</span></span>|<span data-ttu-id="23c59-127">字符串</span><span class="sxs-lookup"><span data-stu-id="23c59-127">String</span></span>|<span data-ttu-id="23c59-128">服务主体名称 (SPN)。</span><span class="sxs-lookup"><span data-stu-id="23c59-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="23c59-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="23c59-129">ipAddress</span></span>|<span data-ttu-id="23c59-130">String</span><span class="sxs-lookup"><span data-stu-id="23c59-130">String</span></span>|<span data-ttu-id="23c59-131">IPAddress。</span><span class="sxs-lookup"><span data-stu-id="23c59-131">IPAddress.</span></span>|
|<span data-ttu-id="23c59-132">userId</span><span class="sxs-lookup"><span data-stu-id="23c59-132">userId</span></span>|<span data-ttu-id="23c59-133">String</span><span class="sxs-lookup"><span data-stu-id="23c59-133">String</span></span>|<span data-ttu-id="23c59-134">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="23c59-134">User Id.</span></span>|
|<span data-ttu-id="23c59-135">scopeTags</span><span class="sxs-lookup"><span data-stu-id="23c59-135">scopeTags</span></span>|<span data-ttu-id="23c59-136">[scopeTagInfo](../resources/intune-auditing-scopetaginfo.md)集合</span><span class="sxs-lookup"><span data-stu-id="23c59-136">[scopeTagInfo](../resources/intune-auditing-scopetaginfo.md) collection</span></span>|<span data-ttu-id="23c59-137">执行审核时的用户范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="23c59-137">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23c59-138">关系</span><span class="sxs-lookup"><span data-stu-id="23c59-138">Relationships</span></span>
<span data-ttu-id="23c59-139">无</span><span class="sxs-lookup"><span data-stu-id="23c59-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23c59-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23c59-140">JSON Representation</span></span>
<span data-ttu-id="23c59-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23c59-141">Here is a JSON representation of the resource.</span></span>
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
  "userId": "String",
  "scopeTags": [
    {
      "@odata.type": "microsoft.graph.scopeTagInfo",
      "scopeTagName": "String",
      "scopeTagId": "String"
    }
  ]
}
```



