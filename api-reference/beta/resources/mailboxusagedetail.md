---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: sarahwxy
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5b3eb643f74129d481b379d72515dbffaafd336c
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980757"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="0de51-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0de51-103">mailboxUsageDetail resource type</span></span>

<span data-ttu-id="0de51-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0de51-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="0de51-105">属性</span><span class="sxs-lookup"><span data-stu-id="0de51-105">Properties</span></span>

| <span data-ttu-id="0de51-106">属性</span><span class="sxs-lookup"><span data-stu-id="0de51-106">Property</span></span>                        | <span data-ttu-id="0de51-107">类型</span><span class="sxs-lookup"><span data-stu-id="0de51-107">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="0de51-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0de51-108">reportRefreshDate</span></span>               | <span data-ttu-id="0de51-109">日期</span><span class="sxs-lookup"><span data-stu-id="0de51-109">Date</span></span>    |
| <span data-ttu-id="0de51-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0de51-110">userPrincipalName</span></span>               | <span data-ttu-id="0de51-111">String</span><span class="sxs-lookup"><span data-stu-id="0de51-111">String</span></span>  |
| <span data-ttu-id="0de51-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0de51-112">displayName</span></span>                     | <span data-ttu-id="0de51-113">String</span><span class="sxs-lookup"><span data-stu-id="0de51-113">String</span></span>  |
| <span data-ttu-id="0de51-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="0de51-114">isDeleted</span></span>                       | <span data-ttu-id="0de51-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0de51-115">Boolean</span></span> |
| <span data-ttu-id="0de51-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="0de51-116">deletedDate</span></span>                     | <span data-ttu-id="0de51-117">日期</span><span class="sxs-lookup"><span data-stu-id="0de51-117">Date</span></span>    |
| <span data-ttu-id="0de51-118">createdDate</span><span class="sxs-lookup"><span data-stu-id="0de51-118">createdDate</span></span>                     | <span data-ttu-id="0de51-119">日期</span><span class="sxs-lookup"><span data-stu-id="0de51-119">Date</span></span>    |
| <span data-ttu-id="0de51-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="0de51-120">lastActivityDate</span></span>                | <span data-ttu-id="0de51-121">日期</span><span class="sxs-lookup"><span data-stu-id="0de51-121">Date</span></span>    |
| <span data-ttu-id="0de51-122">itemCount</span><span class="sxs-lookup"><span data-stu-id="0de51-122">itemCount</span></span>                       | <span data-ttu-id="0de51-123">Int64</span><span class="sxs-lookup"><span data-stu-id="0de51-123">Int64</span></span>   |
| <span data-ttu-id="0de51-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="0de51-124">storageUsedInBytes</span></span>              | <span data-ttu-id="0de51-125">Int64</span><span class="sxs-lookup"><span data-stu-id="0de51-125">Int64</span></span>   |
| <span data-ttu-id="0de51-126">deletedItemCount</span><span class="sxs-lookup"><span data-stu-id="0de51-126">deletedItemCount</span></span>                | <span data-ttu-id="0de51-127">Int64</span><span class="sxs-lookup"><span data-stu-id="0de51-127">Int64</span></span>   |
| <span data-ttu-id="0de51-128">deletedItemSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="0de51-128">deletedItemSizeInBytes</span></span>          | <span data-ttu-id="0de51-129">Int64</span><span class="sxs-lookup"><span data-stu-id="0de51-129">Int64</span></span>   |
| <span data-ttu-id="0de51-130">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="0de51-130">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="0de51-131">Int64</span><span class="sxs-lookup"><span data-stu-id="0de51-131">Int64</span></span>   |
| <span data-ttu-id="0de51-132">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="0de51-132">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="0de51-133">Int64</span><span class="sxs-lookup"><span data-stu-id="0de51-133">Int64</span></span>   |
| <span data-ttu-id="0de51-134">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="0de51-134">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="0de51-135">Int64</span><span class="sxs-lookup"><span data-stu-id="0de51-135">Int64</span></span>   |
| <span data-ttu-id="0de51-136">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0de51-136">reportPeriod</span></span>                    | <span data-ttu-id="0de51-137">String</span><span class="sxs-lookup"><span data-stu-id="0de51-137">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0de51-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0de51-138">JSON representation</span></span>

<span data-ttu-id="0de51-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0de51-139">The following is a JSON representation of the resource.</span></span>

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


