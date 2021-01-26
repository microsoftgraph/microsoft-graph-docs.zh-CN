---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 276153f9613f464cdf11f6dfdad307bb341f646d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982150"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="50685-103">office365ServicesUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="50685-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="50685-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50685-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="50685-105">属性</span><span class="sxs-lookup"><span data-stu-id="50685-105">Properties</span></span>

| <span data-ttu-id="50685-106">属性</span><span class="sxs-lookup"><span data-stu-id="50685-106">Property</span></span>                 | <span data-ttu-id="50685-107">类型</span><span class="sxs-lookup"><span data-stu-id="50685-107">Type</span></span>   | <span data-ttu-id="50685-108">说明</span><span class="sxs-lookup"><span data-stu-id="50685-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="50685-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="50685-109">reportRefreshDate</span></span>        | <span data-ttu-id="50685-110">日期</span><span class="sxs-lookup"><span data-stu-id="50685-110">Date</span></span>   | <span data-ttu-id="50685-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="50685-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="50685-112">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="50685-112">exchangeActive</span></span>           | <span data-ttu-id="50685-113">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-113">Int64</span></span>  | <span data-ttu-id="50685-114">Exchange 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-114">The number of active users on Exchange.</span></span> <span data-ttu-id="50685-115">任何可以阅读和发送电子邮件的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="50685-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="50685-116">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="50685-116">exchangeInactive</span></span>         | <span data-ttu-id="50685-117">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-117">Int64</span></span>  | <span data-ttu-id="50685-118">Exchange 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="50685-119">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="50685-119">oneDriveActive</span></span>           | <span data-ttu-id="50685-120">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-120">Int64</span></span>  | <span data-ttu-id="50685-121">OneDrive 上的活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="50685-122">任何在内部或外部查看或编辑文件、共享文件或同步文件的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="50685-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="50685-123">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="50685-123">oneDriveInactive</span></span>         | <span data-ttu-id="50685-124">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-124">Int64</span></span>  | <span data-ttu-id="50685-125">OneDrive 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="50685-126">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="50685-126">sharePointActive</span></span>         | <span data-ttu-id="50685-127">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-127">Int64</span></span>  | <span data-ttu-id="50685-128">SharePoint 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="50685-129">任何在内部或外部查看或编辑文件、共享文件、同步文件或查看 SharePoint 页面的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="50685-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="50685-130">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="50685-130">sharePointInactive</span></span>       | <span data-ttu-id="50685-131">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-131">Int64</span></span>  | <span data-ttu-id="50685-132">SharePoint 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="50685-133">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="50685-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="50685-134">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-134">Int64</span></span>  | <span data-ttu-id="50685-135">Skype For Business 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="50685-136">组织或参与会议或加入对等会话的任何用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="50685-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="50685-137">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="50685-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="50685-138">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-138">Int64</span></span>  | <span data-ttu-id="50685-139">Skype For Business 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="50685-140">yammerActive</span><span class="sxs-lookup"><span data-stu-id="50685-140">yammerActive</span></span>             | <span data-ttu-id="50685-141">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-141">Int64</span></span>  | <span data-ttu-id="50685-142">Yammer 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-142">The number of active users on Yammer.</span></span> <span data-ttu-id="50685-143">任何可以发布、阅读或喜欢消息的用户都将被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="50685-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="50685-144">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="50685-144">yammerInactive</span></span>           | <span data-ttu-id="50685-145">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-145">Int64</span></span>  | <span data-ttu-id="50685-146">Yammer 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="50685-147">teamsActive</span><span class="sxs-lookup"><span data-stu-id="50685-147">teamsActive</span></span>              | <span data-ttu-id="50685-148">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-148">Int64</span></span>  | <span data-ttu-id="50685-149">Microsoft Teams 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="50685-150">任何在团队频道中发布消息、在私人聊天会话中发送消息或参与会议或通话的用户均被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="50685-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="50685-151">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="50685-151">teamsInactive</span></span>            | <span data-ttu-id="50685-152">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-152">Int64</span></span>  | <span data-ttu-id="50685-153">Microsoft Teams 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="50685-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="50685-154">office365Active</span></span>          | <span data-ttu-id="50685-155">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-155">Int64</span></span>  | <span data-ttu-id="50685-156">Microsoft 365 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-156">The number of active users on Microsoft 365.</span></span>   |
| <span data-ttu-id="50685-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="50685-157">office365Inactive</span></span>        | <span data-ttu-id="50685-158">Int64</span><span class="sxs-lookup"><span data-stu-id="50685-158">Int64</span></span>  | <span data-ttu-id="50685-159">Microsoft 365 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="50685-159">The number of inactive users on Microsoft 365.</span></span>     |
| <span data-ttu-id="50685-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="50685-160">reportPeriod</span></span>             | <span data-ttu-id="50685-161">String</span><span class="sxs-lookup"><span data-stu-id="50685-161">String</span></span> | <span data-ttu-id="50685-162">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="50685-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="50685-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50685-163">JSON representation</span></span>

<span data-ttu-id="50685-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50685-164">The following is a JSON representation of the resource.</span></span>

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


