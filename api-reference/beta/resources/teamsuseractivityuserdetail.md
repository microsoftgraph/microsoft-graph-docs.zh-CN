---
title: teamsUserActivityUserDetail 资源类型
description: 以下是资源 JSON representaion。
author: nkramer
ms.openlocfilehash: a1f47bc52c2a0a613598ce663f16023dce208c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331939"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="e6ad7-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6ad7-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="e6ad7-104">属性</span><span class="sxs-lookup"><span data-stu-id="e6ad7-104">Properties</span></span>

| <span data-ttu-id="e6ad7-105">属性</span><span class="sxs-lookup"><span data-stu-id="e6ad7-105">Property</span></span>                | <span data-ttu-id="e6ad7-106">类型</span><span class="sxs-lookup"><span data-stu-id="e6ad7-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="e6ad7-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e6ad7-107">reportRefreshDate</span></span>       | <span data-ttu-id="e6ad7-108">日期</span><span class="sxs-lookup"><span data-stu-id="e6ad7-108">Date</span></span>              |
| <span data-ttu-id="e6ad7-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6ad7-109">userPrincipalName</span></span>       | <span data-ttu-id="e6ad7-110">字符串</span><span class="sxs-lookup"><span data-stu-id="e6ad7-110">String</span></span>            |
| <span data-ttu-id="e6ad7-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="e6ad7-111">lastActivityDate</span></span>        | <span data-ttu-id="e6ad7-112">日期</span><span class="sxs-lookup"><span data-stu-id="e6ad7-112">Date</span></span>              |
| <span data-ttu-id="e6ad7-113">被</span><span class="sxs-lookup"><span data-stu-id="e6ad7-113">isDeleted</span></span>               | <span data-ttu-id="e6ad7-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6ad7-114">Boolean</span></span>           |
| <span data-ttu-id="e6ad7-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="e6ad7-115">deletedDate</span></span>             | <span data-ttu-id="e6ad7-116">日期</span><span class="sxs-lookup"><span data-stu-id="e6ad7-116">Date</span></span>              |
| <span data-ttu-id="e6ad7-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="e6ad7-117">assignedProducts</span></span>        | <span data-ttu-id="e6ad7-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6ad7-118">String collection</span></span> |
| <span data-ttu-id="e6ad7-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="e6ad7-119">teamChatMessageCount</span></span>    | <span data-ttu-id="e6ad7-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e6ad7-120">Int64</span></span>             |
| <span data-ttu-id="e6ad7-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="e6ad7-121">privateChatMessageCount</span></span> | <span data-ttu-id="e6ad7-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e6ad7-122">Int64</span></span>             |
| <span data-ttu-id="e6ad7-123">callCount</span><span class="sxs-lookup"><span data-stu-id="e6ad7-123">callCount</span></span>               | <span data-ttu-id="e6ad7-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e6ad7-124">Int64</span></span>             |
| <span data-ttu-id="e6ad7-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="e6ad7-125">meetingCount</span></span>            | <span data-ttu-id="e6ad7-126">Int64</span><span class="sxs-lookup"><span data-stu-id="e6ad7-126">Int64</span></span>             |
| <span data-ttu-id="e6ad7-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="e6ad7-127">hasOtherAction</span></span>          | <span data-ttu-id="e6ad7-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6ad7-128">Boolean</span></span>           |
| <span data-ttu-id="e6ad7-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e6ad7-129">reportPeriod</span></span>            | <span data-ttu-id="e6ad7-130">String</span><span class="sxs-lookup"><span data-stu-id="e6ad7-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="e6ad7-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6ad7-131">JSON representation</span></span>

<span data-ttu-id="e6ad7-132">以下是资源 JSON representaion。</span><span class="sxs-lookup"><span data-stu-id="e6ad7-132">The following is a JSON representaion of the resource.</span></span>

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
