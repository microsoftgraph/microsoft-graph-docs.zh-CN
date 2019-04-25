---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581721"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="5c569-103">office365GroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5c569-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5c569-104">属性</span><span class="sxs-lookup"><span data-stu-id="5c569-104">Properties</span></span>

| <span data-ttu-id="5c569-105">属性</span><span class="sxs-lookup"><span data-stu-id="5c569-105">Property</span></span>               | <span data-ttu-id="5c569-106">类型</span><span class="sxs-lookup"><span data-stu-id="5c569-106">Type</span></span>   | <span data-ttu-id="5c569-107">说明</span><span class="sxs-lookup"><span data-stu-id="5c569-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="5c569-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5c569-108">reportRefreshDate</span></span>      | <span data-ttu-id="5c569-109">Date</span><span class="sxs-lookup"><span data-stu-id="5c569-109">Date</span></span>   | <span data-ttu-id="5c569-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="5c569-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="5c569-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="5c569-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="5c569-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5c569-112">Int64</span></span>  | <span data-ttu-id="5c569-113">由组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="5c569-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="5c569-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="5c569-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="5c569-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5c569-115">Int64</span></span>  | <span data-ttu-id="5c569-116">发布到 Yammer 组的邮件数。</span><span class="sxs-lookup"><span data-stu-id="5c569-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="5c569-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="5c569-117">yammerMessagesRead</span></span>     | <span data-ttu-id="5c569-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5c569-118">Int64</span></span>  | <span data-ttu-id="5c569-119">Yammer 组中读取的邮件数。</span><span class="sxs-lookup"><span data-stu-id="5c569-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="5c569-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="5c569-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="5c569-121">Int64</span><span class="sxs-lookup"><span data-stu-id="5c569-121">Int64</span></span>  | <span data-ttu-id="5c569-122">Yammer 组中的已赞邮件数。</span><span class="sxs-lookup"><span data-stu-id="5c569-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="5c569-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="5c569-123">reportDate</span></span>             | <span data-ttu-id="5c569-124">Date</span><span class="sxs-lookup"><span data-stu-id="5c569-124">Date</span></span>   | <span data-ttu-id="5c569-125">向组邮箱或邮件中发送了大量电子邮件的日期已在 Yammer 组中投递、读取或赞</span><span class="sxs-lookup"><span data-stu-id="5c569-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="5c569-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5c569-126">reportPeriod</span></span>           | <span data-ttu-id="5c569-127">String</span><span class="sxs-lookup"><span data-stu-id="5c569-127">String</span></span> | <span data-ttu-id="5c569-128">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="5c569-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="5c569-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c569-129">JSON representation</span></span>

<span data-ttu-id="5c569-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c569-130">The following is a JSON representation of the resource.</span></span>

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
