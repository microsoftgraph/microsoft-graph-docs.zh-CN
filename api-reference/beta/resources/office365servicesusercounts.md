---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 0deb5eceb31ca3453c1cc5f29ae669f7053738c9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522419"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="2e5aa-103">office365ServicesUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e5aa-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="2e5aa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2e5aa-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="2e5aa-105">属性</span><span class="sxs-lookup"><span data-stu-id="2e5aa-105">Properties</span></span>

| <span data-ttu-id="2e5aa-106">属性</span><span class="sxs-lookup"><span data-stu-id="2e5aa-106">Property</span></span>                 | <span data-ttu-id="2e5aa-107">类型</span><span class="sxs-lookup"><span data-stu-id="2e5aa-107">Type</span></span>   | <span data-ttu-id="2e5aa-108">说明</span><span class="sxs-lookup"><span data-stu-id="2e5aa-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="2e5aa-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2e5aa-109">reportRefreshDate</span></span>        | <span data-ttu-id="2e5aa-110">日期</span><span class="sxs-lookup"><span data-stu-id="2e5aa-110">Date</span></span>   | <span data-ttu-id="2e5aa-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="2e5aa-112">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-112">exchangeActive</span></span>           | <span data-ttu-id="2e5aa-113">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-113">Int64</span></span>  | <span data-ttu-id="2e5aa-114">Exchange 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-114">The number of active users on Exchange.</span></span> <span data-ttu-id="2e5aa-115">任何可以读取和发送电子邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="2e5aa-116">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-116">exchangeInactive</span></span>         | <span data-ttu-id="2e5aa-117">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-117">Int64</span></span>  | <span data-ttu-id="2e5aa-118">Exchange 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="2e5aa-119">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-119">oneDriveActive</span></span>           | <span data-ttu-id="2e5aa-120">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-120">Int64</span></span>  | <span data-ttu-id="2e5aa-121">OneDrive 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="2e5aa-122">任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="2e5aa-123">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-123">oneDriveInactive</span></span>         | <span data-ttu-id="2e5aa-124">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-124">Int64</span></span>  | <span data-ttu-id="2e5aa-125">OneDrive 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="2e5aa-126">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-126">sharePointActive</span></span>         | <span data-ttu-id="2e5aa-127">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-127">Int64</span></span>  | <span data-ttu-id="2e5aa-128">SharePoint 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="2e5aa-129">任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="2e5aa-130">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-130">sharePointInactive</span></span>       | <span data-ttu-id="2e5aa-131">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-131">Int64</span></span>  | <span data-ttu-id="2e5aa-132">SharePoint 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="2e5aa-133">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="2e5aa-134">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-134">Int64</span></span>  | <span data-ttu-id="2e5aa-135">Skype For Business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="2e5aa-136">任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="2e5aa-137">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="2e5aa-138">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-138">Int64</span></span>  | <span data-ttu-id="2e5aa-139">Skype For Business 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="2e5aa-140">yammerActive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-140">yammerActive</span></span>             | <span data-ttu-id="2e5aa-141">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-141">Int64</span></span>  | <span data-ttu-id="2e5aa-142">Yammer 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-142">The number of active users on Yammer.</span></span> <span data-ttu-id="2e5aa-143">任何可以发布、阅读或赞邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="2e5aa-144">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-144">yammerInactive</span></span>           | <span data-ttu-id="2e5aa-145">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-145">Int64</span></span>  | <span data-ttu-id="2e5aa-146">Yammer 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="2e5aa-147">teamsActive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-147">teamsActive</span></span>              | <span data-ttu-id="2e5aa-148">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-148">Int64</span></span>  | <span data-ttu-id="2e5aa-149">Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="2e5aa-150">任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="2e5aa-151">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-151">teamsInactive</span></span>            | <span data-ttu-id="2e5aa-152">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-152">Int64</span></span>  | <span data-ttu-id="2e5aa-153">Microsoft 团队中的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="2e5aa-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="2e5aa-154">office365Active</span></span>          | <span data-ttu-id="2e5aa-155">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-155">Int64</span></span>  | <span data-ttu-id="2e5aa-156">Office 365 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-156">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="2e5aa-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="2e5aa-157">office365Inactive</span></span>        | <span data-ttu-id="2e5aa-158">Int64</span><span class="sxs-lookup"><span data-stu-id="2e5aa-158">Int64</span></span>  | <span data-ttu-id="2e5aa-159">Office 365 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-159">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="2e5aa-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2e5aa-160">reportPeriod</span></span>             | <span data-ttu-id="2e5aa-161">String</span><span class="sxs-lookup"><span data-stu-id="2e5aa-161">String</span></span> | <span data-ttu-id="2e5aa-162">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2e5aa-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e5aa-163">JSON representation</span></span>

<span data-ttu-id="2e5aa-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e5aa-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```
