---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bbc51e4859b005c01b0f8d2cfb2db3ca902d60e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581455"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="6d9c3-103">office365ActiveUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d9c3-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6d9c3-104">属性</span><span class="sxs-lookup"><span data-stu-id="6d9c3-104">Properties</span></span>

| <span data-ttu-id="6d9c3-105">属性</span><span class="sxs-lookup"><span data-stu-id="6d9c3-105">Property</span></span>          | <span data-ttu-id="6d9c3-106">类型</span><span class="sxs-lookup"><span data-stu-id="6d9c3-106">Type</span></span>   | <span data-ttu-id="6d9c3-107">说明</span><span class="sxs-lookup"><span data-stu-id="6d9c3-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6d9c3-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6d9c3-108">reportRefreshDate</span></span> | <span data-ttu-id="6d9c3-109">Date</span><span class="sxs-lookup"><span data-stu-id="6d9c3-109">Date</span></span>   | <span data-ttu-id="6d9c3-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="6d9c3-111">office365</span><span class="sxs-lookup"><span data-stu-id="6d9c3-111">office365</span></span>         | <span data-ttu-id="6d9c3-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6d9c3-112">Int64</span></span>  | <span data-ttu-id="6d9c3-113">Office 365 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-113">The number of active users in Office 365.</span></span> <span data-ttu-id="6d9c3-114">此数目包括 Exchange、OneDrive、SharePoint、Skype for business、Yammer 和 Microsoft 团队中的所有活动用户。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="6d9c3-115">您可以在各自的属性说明中查找每个产品的活动用户的定义。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="6d9c3-116">汇票</span><span class="sxs-lookup"><span data-stu-id="6d9c3-116">exchange</span></span>          | <span data-ttu-id="6d9c3-117">Int64</span><span class="sxs-lookup"><span data-stu-id="6d9c3-117">Int64</span></span>  | <span data-ttu-id="6d9c3-118">Exchange 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-118">The number of active users in Exchange.</span></span> <span data-ttu-id="6d9c3-119">任何可以读取和发送电子邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="6d9c3-120">for</span><span class="sxs-lookup"><span data-stu-id="6d9c3-120">oneDrive</span></span>          | <span data-ttu-id="6d9c3-121">Int64</span><span class="sxs-lookup"><span data-stu-id="6d9c3-121">Int64</span></span>  | <span data-ttu-id="6d9c3-122">OneDrive 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="6d9c3-123">任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="6d9c3-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="6d9c3-124">sharePoint</span></span>        | <span data-ttu-id="6d9c3-125">Int64</span><span class="sxs-lookup"><span data-stu-id="6d9c3-125">Int64</span></span>  | <span data-ttu-id="6d9c3-126">SharePoint 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="6d9c3-127">任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="6d9c3-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="6d9c3-128">skypeForBusiness</span></span>  | <span data-ttu-id="6d9c3-129">Int64</span><span class="sxs-lookup"><span data-stu-id="6d9c3-129">Int64</span></span>  | <span data-ttu-id="6d9c3-130">Skype for business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="6d9c3-131">任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="6d9c3-132">yammer</span><span class="sxs-lookup"><span data-stu-id="6d9c3-132">yammer</span></span>            | <span data-ttu-id="6d9c3-133">Int64</span><span class="sxs-lookup"><span data-stu-id="6d9c3-133">Int64</span></span>  | <span data-ttu-id="6d9c3-134">Yammer 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-134">The number of active users in Yammer.</span></span> <span data-ttu-id="6d9c3-135">任何可以发布、阅读或赞邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="6d9c3-136">协作</span><span class="sxs-lookup"><span data-stu-id="6d9c3-136">teams</span></span>             | <span data-ttu-id="6d9c3-137">Int64</span><span class="sxs-lookup"><span data-stu-id="6d9c3-137">Int64</span></span>  | <span data-ttu-id="6d9c3-138">Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="6d9c3-139">任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="6d9c3-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="6d9c3-140">reportDate</span></span>        | <span data-ttu-id="6d9c3-141">Date</span><span class="sxs-lookup"><span data-stu-id="6d9c3-141">Date</span></span>   | <span data-ttu-id="6d9c3-142">用户数处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="6d9c3-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6d9c3-143">reportPeriod</span></span>      | <span data-ttu-id="6d9c3-144">String</span><span class="sxs-lookup"><span data-stu-id="6d9c3-144">String</span></span> | <span data-ttu-id="6d9c3-145">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6d9c3-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d9c3-146">JSON representation</span></span>

<span data-ttu-id="6d9c3-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d9c3-147">The following is a JSON representation of the resource.</span></span>

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
