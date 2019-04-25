---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 63b4b997a0ae559338fffd2acfabaa35dcc306e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581266"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="6345a-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="6345a-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6345a-104">属性</span><span class="sxs-lookup"><span data-stu-id="6345a-104">Properties</span></span>

| <span data-ttu-id="6345a-105">属性</span><span class="sxs-lookup"><span data-stu-id="6345a-105">Property</span></span>                        | <span data-ttu-id="6345a-106">类型</span><span class="sxs-lookup"><span data-stu-id="6345a-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="6345a-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6345a-107">reportRefreshDate</span></span>               | <span data-ttu-id="6345a-108">Date</span><span class="sxs-lookup"><span data-stu-id="6345a-108">Date</span></span>    |
| <span data-ttu-id="6345a-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6345a-109">userPrincipalName</span></span>               | <span data-ttu-id="6345a-110">String</span><span class="sxs-lookup"><span data-stu-id="6345a-110">String</span></span>  |
| <span data-ttu-id="6345a-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6345a-111">displayName</span></span>                     | <span data-ttu-id="6345a-112">String</span><span class="sxs-lookup"><span data-stu-id="6345a-112">String</span></span>  |
| <span data-ttu-id="6345a-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="6345a-113">isDeleted</span></span>                       | <span data-ttu-id="6345a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="6345a-114">Boolean</span></span> |
| <span data-ttu-id="6345a-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="6345a-115">deletedDate</span></span>                     | <span data-ttu-id="6345a-116">Date</span><span class="sxs-lookup"><span data-stu-id="6345a-116">Date</span></span>    |
| <span data-ttu-id="6345a-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="6345a-117">createdDate</span></span>                     | <span data-ttu-id="6345a-118">Date</span><span class="sxs-lookup"><span data-stu-id="6345a-118">Date</span></span>    |
| <span data-ttu-id="6345a-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="6345a-119">lastActivityDate</span></span>                | <span data-ttu-id="6345a-120">Date</span><span class="sxs-lookup"><span data-stu-id="6345a-120">Date</span></span>    |
| <span data-ttu-id="6345a-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="6345a-121">itemCount</span></span>                       | <span data-ttu-id="6345a-122">Int64</span><span class="sxs-lookup"><span data-stu-id="6345a-122">Int64</span></span>   |
| <span data-ttu-id="6345a-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="6345a-123">storageUsedInBytes</span></span>              | <span data-ttu-id="6345a-124">Int64</span><span class="sxs-lookup"><span data-stu-id="6345a-124">Int64</span></span>   |
| <span data-ttu-id="6345a-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="6345a-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="6345a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="6345a-126">Int64</span></span>   |
| <span data-ttu-id="6345a-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="6345a-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="6345a-128">Int64</span><span class="sxs-lookup"><span data-stu-id="6345a-128">Int64</span></span>   |
| <span data-ttu-id="6345a-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="6345a-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="6345a-130">Int64</span><span class="sxs-lookup"><span data-stu-id="6345a-130">Int64</span></span>   |
| <span data-ttu-id="6345a-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6345a-131">reportPeriod</span></span>                    | <span data-ttu-id="6345a-132">String</span><span class="sxs-lookup"><span data-stu-id="6345a-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6345a-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6345a-133">JSON representation</span></span>

<span data-ttu-id="6345a-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6345a-134">The following is a JSON representation of the resource.</span></span>

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
