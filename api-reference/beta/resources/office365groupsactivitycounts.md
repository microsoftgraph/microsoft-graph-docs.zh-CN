---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572330"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="6ceff-103">office365GroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ceff-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6ceff-104">属性</span><span class="sxs-lookup"><span data-stu-id="6ceff-104">Properties</span></span>

| <span data-ttu-id="6ceff-105">属性</span><span class="sxs-lookup"><span data-stu-id="6ceff-105">Property</span></span>               | <span data-ttu-id="6ceff-106">类型</span><span class="sxs-lookup"><span data-stu-id="6ceff-106">Type</span></span>   | <span data-ttu-id="6ceff-107">说明</span><span class="sxs-lookup"><span data-stu-id="6ceff-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6ceff-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6ceff-108">reportRefreshDate</span></span>      | <span data-ttu-id="6ceff-109">Date</span><span class="sxs-lookup"><span data-stu-id="6ceff-109">Date</span></span>   | <span data-ttu-id="6ceff-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="6ceff-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="6ceff-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="6ceff-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="6ceff-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6ceff-112">Int64</span></span>  | <span data-ttu-id="6ceff-113">通过组邮箱收到的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="6ceff-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="6ceff-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="6ceff-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="6ceff-115">Int64</span><span class="sxs-lookup"><span data-stu-id="6ceff-115">Int64</span></span>  | <span data-ttu-id="6ceff-116">发布到 Yammer 组的消息数。</span><span class="sxs-lookup"><span data-stu-id="6ceff-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="6ceff-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="6ceff-117">yammerMessagesRead</span></span>     | <span data-ttu-id="6ceff-118">Int64</span><span class="sxs-lookup"><span data-stu-id="6ceff-118">Int64</span></span>  | <span data-ttu-id="6ceff-119">Yammer 组中读取的消息数。</span><span class="sxs-lookup"><span data-stu-id="6ceff-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="6ceff-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="6ceff-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="6ceff-121">Int64</span><span class="sxs-lookup"><span data-stu-id="6ceff-121">Int64</span></span>  | <span data-ttu-id="6ceff-122">喜欢 Yammer 组中的消息数。</span><span class="sxs-lookup"><span data-stu-id="6ceff-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="6ceff-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="6ceff-123">reportDate</span></span>             | <span data-ttu-id="6ceff-124">Date</span><span class="sxs-lookup"><span data-stu-id="6ceff-124">Date</span></span>   | <span data-ttu-id="6ceff-125">大量的电子邮件发送到组邮箱或日期已发布、 读取或喜欢 Yammer 组中的邮件数</span><span class="sxs-lookup"><span data-stu-id="6ceff-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="6ceff-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6ceff-126">reportPeriod</span></span>           | <span data-ttu-id="6ceff-127">String</span><span class="sxs-lookup"><span data-stu-id="6ceff-127">String</span></span> | <span data-ttu-id="6ceff-128">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="6ceff-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6ceff-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ceff-129">JSON representation</span></span>

<span data-ttu-id="6ceff-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ceff-130">The following is a JSON representation of the resource.</span></span>

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
