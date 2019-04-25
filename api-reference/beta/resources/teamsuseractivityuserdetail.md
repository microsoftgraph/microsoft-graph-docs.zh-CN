---
title: teamsUserActivityUserDetail 资源类型
description: 下面是资源的 JSON representaion。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 32b611ee9ec01b0339389256b8c8dff9eac99fa9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582904"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="5aac2-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="5aac2-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5aac2-104">属性</span><span class="sxs-lookup"><span data-stu-id="5aac2-104">Properties</span></span>

| <span data-ttu-id="5aac2-105">属性</span><span class="sxs-lookup"><span data-stu-id="5aac2-105">Property</span></span>                | <span data-ttu-id="5aac2-106">类型</span><span class="sxs-lookup"><span data-stu-id="5aac2-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="5aac2-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5aac2-107">reportRefreshDate</span></span>       | <span data-ttu-id="5aac2-108">Date</span><span class="sxs-lookup"><span data-stu-id="5aac2-108">Date</span></span>              |
| <span data-ttu-id="5aac2-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5aac2-109">userPrincipalName</span></span>       | <span data-ttu-id="5aac2-110">String</span><span class="sxs-lookup"><span data-stu-id="5aac2-110">String</span></span>            |
| <span data-ttu-id="5aac2-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="5aac2-111">lastActivityDate</span></span>        | <span data-ttu-id="5aac2-112">Date</span><span class="sxs-lookup"><span data-stu-id="5aac2-112">Date</span></span>              |
| <span data-ttu-id="5aac2-113">isDeleted</span><span class="sxs-lookup"><span data-stu-id="5aac2-113">isDeleted</span></span>               | <span data-ttu-id="5aac2-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aac2-114">Boolean</span></span>           |
| <span data-ttu-id="5aac2-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="5aac2-115">deletedDate</span></span>             | <span data-ttu-id="5aac2-116">Date</span><span class="sxs-lookup"><span data-stu-id="5aac2-116">Date</span></span>              |
| <span data-ttu-id="5aac2-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="5aac2-117">assignedProducts</span></span>        | <span data-ttu-id="5aac2-118">String collection</span><span class="sxs-lookup"><span data-stu-id="5aac2-118">String collection</span></span> |
| <span data-ttu-id="5aac2-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="5aac2-119">teamChatMessageCount</span></span>    | <span data-ttu-id="5aac2-120">Int64</span><span class="sxs-lookup"><span data-stu-id="5aac2-120">Int64</span></span>             |
| <span data-ttu-id="5aac2-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="5aac2-121">privateChatMessageCount</span></span> | <span data-ttu-id="5aac2-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5aac2-122">Int64</span></span>             |
| <span data-ttu-id="5aac2-123">callCount</span><span class="sxs-lookup"><span data-stu-id="5aac2-123">callCount</span></span>               | <span data-ttu-id="5aac2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="5aac2-124">Int64</span></span>             |
| <span data-ttu-id="5aac2-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="5aac2-125">meetingCount</span></span>            | <span data-ttu-id="5aac2-126">Int64</span><span class="sxs-lookup"><span data-stu-id="5aac2-126">Int64</span></span>             |
| <span data-ttu-id="5aac2-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="5aac2-127">hasOtherAction</span></span>          | <span data-ttu-id="5aac2-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="5aac2-128">Boolean</span></span>           |
| <span data-ttu-id="5aac2-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5aac2-129">reportPeriod</span></span>            | <span data-ttu-id="5aac2-130">String</span><span class="sxs-lookup"><span data-stu-id="5aac2-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="5aac2-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5aac2-131">JSON representation</span></span>

<span data-ttu-id="5aac2-132">下面是资源的 JSON representaion。</span><span class="sxs-lookup"><span data-stu-id="5aac2-132">The following is a JSON representaion of the resource.</span></span>

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
