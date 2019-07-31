---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c1e441b142ef27abbdde4ac613ef8d75848f5001
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966550"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="5158b-103">office365GroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="5158b-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="5158b-104">属性</span><span class="sxs-lookup"><span data-stu-id="5158b-104">Properties</span></span>

| <span data-ttu-id="5158b-105">属性</span><span class="sxs-lookup"><span data-stu-id="5158b-105">Property</span></span>               | <span data-ttu-id="5158b-106">类型</span><span class="sxs-lookup"><span data-stu-id="5158b-106">Type</span></span>   | <span data-ttu-id="5158b-107">说明</span><span class="sxs-lookup"><span data-stu-id="5158b-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="5158b-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5158b-108">reportRefreshDate</span></span>      | <span data-ttu-id="5158b-109">日期</span><span class="sxs-lookup"><span data-stu-id="5158b-109">Date</span></span>   | <span data-ttu-id="5158b-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="5158b-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="5158b-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="5158b-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="5158b-112">Int64</span><span class="sxs-lookup"><span data-stu-id="5158b-112">Int64</span></span>  | <span data-ttu-id="5158b-113">由组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="5158b-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="5158b-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="5158b-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="5158b-115">Int64</span><span class="sxs-lookup"><span data-stu-id="5158b-115">Int64</span></span>  | <span data-ttu-id="5158b-116">发布到 Yammer 组的邮件数。</span><span class="sxs-lookup"><span data-stu-id="5158b-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="5158b-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="5158b-117">yammerMessagesRead</span></span>     | <span data-ttu-id="5158b-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5158b-118">Int64</span></span>  | <span data-ttu-id="5158b-119">Yammer 组中读取的邮件数。</span><span class="sxs-lookup"><span data-stu-id="5158b-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="5158b-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="5158b-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="5158b-121">Int64</span><span class="sxs-lookup"><span data-stu-id="5158b-121">Int64</span></span>  | <span data-ttu-id="5158b-122">Yammer 组中的已赞邮件数。</span><span class="sxs-lookup"><span data-stu-id="5158b-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="5158b-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="5158b-123">reportDate</span></span>             | <span data-ttu-id="5158b-124">日期</span><span class="sxs-lookup"><span data-stu-id="5158b-124">Date</span></span>   | <span data-ttu-id="5158b-125">向组邮箱或邮件中发送了大量电子邮件的日期已在 Yammer 组中投递、读取或赞</span><span class="sxs-lookup"><span data-stu-id="5158b-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="5158b-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5158b-126">reportPeriod</span></span>           | <span data-ttu-id="5158b-127">String</span><span class="sxs-lookup"><span data-stu-id="5158b-127">String</span></span> | <span data-ttu-id="5158b-128">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="5158b-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="5158b-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5158b-129">JSON representation</span></span>

<span data-ttu-id="5158b-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5158b-130">The following is a JSON representation of the resource.</span></span>

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
