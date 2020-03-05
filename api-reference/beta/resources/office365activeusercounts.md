---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b8e3e90424df29218de7a136e4922df59c4af0b5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522468"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="a95a3-103">office365ActiveUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="a95a3-103">office365ActiveUserCounts resource type</span></span>

<span data-ttu-id="a95a3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a95a3-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a95a3-105">属性</span><span class="sxs-lookup"><span data-stu-id="a95a3-105">Properties</span></span>

| <span data-ttu-id="a95a3-106">属性</span><span class="sxs-lookup"><span data-stu-id="a95a3-106">Property</span></span>          | <span data-ttu-id="a95a3-107">类型</span><span class="sxs-lookup"><span data-stu-id="a95a3-107">Type</span></span>   | <span data-ttu-id="a95a3-108">说明</span><span class="sxs-lookup"><span data-stu-id="a95a3-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a95a3-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a95a3-109">reportRefreshDate</span></span> | <span data-ttu-id="a95a3-110">日期</span><span class="sxs-lookup"><span data-stu-id="a95a3-110">Date</span></span>   | <span data-ttu-id="a95a3-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="a95a3-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="a95a3-112">office365</span><span class="sxs-lookup"><span data-stu-id="a95a3-112">office365</span></span>         | <span data-ttu-id="a95a3-113">Int64</span><span class="sxs-lookup"><span data-stu-id="a95a3-113">Int64</span></span>  | <span data-ttu-id="a95a3-114">Office 365 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-114">The number of active users in Office 365.</span></span> <span data-ttu-id="a95a3-115">此数目包括 Exchange、OneDrive、SharePoint、Skype For Business、Yammer 和 Microsoft 团队中的所有活动用户。</span><span class="sxs-lookup"><span data-stu-id="a95a3-115">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="a95a3-116">您可以在各自的属性说明中查找每个产品的活动用户的定义。</span><span class="sxs-lookup"><span data-stu-id="a95a3-116">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="a95a3-117">汇票</span><span class="sxs-lookup"><span data-stu-id="a95a3-117">exchange</span></span>          | <span data-ttu-id="a95a3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="a95a3-118">Int64</span></span>  | <span data-ttu-id="a95a3-119">Exchange 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-119">The number of active users in Exchange.</span></span> <span data-ttu-id="a95a3-120">任何可以读取和发送电子邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="a95a3-120">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="a95a3-121">For</span><span class="sxs-lookup"><span data-stu-id="a95a3-121">oneDrive</span></span>          | <span data-ttu-id="a95a3-122">Int64</span><span class="sxs-lookup"><span data-stu-id="a95a3-122">Int64</span></span>  | <span data-ttu-id="a95a3-123">OneDrive 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-123">The number of active users in OneDrive.</span></span> <span data-ttu-id="a95a3-124">任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="a95a3-124">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="a95a3-125">sharePoint</span><span class="sxs-lookup"><span data-stu-id="a95a3-125">sharePoint</span></span>        | <span data-ttu-id="a95a3-126">Int64</span><span class="sxs-lookup"><span data-stu-id="a95a3-126">Int64</span></span>  | <span data-ttu-id="a95a3-127">SharePoint 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-127">The number of active users in SharePoint.</span></span> <span data-ttu-id="a95a3-128">任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="a95a3-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="a95a3-129">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="a95a3-129">skypeForBusiness</span></span>  | <span data-ttu-id="a95a3-130">Int64</span><span class="sxs-lookup"><span data-stu-id="a95a3-130">Int64</span></span>  | <span data-ttu-id="a95a3-131">Skype For Business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-131">The number of active users in Skype For Business.</span></span> <span data-ttu-id="a95a3-132">任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="a95a3-132">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="a95a3-133">yammer</span><span class="sxs-lookup"><span data-stu-id="a95a3-133">yammer</span></span>            | <span data-ttu-id="a95a3-134">Int64</span><span class="sxs-lookup"><span data-stu-id="a95a3-134">Int64</span></span>  | <span data-ttu-id="a95a3-135">Yammer 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-135">The number of active users in Yammer.</span></span> <span data-ttu-id="a95a3-136">任何可以发布、阅读或赞邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="a95a3-136">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="a95a3-137">协作</span><span class="sxs-lookup"><span data-stu-id="a95a3-137">teams</span></span>             | <span data-ttu-id="a95a3-138">Int64</span><span class="sxs-lookup"><span data-stu-id="a95a3-138">Int64</span></span>  | <span data-ttu-id="a95a3-139">Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-139">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="a95a3-140">任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="a95a3-140">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="a95a3-141">reportDate</span><span class="sxs-lookup"><span data-stu-id="a95a3-141">reportDate</span></span>        | <span data-ttu-id="a95a3-142">日期</span><span class="sxs-lookup"><span data-stu-id="a95a3-142">Date</span></span>   | <span data-ttu-id="a95a3-143">用户数处于活动状态的日期。</span><span class="sxs-lookup"><span data-stu-id="a95a3-143">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="a95a3-144">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a95a3-144">reportPeriod</span></span>      | <span data-ttu-id="a95a3-145">String</span><span class="sxs-lookup"><span data-stu-id="a95a3-145">String</span></span> | <span data-ttu-id="a95a3-146">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="a95a3-146">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="a95a3-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a95a3-147">JSON representation</span></span>

<span data-ttu-id="a95a3-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a95a3-148">The following is a JSON representation of the resource.</span></span>

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
