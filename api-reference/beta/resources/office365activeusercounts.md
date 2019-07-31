---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0d0ebd451252766801239e63804b59b9a1747764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966543"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="fca68-103">office365ActiveUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="fca68-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fca68-104">属性</span><span class="sxs-lookup"><span data-stu-id="fca68-104">Properties</span></span>

| <span data-ttu-id="fca68-105">属性</span><span class="sxs-lookup"><span data-stu-id="fca68-105">Property</span></span>          | <span data-ttu-id="fca68-106">类型</span><span class="sxs-lookup"><span data-stu-id="fca68-106">Type</span></span>   | <span data-ttu-id="fca68-107">说明</span><span class="sxs-lookup"><span data-stu-id="fca68-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="fca68-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fca68-108">reportRefreshDate</span></span> | <span data-ttu-id="fca68-109">日期</span><span class="sxs-lookup"><span data-stu-id="fca68-109">Date</span></span>   | <span data-ttu-id="fca68-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="fca68-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="fca68-111">office365</span><span class="sxs-lookup"><span data-stu-id="fca68-111">office365</span></span>         | <span data-ttu-id="fca68-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fca68-112">Int64</span></span>  | <span data-ttu-id="fca68-113">Office 365 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="fca68-113">The number of active users in Office 365.</span></span> <span data-ttu-id="fca68-114">此数目包括 Exchange、OneDrive、SharePoint、Skype For Business、Yammer 和 Microsoft 团队中的所有活动用户。</span><span class="sxs-lookup"><span data-stu-id="fca68-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="fca68-115">您可以在各自的属性说明中查找每个产品的活动用户的定义。</span><span class="sxs-lookup"><span data-stu-id="fca68-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="fca68-116">汇票</span><span class="sxs-lookup"><span data-stu-id="fca68-116">exchange</span></span>          | <span data-ttu-id="fca68-117">Int64</span><span class="sxs-lookup"><span data-stu-id="fca68-117">Int64</span></span>  | <span data-ttu-id="fca68-118">Exchange 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="fca68-118">The number of active users in Exchange.</span></span> <span data-ttu-id="fca68-119">任何可以读取和发送电子邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="fca68-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="fca68-120">For</span><span class="sxs-lookup"><span data-stu-id="fca68-120">oneDrive</span></span>          | <span data-ttu-id="fca68-121">Int64</span><span class="sxs-lookup"><span data-stu-id="fca68-121">Int64</span></span>  | <span data-ttu-id="fca68-122">OneDrive 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="fca68-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="fca68-123">任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="fca68-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="fca68-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="fca68-124">sharePoint</span></span>        | <span data-ttu-id="fca68-125">Int64</span><span class="sxs-lookup"><span data-stu-id="fca68-125">Int64</span></span>  | <span data-ttu-id="fca68-126">SharePoint 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="fca68-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="fca68-127">任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="fca68-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="fca68-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="fca68-128">skypeForBusiness</span></span>  | <span data-ttu-id="fca68-129">Int64</span><span class="sxs-lookup"><span data-stu-id="fca68-129">Int64</span></span>  | <span data-ttu-id="fca68-130">Skype For Business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="fca68-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="fca68-131">任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="fca68-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="fca68-132">yammer</span><span class="sxs-lookup"><span data-stu-id="fca68-132">yammer</span></span>            | <span data-ttu-id="fca68-133">Int64</span><span class="sxs-lookup"><span data-stu-id="fca68-133">Int64</span></span>  | <span data-ttu-id="fca68-134">Yammer 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="fca68-134">The number of active users in Yammer.</span></span> <span data-ttu-id="fca68-135">任何可以发布、阅读或赞邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="fca68-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="fca68-136">协作</span><span class="sxs-lookup"><span data-stu-id="fca68-136">teams</span></span>             | <span data-ttu-id="fca68-137">Int64</span><span class="sxs-lookup"><span data-stu-id="fca68-137">Int64</span></span>  | <span data-ttu-id="fca68-138">Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="fca68-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="fca68-139">任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="fca68-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="fca68-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="fca68-140">reportDate</span></span>        | <span data-ttu-id="fca68-141">日期</span><span class="sxs-lookup"><span data-stu-id="fca68-141">Date</span></span>   | <span data-ttu-id="fca68-142">用户数处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="fca68-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="fca68-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fca68-143">reportPeriod</span></span>      | <span data-ttu-id="fca68-144">String</span><span class="sxs-lookup"><span data-stu-id="fca68-144">String</span></span> | <span data-ttu-id="fca68-145">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="fca68-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="fca68-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fca68-146">JSON representation</span></span>

<span data-ttu-id="fca68-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fca68-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
