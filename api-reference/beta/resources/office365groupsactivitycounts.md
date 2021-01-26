---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: a212028e4ba9d38ea38e99c835d89fe1fe7d850b
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980694"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="a81a8-103">office365GroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a81a8-103">office365GroupsActivityCounts resource type</span></span>

<span data-ttu-id="a81a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a81a8-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a81a8-105">属性</span><span class="sxs-lookup"><span data-stu-id="a81a8-105">Properties</span></span>

| <span data-ttu-id="a81a8-106">属性</span><span class="sxs-lookup"><span data-stu-id="a81a8-106">Property</span></span>               | <span data-ttu-id="a81a8-107">类型</span><span class="sxs-lookup"><span data-stu-id="a81a8-107">Type</span></span>   | <span data-ttu-id="a81a8-108">说明</span><span class="sxs-lookup"><span data-stu-id="a81a8-108">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a81a8-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a81a8-109">reportRefreshDate</span></span>      | <span data-ttu-id="a81a8-110">日期</span><span class="sxs-lookup"><span data-stu-id="a81a8-110">Date</span></span>   | <span data-ttu-id="a81a8-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="a81a8-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="a81a8-112">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="a81a8-112">exchangeEmailsReceived</span></span> | <span data-ttu-id="a81a8-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a81a8-113">Int64</span></span>  | <span data-ttu-id="a81a8-114">组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="a81a8-114">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="a81a8-115">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="a81a8-115">yammerMessagesPosted</span></span>   | <span data-ttu-id="a81a8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a81a8-116">Int64</span></span>  | <span data-ttu-id="a81a8-117">张贴到 Yammer 组的消息数。</span><span class="sxs-lookup"><span data-stu-id="a81a8-117">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="a81a8-118">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="a81a8-118">yammerMessagesRead</span></span>     | <span data-ttu-id="a81a8-119">Int64</span><span class="sxs-lookup"><span data-stu-id="a81a8-119">Int64</span></span>  | <span data-ttu-id="a81a8-120">Yammer 组中读取的消息数。</span><span class="sxs-lookup"><span data-stu-id="a81a8-120">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="a81a8-121">yammerMessages在</span><span class="sxs-lookup"><span data-stu-id="a81a8-121">yammerMessagesLiked</span></span>    | <span data-ttu-id="a81a8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a81a8-122">Int64</span></span>  | <span data-ttu-id="a81a8-123">Yammer 组中喜欢的消息数。</span><span class="sxs-lookup"><span data-stu-id="a81a8-123">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="a81a8-124">reportDate</span><span class="sxs-lookup"><span data-stu-id="a81a8-124">reportDate</span></span>             | <span data-ttu-id="a81a8-125">日期</span><span class="sxs-lookup"><span data-stu-id="a81a8-125">Date</span></span>   | <span data-ttu-id="a81a8-126">向组邮箱发送大量电子邮件或 Yammer 组中发布、阅读或喜欢大量邮件的日期</span><span class="sxs-lookup"><span data-stu-id="a81a8-126">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="a81a8-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a81a8-127">reportPeriod</span></span>           | <span data-ttu-id="a81a8-128">String</span><span class="sxs-lookup"><span data-stu-id="a81a8-128">String</span></span> | <span data-ttu-id="a81a8-129">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="a81a8-129">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="a81a8-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a81a8-130">JSON representation</span></span>

<span data-ttu-id="a81a8-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a81a8-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```


