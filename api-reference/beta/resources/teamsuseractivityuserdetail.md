---
title: teamsUserActivityUserDetail 资源类型
description: 以下是资源 JSON representaion。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913427"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="0f122-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f122-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="0f122-104">属性</span><span class="sxs-lookup"><span data-stu-id="0f122-104">Properties</span></span>

| <span data-ttu-id="0f122-105">属性</span><span class="sxs-lookup"><span data-stu-id="0f122-105">Property</span></span>                | <span data-ttu-id="0f122-106">类型</span><span class="sxs-lookup"><span data-stu-id="0f122-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="0f122-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="0f122-107">reportRefreshDate</span></span>       | <span data-ttu-id="0f122-108">日期</span><span class="sxs-lookup"><span data-stu-id="0f122-108">Date</span></span>              |
| <span data-ttu-id="0f122-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f122-109">userPrincipalName</span></span>       | <span data-ttu-id="0f122-110">字符串</span><span class="sxs-lookup"><span data-stu-id="0f122-110">String</span></span>            |
| <span data-ttu-id="0f122-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="0f122-111">lastActivityDate</span></span>        | <span data-ttu-id="0f122-112">日期</span><span class="sxs-lookup"><span data-stu-id="0f122-112">Date</span></span>              |
| <span data-ttu-id="0f122-113">被</span><span class="sxs-lookup"><span data-stu-id="0f122-113">isDeleted</span></span>               | <span data-ttu-id="0f122-114">布尔</span><span class="sxs-lookup"><span data-stu-id="0f122-114">Boolean</span></span>           |
| <span data-ttu-id="0f122-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="0f122-115">deletedDate</span></span>             | <span data-ttu-id="0f122-116">日期</span><span class="sxs-lookup"><span data-stu-id="0f122-116">Date</span></span>              |
| <span data-ttu-id="0f122-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="0f122-117">assignedProducts</span></span>        | <span data-ttu-id="0f122-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="0f122-118">String collection</span></span> |
| <span data-ttu-id="0f122-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="0f122-119">teamChatMessageCount</span></span>    | <span data-ttu-id="0f122-120">Int64</span><span class="sxs-lookup"><span data-stu-id="0f122-120">Int64</span></span>             |
| <span data-ttu-id="0f122-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="0f122-121">privateChatMessageCount</span></span> | <span data-ttu-id="0f122-122">Int64</span><span class="sxs-lookup"><span data-stu-id="0f122-122">Int64</span></span>             |
| <span data-ttu-id="0f122-123">callCount</span><span class="sxs-lookup"><span data-stu-id="0f122-123">callCount</span></span>               | <span data-ttu-id="0f122-124">Int64</span><span class="sxs-lookup"><span data-stu-id="0f122-124">Int64</span></span>             |
| <span data-ttu-id="0f122-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="0f122-125">meetingCount</span></span>            | <span data-ttu-id="0f122-126">Int64</span><span class="sxs-lookup"><span data-stu-id="0f122-126">Int64</span></span>             |
| <span data-ttu-id="0f122-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="0f122-127">hasOtherAction</span></span>          | <span data-ttu-id="0f122-128">布尔</span><span class="sxs-lookup"><span data-stu-id="0f122-128">Boolean</span></span>           |
| <span data-ttu-id="0f122-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="0f122-129">reportPeriod</span></span>            | <span data-ttu-id="0f122-130">String</span><span class="sxs-lookup"><span data-stu-id="0f122-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="0f122-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f122-131">JSON representation</span></span>

<span data-ttu-id="0f122-132">以下是资源 JSON representaion。</span><span class="sxs-lookup"><span data-stu-id="0f122-132">The following is a JSON representaion of the resource.</span></span>

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
