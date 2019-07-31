---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: e630a64e7ece98d956a5f3821ec92413512fc7e4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966935"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="03fc3-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="03fc3-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="03fc3-104">属性</span><span class="sxs-lookup"><span data-stu-id="03fc3-104">Properties</span></span>

| <span data-ttu-id="03fc3-105">属性</span><span class="sxs-lookup"><span data-stu-id="03fc3-105">Property</span></span>                        | <span data-ttu-id="03fc3-106">类型</span><span class="sxs-lookup"><span data-stu-id="03fc3-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="03fc3-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="03fc3-107">reportRefreshDate</span></span>               | <span data-ttu-id="03fc3-108">日期</span><span class="sxs-lookup"><span data-stu-id="03fc3-108">Date</span></span>    |
| <span data-ttu-id="03fc3-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03fc3-109">userPrincipalName</span></span>               | <span data-ttu-id="03fc3-110">String</span><span class="sxs-lookup"><span data-stu-id="03fc3-110">String</span></span>  |
| <span data-ttu-id="03fc3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="03fc3-111">displayName</span></span>                     | <span data-ttu-id="03fc3-112">String</span><span class="sxs-lookup"><span data-stu-id="03fc3-112">String</span></span>  |
| <span data-ttu-id="03fc3-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="03fc3-113">isDeleted</span></span>                       | <span data-ttu-id="03fc3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="03fc3-114">Boolean</span></span> |
| <span data-ttu-id="03fc3-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="03fc3-115">deletedDate</span></span>                     | <span data-ttu-id="03fc3-116">日期</span><span class="sxs-lookup"><span data-stu-id="03fc3-116">Date</span></span>    |
| <span data-ttu-id="03fc3-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="03fc3-117">createdDate</span></span>                     | <span data-ttu-id="03fc3-118">日期</span><span class="sxs-lookup"><span data-stu-id="03fc3-118">Date</span></span>    |
| <span data-ttu-id="03fc3-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="03fc3-119">lastActivityDate</span></span>                | <span data-ttu-id="03fc3-120">日期</span><span class="sxs-lookup"><span data-stu-id="03fc3-120">Date</span></span>    |
| <span data-ttu-id="03fc3-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="03fc3-121">itemCount</span></span>                       | <span data-ttu-id="03fc3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="03fc3-122">Int64</span></span>   |
| <span data-ttu-id="03fc3-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="03fc3-123">storageUsedInBytes</span></span>              | <span data-ttu-id="03fc3-124">Int64</span><span class="sxs-lookup"><span data-stu-id="03fc3-124">Int64</span></span>   |
| <span data-ttu-id="03fc3-125">deletedItemCount</span><span class="sxs-lookup"><span data-stu-id="03fc3-125">deletedItemCount</span></span>                | <span data-ttu-id="03fc3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="03fc3-126">Int64</span></span>   |
| <span data-ttu-id="03fc3-127">deletedItemSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="03fc3-127">deletedItemSizeInBytes</span></span>          | <span data-ttu-id="03fc3-128">Int64</span><span class="sxs-lookup"><span data-stu-id="03fc3-128">Int64</span></span>   |
| <span data-ttu-id="03fc3-129">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="03fc3-129">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="03fc3-130">Int64</span><span class="sxs-lookup"><span data-stu-id="03fc3-130">Int64</span></span>   |
| <span data-ttu-id="03fc3-131">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="03fc3-131">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="03fc3-132">Int64</span><span class="sxs-lookup"><span data-stu-id="03fc3-132">Int64</span></span>   |
| <span data-ttu-id="03fc3-133">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="03fc3-133">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="03fc3-134">Int64</span><span class="sxs-lookup"><span data-stu-id="03fc3-134">Int64</span></span>   |
| <span data-ttu-id="03fc3-135">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="03fc3-135">reportPeriod</span></span>                    | <span data-ttu-id="03fc3-136">String</span><span class="sxs-lookup"><span data-stu-id="03fc3-136">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="03fc3-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03fc3-137">JSON representation</span></span>

<span data-ttu-id="03fc3-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03fc3-138">The following is a JSON representation of the resource.</span></span>

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
