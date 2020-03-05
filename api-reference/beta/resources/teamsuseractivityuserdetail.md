---
title: teamsUserActivityUserDetail 资源类型
description: 下面是资源的 JSON representaion。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 237cfc933cbabd628320131866f7bf24ba0195c7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519811"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="70da1-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="70da1-103">teamsUserActivityUserDetail resource type</span></span>

<span data-ttu-id="70da1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="70da1-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="70da1-105">属性</span><span class="sxs-lookup"><span data-stu-id="70da1-105">Properties</span></span>

| <span data-ttu-id="70da1-106">属性</span><span class="sxs-lookup"><span data-stu-id="70da1-106">Property</span></span>                | <span data-ttu-id="70da1-107">类型</span><span class="sxs-lookup"><span data-stu-id="70da1-107">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="70da1-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="70da1-108">reportRefreshDate</span></span>       | <span data-ttu-id="70da1-109">日期</span><span class="sxs-lookup"><span data-stu-id="70da1-109">Date</span></span>              |
| <span data-ttu-id="70da1-110">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70da1-110">userPrincipalName</span></span>       | <span data-ttu-id="70da1-111">String</span><span class="sxs-lookup"><span data-stu-id="70da1-111">String</span></span>            |
| <span data-ttu-id="70da1-112">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="70da1-112">lastActivityDate</span></span>        | <span data-ttu-id="70da1-113">日期</span><span class="sxs-lookup"><span data-stu-id="70da1-113">Date</span></span>              |
| <span data-ttu-id="70da1-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="70da1-114">isDeleted</span></span>               | <span data-ttu-id="70da1-115">布尔</span><span class="sxs-lookup"><span data-stu-id="70da1-115">Boolean</span></span>           |
| <span data-ttu-id="70da1-116">deletedDate</span><span class="sxs-lookup"><span data-stu-id="70da1-116">deletedDate</span></span>             | <span data-ttu-id="70da1-117">日期</span><span class="sxs-lookup"><span data-stu-id="70da1-117">Date</span></span>              |
| <span data-ttu-id="70da1-118">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="70da1-118">assignedProducts</span></span>        | <span data-ttu-id="70da1-119">String 集合</span><span class="sxs-lookup"><span data-stu-id="70da1-119">String collection</span></span> |
| <span data-ttu-id="70da1-120">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="70da1-120">teamChatMessageCount</span></span>    | <span data-ttu-id="70da1-121">Int64</span><span class="sxs-lookup"><span data-stu-id="70da1-121">Int64</span></span>             |
| <span data-ttu-id="70da1-122">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="70da1-122">privateChatMessageCount</span></span> | <span data-ttu-id="70da1-123">Int64</span><span class="sxs-lookup"><span data-stu-id="70da1-123">Int64</span></span>             |
| <span data-ttu-id="70da1-124">callCount</span><span class="sxs-lookup"><span data-stu-id="70da1-124">callCount</span></span>               | <span data-ttu-id="70da1-125">Int64</span><span class="sxs-lookup"><span data-stu-id="70da1-125">Int64</span></span>             |
| <span data-ttu-id="70da1-126">meetingCount</span><span class="sxs-lookup"><span data-stu-id="70da1-126">meetingCount</span></span>            | <span data-ttu-id="70da1-127">Int64</span><span class="sxs-lookup"><span data-stu-id="70da1-127">Int64</span></span>             |
| <span data-ttu-id="70da1-128">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="70da1-128">hasOtherAction</span></span>          | <span data-ttu-id="70da1-129">布尔</span><span class="sxs-lookup"><span data-stu-id="70da1-129">Boolean</span></span>           |
| <span data-ttu-id="70da1-130">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="70da1-130">reportPeriod</span></span>            | <span data-ttu-id="70da1-131">String</span><span class="sxs-lookup"><span data-stu-id="70da1-131">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="70da1-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70da1-132">JSON representation</span></span>

<span data-ttu-id="70da1-133">下面是资源的 JSON representaion。</span><span class="sxs-lookup"><span data-stu-id="70da1-133">The following is a JSON representaion of the resource.</span></span>

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
