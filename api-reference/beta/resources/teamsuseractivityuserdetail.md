---
title: teamsUserActivityUserDetail 资源类型
description: 以下是资源 JSON representaion。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 2e3f64c7065343712f6a9d9c6a114bf95f24c171
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823651"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="1baf0-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="1baf0-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="1baf0-104">属性</span><span class="sxs-lookup"><span data-stu-id="1baf0-104">Properties</span></span>

| <span data-ttu-id="1baf0-105">属性</span><span class="sxs-lookup"><span data-stu-id="1baf0-105">Property</span></span>                | <span data-ttu-id="1baf0-106">类型</span><span class="sxs-lookup"><span data-stu-id="1baf0-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="1baf0-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="1baf0-107">reportRefreshDate</span></span>       | <span data-ttu-id="1baf0-108">日期</span><span class="sxs-lookup"><span data-stu-id="1baf0-108">Date</span></span>              |
| <span data-ttu-id="1baf0-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1baf0-109">userPrincipalName</span></span>       | <span data-ttu-id="1baf0-110">字符串</span><span class="sxs-lookup"><span data-stu-id="1baf0-110">String</span></span>            |
| <span data-ttu-id="1baf0-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="1baf0-111">lastActivityDate</span></span>        | <span data-ttu-id="1baf0-112">日期</span><span class="sxs-lookup"><span data-stu-id="1baf0-112">Date</span></span>              |
| <span data-ttu-id="1baf0-113">被</span><span class="sxs-lookup"><span data-stu-id="1baf0-113">isDeleted</span></span>               | <span data-ttu-id="1baf0-114">布尔</span><span class="sxs-lookup"><span data-stu-id="1baf0-114">Boolean</span></span>           |
| <span data-ttu-id="1baf0-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="1baf0-115">deletedDate</span></span>             | <span data-ttu-id="1baf0-116">日期</span><span class="sxs-lookup"><span data-stu-id="1baf0-116">Date</span></span>              |
| <span data-ttu-id="1baf0-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="1baf0-117">assignedProducts</span></span>        | <span data-ttu-id="1baf0-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="1baf0-118">String collection</span></span> |
| <span data-ttu-id="1baf0-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="1baf0-119">teamChatMessageCount</span></span>    | <span data-ttu-id="1baf0-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1baf0-120">Int64</span></span>             |
| <span data-ttu-id="1baf0-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="1baf0-121">privateChatMessageCount</span></span> | <span data-ttu-id="1baf0-122">Int64</span><span class="sxs-lookup"><span data-stu-id="1baf0-122">Int64</span></span>             |
| <span data-ttu-id="1baf0-123">callCount</span><span class="sxs-lookup"><span data-stu-id="1baf0-123">callCount</span></span>               | <span data-ttu-id="1baf0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="1baf0-124">Int64</span></span>             |
| <span data-ttu-id="1baf0-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="1baf0-125">meetingCount</span></span>            | <span data-ttu-id="1baf0-126">Int64</span><span class="sxs-lookup"><span data-stu-id="1baf0-126">Int64</span></span>             |
| <span data-ttu-id="1baf0-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="1baf0-127">hasOtherAction</span></span>          | <span data-ttu-id="1baf0-128">布尔</span><span class="sxs-lookup"><span data-stu-id="1baf0-128">Boolean</span></span>           |
| <span data-ttu-id="1baf0-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="1baf0-129">reportPeriod</span></span>            | <span data-ttu-id="1baf0-130">String</span><span class="sxs-lookup"><span data-stu-id="1baf0-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="1baf0-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1baf0-131">JSON representation</span></span>

<span data-ttu-id="1baf0-132">以下是资源 JSON representaion。</span><span class="sxs-lookup"><span data-stu-id="1baf0-132">The following is a JSON representaion of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```
