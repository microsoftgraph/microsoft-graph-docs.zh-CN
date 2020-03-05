---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9c84ee4f36dac10499d553333654635934ca01a6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522860"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="c627c-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c627c-103">mailboxUsageDetail resource type</span></span>

<span data-ttu-id="c627c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c627c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c627c-105">属性</span><span class="sxs-lookup"><span data-stu-id="c627c-105">Properties</span></span>

| <span data-ttu-id="c627c-106">属性</span><span class="sxs-lookup"><span data-stu-id="c627c-106">Property</span></span>                        | <span data-ttu-id="c627c-107">类型</span><span class="sxs-lookup"><span data-stu-id="c627c-107">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="c627c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c627c-108">reportRefreshDate</span></span>               | <span data-ttu-id="c627c-109">日期</span><span class="sxs-lookup"><span data-stu-id="c627c-109">Date</span></span>    |
| <span data-ttu-id="c627c-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c627c-110">userPrincipalName</span></span>               | <span data-ttu-id="c627c-111">String</span><span class="sxs-lookup"><span data-stu-id="c627c-111">String</span></span>  |
| <span data-ttu-id="c627c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c627c-112">displayName</span></span>                     | <span data-ttu-id="c627c-113">String</span><span class="sxs-lookup"><span data-stu-id="c627c-113">String</span></span>  |
| <span data-ttu-id="c627c-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c627c-114">isDeleted</span></span>                       | <span data-ttu-id="c627c-115">布尔</span><span class="sxs-lookup"><span data-stu-id="c627c-115">Boolean</span></span> |
| <span data-ttu-id="c627c-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="c627c-116">deletedDate</span></span>                     | <span data-ttu-id="c627c-117">日期</span><span class="sxs-lookup"><span data-stu-id="c627c-117">Date</span></span>    |
| <span data-ttu-id="c627c-118">createdDate</span><span class="sxs-lookup"><span data-stu-id="c627c-118">createdDate</span></span>                     | <span data-ttu-id="c627c-119">日期</span><span class="sxs-lookup"><span data-stu-id="c627c-119">Date</span></span>    |
| <span data-ttu-id="c627c-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c627c-120">lastActivityDate</span></span>                | <span data-ttu-id="c627c-121">日期</span><span class="sxs-lookup"><span data-stu-id="c627c-121">Date</span></span>    |
| <span data-ttu-id="c627c-122">itemCount</span><span class="sxs-lookup"><span data-stu-id="c627c-122">itemCount</span></span>                       | <span data-ttu-id="c627c-123">Int64</span><span class="sxs-lookup"><span data-stu-id="c627c-123">Int64</span></span>   |
| <span data-ttu-id="c627c-124">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c627c-124">storageUsedInBytes</span></span>              | <span data-ttu-id="c627c-125">Int64</span><span class="sxs-lookup"><span data-stu-id="c627c-125">Int64</span></span>   |
| <span data-ttu-id="c627c-126">deletedItemCount</span><span class="sxs-lookup"><span data-stu-id="c627c-126">deletedItemCount</span></span>                | <span data-ttu-id="c627c-127">Int64</span><span class="sxs-lookup"><span data-stu-id="c627c-127">Int64</span></span>   |
| <span data-ttu-id="c627c-128">deletedItemSizeInBytes</span><span class="sxs-lookup"><span data-stu-id="c627c-128">deletedItemSizeInBytes</span></span>          | <span data-ttu-id="c627c-129">Int64</span><span class="sxs-lookup"><span data-stu-id="c627c-129">Int64</span></span>   |
| <span data-ttu-id="c627c-130">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="c627c-130">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="c627c-131">Int64</span><span class="sxs-lookup"><span data-stu-id="c627c-131">Int64</span></span>   |
| <span data-ttu-id="c627c-132">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="c627c-132">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="c627c-133">Int64</span><span class="sxs-lookup"><span data-stu-id="c627c-133">Int64</span></span>   |
| <span data-ttu-id="c627c-134">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="c627c-134">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="c627c-135">Int64</span><span class="sxs-lookup"><span data-stu-id="c627c-135">Int64</span></span>   |
| <span data-ttu-id="c627c-136">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c627c-136">reportPeriod</span></span>                    | <span data-ttu-id="c627c-137">String</span><span class="sxs-lookup"><span data-stu-id="c627c-137">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c627c-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c627c-138">JSON representation</span></span>

<span data-ttu-id="c627c-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c627c-139">The following is a JSON representation of the resource.</span></span>

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
