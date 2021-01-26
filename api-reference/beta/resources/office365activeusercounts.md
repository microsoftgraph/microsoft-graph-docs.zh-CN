---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 67c9b898da9a106685739ebbf78ccef6425c6617
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980736"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="2f0cf-103">office365ActiveUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f0cf-103">office365ActiveUserCounts resource type</span></span>

<span data-ttu-id="2f0cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f0cf-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2f0cf-105">属性</span><span class="sxs-lookup"><span data-stu-id="2f0cf-105">Properties</span></span>

| <span data-ttu-id="2f0cf-106">属性</span><span class="sxs-lookup"><span data-stu-id="2f0cf-106">Property</span></span>          | <span data-ttu-id="2f0cf-107">类型</span><span class="sxs-lookup"><span data-stu-id="2f0cf-107">Type</span></span>   | <span data-ttu-id="2f0cf-108">说明</span><span class="sxs-lookup"><span data-stu-id="2f0cf-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2f0cf-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2f0cf-109">reportRefreshDate</span></span> | <span data-ttu-id="2f0cf-110">日期</span><span class="sxs-lookup"><span data-stu-id="2f0cf-110">Date</span></span>   | <span data-ttu-id="2f0cf-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="2f0cf-112">office365</span><span class="sxs-lookup"><span data-stu-id="2f0cf-112">office365</span></span>         | <span data-ttu-id="2f0cf-113">Int64</span><span class="sxs-lookup"><span data-stu-id="2f0cf-113">Int64</span></span>  | <span data-ttu-id="2f0cf-114">Microsoft 365 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-114">The number of active users in Microsoft 365.</span></span> <span data-ttu-id="2f0cf-115">此数字包括 Exchange、OneDrive、SharePoint、Skype For Business、Yammer 和 Microsoft Teams 的所有活动用户。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-115">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="2f0cf-116">您可以在各自的属性说明中查找每个产品的活动用户的定义。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-116">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="2f0cf-117">exchange</span><span class="sxs-lookup"><span data-stu-id="2f0cf-117">exchange</span></span>          | <span data-ttu-id="2f0cf-118">Int64</span><span class="sxs-lookup"><span data-stu-id="2f0cf-118">Int64</span></span>  | <span data-ttu-id="2f0cf-119">Exchange 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-119">The number of active users in Exchange.</span></span> <span data-ttu-id="2f0cf-120">任何可以阅读和发送电子邮件的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-120">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="2f0cf-121">oneDrive</span><span class="sxs-lookup"><span data-stu-id="2f0cf-121">oneDrive</span></span>          | <span data-ttu-id="2f0cf-122">Int64</span><span class="sxs-lookup"><span data-stu-id="2f0cf-122">Int64</span></span>  | <span data-ttu-id="2f0cf-123">OneDrive 中的活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-123">The number of active users in OneDrive.</span></span> <span data-ttu-id="2f0cf-124">任何在内部或外部查看或编辑文件、共享文件或同步文件的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-124">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="2f0cf-125">sharePoint</span><span class="sxs-lookup"><span data-stu-id="2f0cf-125">sharePoint</span></span>        | <span data-ttu-id="2f0cf-126">Int64</span><span class="sxs-lookup"><span data-stu-id="2f0cf-126">Int64</span></span>  | <span data-ttu-id="2f0cf-127">SharePoint 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-127">The number of active users in SharePoint.</span></span> <span data-ttu-id="2f0cf-128">任何在内部或外部查看或编辑文件、共享文件、同步文件或查看 SharePoint 页面的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="2f0cf-129">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="2f0cf-129">skypeForBusiness</span></span>  | <span data-ttu-id="2f0cf-130">Int64</span><span class="sxs-lookup"><span data-stu-id="2f0cf-130">Int64</span></span>  | <span data-ttu-id="2f0cf-131">Skype For Business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-131">The number of active users in Skype For Business.</span></span> <span data-ttu-id="2f0cf-132">组织或参与会议或加入对等会话的任何用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-132">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="2f0cf-133">yammer</span><span class="sxs-lookup"><span data-stu-id="2f0cf-133">yammer</span></span>            | <span data-ttu-id="2f0cf-134">Int64</span><span class="sxs-lookup"><span data-stu-id="2f0cf-134">Int64</span></span>  | <span data-ttu-id="2f0cf-135">Yammer 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-135">The number of active users in Yammer.</span></span> <span data-ttu-id="2f0cf-136">任何可以发布、阅读或喜欢消息的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-136">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="2f0cf-137">teams</span><span class="sxs-lookup"><span data-stu-id="2f0cf-137">teams</span></span>             | <span data-ttu-id="2f0cf-138">Int64</span><span class="sxs-lookup"><span data-stu-id="2f0cf-138">Int64</span></span>  | <span data-ttu-id="2f0cf-139">Microsoft Teams 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-139">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="2f0cf-140">任何在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的用户均被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-140">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="2f0cf-141">reportDate</span><span class="sxs-lookup"><span data-stu-id="2f0cf-141">reportDate</span></span>        | <span data-ttu-id="2f0cf-142">日期</span><span class="sxs-lookup"><span data-stu-id="2f0cf-142">Date</span></span>   | <span data-ttu-id="2f0cf-143">许多用户处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-143">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="2f0cf-144">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2f0cf-144">reportPeriod</span></span>      | <span data-ttu-id="2f0cf-145">String</span><span class="sxs-lookup"><span data-stu-id="2f0cf-145">String</span></span> | <span data-ttu-id="2f0cf-146">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-146">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2f0cf-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f0cf-147">JSON representation</span></span>

<span data-ttu-id="2f0cf-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f0cf-148">The following is a JSON representation of the resource.</span></span>

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


