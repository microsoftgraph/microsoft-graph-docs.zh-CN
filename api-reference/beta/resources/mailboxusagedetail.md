---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: pranoychaudhuri
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: bea72f49f1cefc7874d9a5aa7e92e7dcd7caaa71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055230"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="1b6b1-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b6b1-103">mailboxUsageDetail resource type</span></span>

<span data-ttu-id="1b6b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b6b1-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="1b6b1-105">属性</span><span class="sxs-lookup"><span data-stu-id="1b6b1-105">Properties</span></span>

| <span data-ttu-id="1b6b1-106">属性</span><span class="sxs-lookup"><span data-stu-id="1b6b1-106">Property</span></span>                        | <span data-ttu-id="1b6b1-107">类型</span><span class="sxs-lookup"><span data-stu-id="1b6b1-107">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="1b6b1-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1b6b1-108">reportRefreshDate</span></span>               | <span data-ttu-id="1b6b1-109">日期</span><span class="sxs-lookup"><span data-stu-id="1b6b1-109">Date</span></span>    |
| <span data-ttu-id="1b6b1-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b6b1-110">userPrincipalName</span></span>               | <span data-ttu-id="1b6b1-111">String</span><span class="sxs-lookup"><span data-stu-id="1b6b1-111">String</span></span>  |
| <span data-ttu-id="1b6b1-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1b6b1-112">displayName</span></span>                     | <span data-ttu-id="1b6b1-113">String</span><span class="sxs-lookup"><span data-stu-id="1b6b1-113">String</span></span>  |
| <span data-ttu-id="1b6b1-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="1b6b1-114">isDeleted</span></span>                       | <span data-ttu-id="1b6b1-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b6b1-115">Boolean</span></span> |
| <span data-ttu-id="1b6b1-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="1b6b1-116">deletedDate</span></span>                     | <span data-ttu-id="1b6b1-117">日期</span><span class="sxs-lookup"><span data-stu-id="1b6b1-117">Date</span></span>    |
| <span data-ttu-id="1b6b1-118">createdDate</span><span class="sxs-lookup"><span data-stu-id="1b6b1-118">createdDate</span></span>                     | <span data-ttu-id="1b6b1-119">日期</span><span class="sxs-lookup"><span data-stu-id="1b6b1-119">Date</span></span>    |
| <span data-ttu-id="1b6b1-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1b6b1-120">lastActivityDate</span></span>                | <span data-ttu-id="1b6b1-121">日期</span><span class="sxs-lookup"><span data-stu-id="1b6b1-121">Date</span></span>    |
| <span data-ttu-id="1b6b1-122">itemCount</span><span class="sxs-lookup"><span data-stu-id="1b6b1-122">itemCount</span></span>                       | <span data-ttu-id="1b6b1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="1b6b1-123">Int64</span></span>   |
| <span data-ttu-id="1b6b1-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="1b6b1-124">storageUsedInBytes</span></span>              | <span data-ttu-id="1b6b1-125">Int64</span><span class="sxs-lookup"><span data-stu-id="1b6b1-125">Int64</span></span>   |
| <span data-ttu-id="1b6b1-126">deletedItemCount</span><span class="sxs-lookup"><span data-stu-id="1b6b1-126">deletedItemCount</span></span>                | <span data-ttu-id="1b6b1-127">Int64</span><span class="sxs-lookup"><span data-stu-id="1b6b1-127">Int64</span></span>   |
| <span data-ttu-id="1b6b1-128">deletedItemSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="1b6b1-128">deletedItemSizeInBytes</span></span>          | <span data-ttu-id="1b6b1-129">Int64</span><span class="sxs-lookup"><span data-stu-id="1b6b1-129">Int64</span></span>   |
| <span data-ttu-id="1b6b1-130">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="1b6b1-130">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="1b6b1-131">Int64</span><span class="sxs-lookup"><span data-stu-id="1b6b1-131">Int64</span></span>   |
| <span data-ttu-id="1b6b1-132">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="1b6b1-132">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="1b6b1-133">Int64</span><span class="sxs-lookup"><span data-stu-id="1b6b1-133">Int64</span></span>   |
| <span data-ttu-id="1b6b1-134">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="1b6b1-134">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="1b6b1-135">Int64</span><span class="sxs-lookup"><span data-stu-id="1b6b1-135">Int64</span></span>   |
| <span data-ttu-id="1b6b1-136">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1b6b1-136">reportPeriod</span></span>                    | <span data-ttu-id="1b6b1-137">String</span><span class="sxs-lookup"><span data-stu-id="1b6b1-137">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1b6b1-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b6b1-138">JSON representation</span></span>

<span data-ttu-id="1b6b1-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b6b1-139">The following is a JSON representation of the resource.</span></span>

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


