---
title: mailboxUsageDetail 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: af49fac7c6286c7e9f9ce1e6d7ffdede225b4072
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043127"
---
# <a name="mailboxusagedetail-resource-type"></a><span data-ttu-id="669ba-103">mailboxUsageDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="669ba-103">mailboxUsageDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="669ba-104">属性</span><span class="sxs-lookup"><span data-stu-id="669ba-104">Properties</span></span>

| <span data-ttu-id="669ba-105">属性</span><span class="sxs-lookup"><span data-stu-id="669ba-105">Property</span></span>                        | <span data-ttu-id="669ba-106">类型</span><span class="sxs-lookup"><span data-stu-id="669ba-106">Type</span></span>    |
| :------------------------------ | :------ |
| <span data-ttu-id="669ba-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="669ba-107">reportRefreshDate</span></span>               | <span data-ttu-id="669ba-108">日期</span><span class="sxs-lookup"><span data-stu-id="669ba-108">Date</span></span>    |
| <span data-ttu-id="669ba-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="669ba-109">userPrincipalName</span></span>               | <span data-ttu-id="669ba-110">字符串</span><span class="sxs-lookup"><span data-stu-id="669ba-110">String</span></span>  |
| <span data-ttu-id="669ba-111">displayName</span><span class="sxs-lookup"><span data-stu-id="669ba-111">displayName</span></span>                     | <span data-ttu-id="669ba-112">字符串</span><span class="sxs-lookup"><span data-stu-id="669ba-112">String</span></span>  |
| <span data-ttu-id="669ba-113">被</span><span class="sxs-lookup"><span data-stu-id="669ba-113">isDeleted</span></span>                       | <span data-ttu-id="669ba-114">布尔</span><span class="sxs-lookup"><span data-stu-id="669ba-114">Boolean</span></span> |
| <span data-ttu-id="669ba-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="669ba-115">deletedDate</span></span>                     | <span data-ttu-id="669ba-116">日期</span><span class="sxs-lookup"><span data-stu-id="669ba-116">Date</span></span>    |
| <span data-ttu-id="669ba-117">createdDate</span><span class="sxs-lookup"><span data-stu-id="669ba-117">createdDate</span></span>                     | <span data-ttu-id="669ba-118">日期</span><span class="sxs-lookup"><span data-stu-id="669ba-118">Date</span></span>    |
| <span data-ttu-id="669ba-119">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="669ba-119">lastActivityDate</span></span>                | <span data-ttu-id="669ba-120">日期</span><span class="sxs-lookup"><span data-stu-id="669ba-120">Date</span></span>    |
| <span data-ttu-id="669ba-121">itemCount</span><span class="sxs-lookup"><span data-stu-id="669ba-121">itemCount</span></span>                       | <span data-ttu-id="669ba-122">Int64</span><span class="sxs-lookup"><span data-stu-id="669ba-122">Int64</span></span>   |
| <span data-ttu-id="669ba-123">storageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="669ba-123">storageUsedInBytes</span></span>              | <span data-ttu-id="669ba-124">Int64</span><span class="sxs-lookup"><span data-stu-id="669ba-124">Int64</span></span>   |
| <span data-ttu-id="669ba-125">issueWarningQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="669ba-125">issueWarningQuotaInBytes</span></span>        | <span data-ttu-id="669ba-126">Int64</span><span class="sxs-lookup"><span data-stu-id="669ba-126">Int64</span></span>   |
| <span data-ttu-id="669ba-127">prohibitSendQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="669ba-127">prohibitSendQuotaInBytes</span></span>        | <span data-ttu-id="669ba-128">Int64</span><span class="sxs-lookup"><span data-stu-id="669ba-128">Int64</span></span>   |
| <span data-ttu-id="669ba-129">prohibitSendReceiveQuotaInBytes</span><span class="sxs-lookup"><span data-stu-id="669ba-129">prohibitSendReceiveQuotaInBytes</span></span> | <span data-ttu-id="669ba-130">Int64</span><span class="sxs-lookup"><span data-stu-id="669ba-130">Int64</span></span>   |
| <span data-ttu-id="669ba-131">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="669ba-131">reportPeriod</span></span>                    | <span data-ttu-id="669ba-132">String</span><span class="sxs-lookup"><span data-stu-id="669ba-132">String</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="669ba-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="669ba-133">JSON representation</span></span>

<span data-ttu-id="669ba-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="669ba-134">The following is a JSON representation of the resource.</span></span>

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
