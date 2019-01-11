---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 25cb41e38138a677bfc6636b035003bb8fc5858c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818009"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="58c55-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="58c55-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="58c55-104">属性</span><span class="sxs-lookup"><span data-stu-id="58c55-104">Properties</span></span>

| <span data-ttu-id="58c55-105">属性</span><span class="sxs-lookup"><span data-stu-id="58c55-105">Property</span></span>                        | <span data-ttu-id="58c55-106">类型</span><span class="sxs-lookup"><span data-stu-id="58c55-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="58c55-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="58c55-107">reportRefreshDate</span></span>               | <span data-ttu-id="58c55-108">日期</span><span class="sxs-lookup"><span data-stu-id="58c55-108">Date</span></span>    |
| <span data-ttu-id="58c55-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58c55-109">userPrincipalName</span></span>               | <span data-ttu-id="58c55-110">字符串</span><span class="sxs-lookup"><span data-stu-id="58c55-110">String</span></span>  |
| <span data-ttu-id="58c55-111">displayName</span><span class="sxs-lookup"><span data-stu-id="58c55-111">displayName</span></span>                     | <span data-ttu-id="58c55-112">字符串</span><span class="sxs-lookup"><span data-stu-id="58c55-112">String</span></span>  |
| <span data-ttu-id="58c55-113">被</span><span class="sxs-lookup"><span data-stu-id="58c55-113">isDeleted</span></span>                       | <span data-ttu-id="58c55-114">布尔</span><span class="sxs-lookup"><span data-stu-id="58c55-114">Boolean</span></span> |
| <span data-ttu-id="58c55-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="58c55-115">deletedDate</span></span>                     | <span data-ttu-id="58c55-116">日期</span><span class="sxs-lookup"><span data-stu-id="58c55-116">Date</span></span>    |
| <span data-ttu-id="58c55-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="58c55-117">createdDate</span></span>                     | <span data-ttu-id="58c55-118">日期</span><span class="sxs-lookup"><span data-stu-id="58c55-118">Date</span></span>    |
| <span data-ttu-id="58c55-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="58c55-119">lastActivityDate</span></span>                | <span data-ttu-id="58c55-120">日期</span><span class="sxs-lookup"><span data-stu-id="58c55-120">Date</span></span>    |
| <span data-ttu-id="58c55-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="58c55-121">itemCount</span></span>                       | <span data-ttu-id="58c55-122">Int64</span><span class="sxs-lookup"><span data-stu-id="58c55-122">Int64</span></span>   |
| <span data-ttu-id="58c55-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="58c55-123">storageUsedInBytes</span></span>              | <span data-ttu-id="58c55-124">Int64</span><span class="sxs-lookup"><span data-stu-id="58c55-124">Int64</span></span>   |
| <span data-ttu-id="58c55-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="58c55-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="58c55-126">Int64</span><span class="sxs-lookup"><span data-stu-id="58c55-126">Int64</span></span>   |
| <span data-ttu-id="58c55-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="58c55-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="58c55-128">Int64</span><span class="sxs-lookup"><span data-stu-id="58c55-128">Int64</span></span>   |
| <span data-ttu-id="58c55-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="58c55-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="58c55-130">Int64</span><span class="sxs-lookup"><span data-stu-id="58c55-130">Int64</span></span>   |
| <span data-ttu-id="58c55-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="58c55-131">reportPeriod</span></span>                    | <span data-ttu-id="58c55-132">String</span><span class="sxs-lookup"><span data-stu-id="58c55-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="58c55-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58c55-133">JSON representation</span></span>

<span data-ttu-id="58c55-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58c55-134">The following is a JSON representation of the resource.</span></span>

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
  "issueWarningQuotaInBytes": 1024, 
  "prohibitSendQuotaInBytes": 1024, 
  "prohibitSendReceiveQuotaInBytes": 1024, 
  "reportPeriod": "String"
}
```
