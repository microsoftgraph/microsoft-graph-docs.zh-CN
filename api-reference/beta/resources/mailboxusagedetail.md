---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 485dba38275cb437f069abf1309bdc0705ad967a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473477"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="e23ab-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e23ab-103">mailboxUsageDetail resource type</span></span>

<span data-ttu-id="e23ab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e23ab-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e23ab-105">属性</span><span class="sxs-lookup"><span data-stu-id="e23ab-105">Properties</span></span>

| <span data-ttu-id="e23ab-106">属性</span><span class="sxs-lookup"><span data-stu-id="e23ab-106">Property</span></span>                        | <span data-ttu-id="e23ab-107">类型</span><span class="sxs-lookup"><span data-stu-id="e23ab-107">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="e23ab-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e23ab-108">reportRefreshDate</span></span>               | <span data-ttu-id="e23ab-109">日期</span><span class="sxs-lookup"><span data-stu-id="e23ab-109">Date</span></span>    |
| <span data-ttu-id="e23ab-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e23ab-110">userPrincipalName</span></span>               | <span data-ttu-id="e23ab-111">String</span><span class="sxs-lookup"><span data-stu-id="e23ab-111">String</span></span>  |
| <span data-ttu-id="e23ab-112">displayName</span><span class="sxs-lookup"><span data-stu-id="e23ab-112">displayName</span></span>                     | <span data-ttu-id="e23ab-113">String</span><span class="sxs-lookup"><span data-stu-id="e23ab-113">String</span></span>  |
| <span data-ttu-id="e23ab-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="e23ab-114">isDeleted</span></span>                       | <span data-ttu-id="e23ab-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="e23ab-115">Boolean</span></span> |
| <span data-ttu-id="e23ab-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="e23ab-116">deletedDate</span></span>                     | <span data-ttu-id="e23ab-117">日期</span><span class="sxs-lookup"><span data-stu-id="e23ab-117">Date</span></span>    |
| <span data-ttu-id="e23ab-118">createdDate</span><span class="sxs-lookup"><span data-stu-id="e23ab-118">createdDate</span></span>                     | <span data-ttu-id="e23ab-119">日期</span><span class="sxs-lookup"><span data-stu-id="e23ab-119">Date</span></span>    |
| <span data-ttu-id="e23ab-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e23ab-120">lastActivityDate</span></span>                | <span data-ttu-id="e23ab-121">日期</span><span class="sxs-lookup"><span data-stu-id="e23ab-121">Date</span></span>    |
| <span data-ttu-id="e23ab-122">itemCount</span><span class="sxs-lookup"><span data-stu-id="e23ab-122">itemCount</span></span>                       | <span data-ttu-id="e23ab-123">Int64</span><span class="sxs-lookup"><span data-stu-id="e23ab-123">Int64</span></span>   |
| <span data-ttu-id="e23ab-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="e23ab-124">storageUsedInBytes</span></span>              | <span data-ttu-id="e23ab-125">Int64</span><span class="sxs-lookup"><span data-stu-id="e23ab-125">Int64</span></span>   |
| <span data-ttu-id="e23ab-126">deletedItemCount</span><span class="sxs-lookup"><span data-stu-id="e23ab-126">deletedItemCount</span></span>                | <span data-ttu-id="e23ab-127">Int64</span><span class="sxs-lookup"><span data-stu-id="e23ab-127">Int64</span></span>   |
| <span data-ttu-id="e23ab-128">deletedItemSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="e23ab-128">deletedItemSizeInBytes</span></span>          | <span data-ttu-id="e23ab-129">Int64</span><span class="sxs-lookup"><span data-stu-id="e23ab-129">Int64</span></span>   |
| <span data-ttu-id="e23ab-130">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="e23ab-130">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="e23ab-131">Int64</span><span class="sxs-lookup"><span data-stu-id="e23ab-131">Int64</span></span>   |
| <span data-ttu-id="e23ab-132">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="e23ab-132">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="e23ab-133">Int64</span><span class="sxs-lookup"><span data-stu-id="e23ab-133">Int64</span></span>   |
| <span data-ttu-id="e23ab-134">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="e23ab-134">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="e23ab-135">Int64</span><span class="sxs-lookup"><span data-stu-id="e23ab-135">Int64</span></span>   |
| <span data-ttu-id="e23ab-136">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e23ab-136">reportPeriod</span></span>                    | <span data-ttu-id="e23ab-137">String</span><span class="sxs-lookup"><span data-stu-id="e23ab-137">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e23ab-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e23ab-138">JSON representation</span></span>

<span data-ttu-id="e23ab-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e23ab-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailboxUsageDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "createdDate": "Date", 
  "lastActivityDate": "Date", 
  "itemCount": 1024, 
  "storageUsedInBytes": 1024, 
  "deletedItemCount": 1024,
  "deletedItemSizeInBytes": 1024, 
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
