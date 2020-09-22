---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 6c67de6592d32c15e7d64112ce9ac31b6a5d4c41
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092424"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="640c7-103">office365GroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="640c7-103">office365GroupsActivityCounts resource type</span></span>

<span data-ttu-id="640c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="640c7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="640c7-105">属性</span><span class="sxs-lookup"><span data-stu-id="640c7-105">Properties</span></span>

| <span data-ttu-id="640c7-106">属性</span><span class="sxs-lookup"><span data-stu-id="640c7-106">Property</span></span>               | <span data-ttu-id="640c7-107">类型</span><span class="sxs-lookup"><span data-stu-id="640c7-107">Type</span></span>   | <span data-ttu-id="640c7-108">说明</span><span class="sxs-lookup"><span data-stu-id="640c7-108">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="640c7-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="640c7-109">reportRefreshDate</span></span>      | <span data-ttu-id="640c7-110">日期</span><span class="sxs-lookup"><span data-stu-id="640c7-110">Date</span></span>   | <span data-ttu-id="640c7-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="640c7-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="640c7-112">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="640c7-112">exchangeEmailsReceived</span></span> | <span data-ttu-id="640c7-113">Int64</span><span class="sxs-lookup"><span data-stu-id="640c7-113">Int64</span></span>  | <span data-ttu-id="640c7-114">由组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="640c7-114">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="640c7-115">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="640c7-115">yammerMessagesPosted</span></span>   | <span data-ttu-id="640c7-116">Int64</span><span class="sxs-lookup"><span data-stu-id="640c7-116">Int64</span></span>  | <span data-ttu-id="640c7-117">发布到 Yammer 组的邮件数。</span><span class="sxs-lookup"><span data-stu-id="640c7-117">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="640c7-118">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="640c7-118">yammerMessagesRead</span></span>     | <span data-ttu-id="640c7-119">Int64</span><span class="sxs-lookup"><span data-stu-id="640c7-119">Int64</span></span>  | <span data-ttu-id="640c7-120">Yammer 组中读取的邮件数。</span><span class="sxs-lookup"><span data-stu-id="640c7-120">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="640c7-121">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="640c7-121">yammerMessagesLiked</span></span>    | <span data-ttu-id="640c7-122">Int64</span><span class="sxs-lookup"><span data-stu-id="640c7-122">Int64</span></span>  | <span data-ttu-id="640c7-123">Yammer 组中的已赞邮件数。</span><span class="sxs-lookup"><span data-stu-id="640c7-123">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="640c7-124">reportDate</span><span class="sxs-lookup"><span data-stu-id="640c7-124">reportDate</span></span>             | <span data-ttu-id="640c7-125">日期</span><span class="sxs-lookup"><span data-stu-id="640c7-125">Date</span></span>   | <span data-ttu-id="640c7-126">向组邮箱或邮件中发送了大量电子邮件的日期已在 Yammer 组中投递、读取或赞</span><span class="sxs-lookup"><span data-stu-id="640c7-126">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="640c7-127">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="640c7-127">reportPeriod</span></span>           | <span data-ttu-id="640c7-128">字符串</span><span class="sxs-lookup"><span data-stu-id="640c7-128">String</span></span> | <span data-ttu-id="640c7-129">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="640c7-129">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="640c7-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="640c7-130">JSON representation</span></span>

<span data-ttu-id="640c7-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="640c7-131">The following is a JSON representation of the resource.</span></span>

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


