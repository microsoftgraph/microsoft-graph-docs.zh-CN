---
title: office365GroupsActivityCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 4f3a5bf02f5f477ebab036fc9afa5d35a8061138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048262"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="9ddab-103">office365GroupsActivityCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ddab-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="9ddab-104">属性</span><span class="sxs-lookup"><span data-stu-id="9ddab-104">Properties</span></span>

| <span data-ttu-id="9ddab-105">属性</span><span class="sxs-lookup"><span data-stu-id="9ddab-105">Property</span></span>               | <span data-ttu-id="9ddab-106">类型</span><span class="sxs-lookup"><span data-stu-id="9ddab-106">Type</span></span>   | <span data-ttu-id="9ddab-107">说明</span><span class="sxs-lookup"><span data-stu-id="9ddab-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="9ddab-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="9ddab-108">reportRefreshDate</span></span>      | <span data-ttu-id="9ddab-109">日期</span><span class="sxs-lookup"><span data-stu-id="9ddab-109">Date</span></span>   | <span data-ttu-id="9ddab-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="9ddab-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="9ddab-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="9ddab-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="9ddab-112">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddab-112">Int64</span></span>  | <span data-ttu-id="9ddab-113">通过组邮箱收到的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="9ddab-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="9ddab-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="9ddab-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="9ddab-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddab-115">Int64</span></span>  | <span data-ttu-id="9ddab-116">发布到 Yammer 组的消息数。</span><span class="sxs-lookup"><span data-stu-id="9ddab-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="9ddab-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="9ddab-117">yammerMessagesRead</span></span>     | <span data-ttu-id="9ddab-118">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddab-118">Int64</span></span>  | <span data-ttu-id="9ddab-119">Yammer 组中读取的消息数。</span><span class="sxs-lookup"><span data-stu-id="9ddab-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="9ddab-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="9ddab-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="9ddab-121">Int64</span><span class="sxs-lookup"><span data-stu-id="9ddab-121">Int64</span></span>  | <span data-ttu-id="9ddab-122">喜欢 Yammer 组中的消息数。</span><span class="sxs-lookup"><span data-stu-id="9ddab-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="9ddab-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="9ddab-123">reportDate</span></span>             | <span data-ttu-id="9ddab-124">日期</span><span class="sxs-lookup"><span data-stu-id="9ddab-124">Date</span></span>   | <span data-ttu-id="9ddab-125">大量的电子邮件发送到组邮箱或日期已发布、 读取或喜欢 Yammer 组中的邮件数</span><span class="sxs-lookup"><span data-stu-id="9ddab-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="9ddab-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="9ddab-126">reportPeriod</span></span>           | <span data-ttu-id="9ddab-127">字符串</span><span class="sxs-lookup"><span data-stu-id="9ddab-127">String</span></span> | <span data-ttu-id="9ddab-128">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="9ddab-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="9ddab-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ddab-129">JSON representation</span></span>

<span data-ttu-id="9ddab-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ddab-130">The following is a JSON representation of the resource.</span></span>

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
