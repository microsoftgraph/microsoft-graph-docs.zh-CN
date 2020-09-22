---
title: teamsUserActivityUserDetail 资源类型
description: 下面是资源的 JSON representaion。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 73208044be5d3612303774f92dfced2302939de8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046354"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="7269f-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="7269f-103">teamsUserActivityUserDetail resource type</span></span>

<span data-ttu-id="7269f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7269f-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="7269f-105">属性</span><span class="sxs-lookup"><span data-stu-id="7269f-105">Properties</span></span>

| <span data-ttu-id="7269f-106">属性</span><span class="sxs-lookup"><span data-stu-id="7269f-106">Property</span></span>                | <span data-ttu-id="7269f-107">类型</span><span class="sxs-lookup"><span data-stu-id="7269f-107">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="7269f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="7269f-108">reportRefreshDate</span></span>       | <span data-ttu-id="7269f-109">日期</span><span class="sxs-lookup"><span data-stu-id="7269f-109">Date</span></span>              |
| <span data-ttu-id="7269f-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7269f-110">userPrincipalName</span></span>       | <span data-ttu-id="7269f-111">String</span><span class="sxs-lookup"><span data-stu-id="7269f-111">String</span></span>            |
| <span data-ttu-id="7269f-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="7269f-112">lastActivityDate</span></span>        | <span data-ttu-id="7269f-113">日期</span><span class="sxs-lookup"><span data-stu-id="7269f-113">Date</span></span>              |
| <span data-ttu-id="7269f-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="7269f-114">isDeleted</span></span>               | <span data-ttu-id="7269f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="7269f-115">Boolean</span></span>           |
| <span data-ttu-id="7269f-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="7269f-116">deletedDate</span></span>             | <span data-ttu-id="7269f-117">日期</span><span class="sxs-lookup"><span data-stu-id="7269f-117">Date</span></span>              |
| <span data-ttu-id="7269f-118">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="7269f-118">assignedProducts</span></span>        | <span data-ttu-id="7269f-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="7269f-119">String collection</span></span> |
| <span data-ttu-id="7269f-120">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="7269f-120">teamChatMessageCount</span></span>    | <span data-ttu-id="7269f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="7269f-121">Int64</span></span>             |
| <span data-ttu-id="7269f-122">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="7269f-122">privateChatMessageCount</span></span> | <span data-ttu-id="7269f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="7269f-123">Int64</span></span>             |
| <span data-ttu-id="7269f-124">callCount</span><span class="sxs-lookup"><span data-stu-id="7269f-124">callCount</span></span>               | <span data-ttu-id="7269f-125">Int64</span><span class="sxs-lookup"><span data-stu-id="7269f-125">Int64</span></span>             |
| <span data-ttu-id="7269f-126">meetingCount</span><span class="sxs-lookup"><span data-stu-id="7269f-126">meetingCount</span></span>            | <span data-ttu-id="7269f-127">Int64</span><span class="sxs-lookup"><span data-stu-id="7269f-127">Int64</span></span>             |
| <span data-ttu-id="7269f-128">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="7269f-128">hasOtherAction</span></span>          | <span data-ttu-id="7269f-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="7269f-129">Boolean</span></span>           |
| <span data-ttu-id="7269f-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="7269f-130">reportPeriod</span></span>            | <span data-ttu-id="7269f-131">String</span><span class="sxs-lookup"><span data-stu-id="7269f-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="7269f-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7269f-132">JSON representation</span></span>

<span data-ttu-id="7269f-133">下面是资源的 JSON representaion。</span><span class="sxs-lookup"><span data-stu-id="7269f-133">The following is a JSON representaion of the resource.</span></span>

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


