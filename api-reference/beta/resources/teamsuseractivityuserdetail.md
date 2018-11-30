---
title: teamsUserActivityUserDetail 资源类型
description: 以下是资源 JSON representaion。
ms.openlocfilehash: 4e40ea4adf07450e6b51555df47579955a2a0286
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048143"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="2af28-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="2af28-103">teamsUserActivityUserDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2af28-104">属性</span><span class="sxs-lookup"><span data-stu-id="2af28-104">Properties</span></span>

| <span data-ttu-id="2af28-105">属性</span><span class="sxs-lookup"><span data-stu-id="2af28-105">Property</span></span>                | <span data-ttu-id="2af28-106">类型</span><span class="sxs-lookup"><span data-stu-id="2af28-106">Type</span></span>              |
| :---------------------- | :---------------- |
| <span data-ttu-id="2af28-107">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2af28-107">reportRefreshDate</span></span>       | <span data-ttu-id="2af28-108">日期</span><span class="sxs-lookup"><span data-stu-id="2af28-108">Date</span></span>              |
| <span data-ttu-id="2af28-109">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2af28-109">userPrincipalName</span></span>       | <span data-ttu-id="2af28-110">字符串</span><span class="sxs-lookup"><span data-stu-id="2af28-110">String</span></span>            |
| <span data-ttu-id="2af28-111">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="2af28-111">lastActivityDate</span></span>        | <span data-ttu-id="2af28-112">日期</span><span class="sxs-lookup"><span data-stu-id="2af28-112">Date</span></span>              |
| <span data-ttu-id="2af28-113">被</span><span class="sxs-lookup"><span data-stu-id="2af28-113">isDeleted</span></span>               | <span data-ttu-id="2af28-114">布尔</span><span class="sxs-lookup"><span data-stu-id="2af28-114">Boolean</span></span>           |
| <span data-ttu-id="2af28-115">deletedDate</span><span class="sxs-lookup"><span data-stu-id="2af28-115">deletedDate</span></span>             | <span data-ttu-id="2af28-116">日期</span><span class="sxs-lookup"><span data-stu-id="2af28-116">Date</span></span>              |
| <span data-ttu-id="2af28-117">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="2af28-117">assignedProducts</span></span>        | <span data-ttu-id="2af28-118">String 集合</span><span class="sxs-lookup"><span data-stu-id="2af28-118">String collection</span></span> |
| <span data-ttu-id="2af28-119">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="2af28-119">teamChatMessageCount</span></span>    | <span data-ttu-id="2af28-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2af28-120">Int64</span></span>             |
| <span data-ttu-id="2af28-121">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="2af28-121">privateChatMessageCount</span></span> | <span data-ttu-id="2af28-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2af28-122">Int64</span></span>             |
| <span data-ttu-id="2af28-123">callCount</span><span class="sxs-lookup"><span data-stu-id="2af28-123">callCount</span></span>               | <span data-ttu-id="2af28-124">Int64</span><span class="sxs-lookup"><span data-stu-id="2af28-124">Int64</span></span>             |
| <span data-ttu-id="2af28-125">meetingCount</span><span class="sxs-lookup"><span data-stu-id="2af28-125">meetingCount</span></span>            | <span data-ttu-id="2af28-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2af28-126">Int64</span></span>             |
| <span data-ttu-id="2af28-127">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="2af28-127">hasOtherAction</span></span>          | <span data-ttu-id="2af28-128">布尔</span><span class="sxs-lookup"><span data-stu-id="2af28-128">Boolean</span></span>           |
| <span data-ttu-id="2af28-129">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2af28-129">reportPeriod</span></span>            | <span data-ttu-id="2af28-130">String</span><span class="sxs-lookup"><span data-stu-id="2af28-130">String</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="2af28-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2af28-131">JSON representation</span></span>

<span data-ttu-id="2af28-132">以下是资源 JSON representaion。</span><span class="sxs-lookup"><span data-stu-id="2af28-132">The following is a JSON representaion of the resource.</span></span>

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
