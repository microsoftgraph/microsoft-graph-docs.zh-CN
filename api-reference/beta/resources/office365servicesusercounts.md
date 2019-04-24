---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32505457"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="6ad95-103">office365ServicesUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ad95-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="6ad95-104">属性</span><span class="sxs-lookup"><span data-stu-id="6ad95-104">Properties</span></span>

| <span data-ttu-id="6ad95-105">属性</span><span class="sxs-lookup"><span data-stu-id="6ad95-105">Property</span></span>                 | <span data-ttu-id="6ad95-106">类型</span><span class="sxs-lookup"><span data-stu-id="6ad95-106">Type</span></span>   | <span data-ttu-id="6ad95-107">说明</span><span class="sxs-lookup"><span data-stu-id="6ad95-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="6ad95-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="6ad95-108">reportRefreshDate</span></span>        | <span data-ttu-id="6ad95-109">Date</span><span class="sxs-lookup"><span data-stu-id="6ad95-109">Date</span></span>   | <span data-ttu-id="6ad95-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="6ad95-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="6ad95-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="6ad95-111">exchangeActive</span></span>           | <span data-ttu-id="6ad95-112">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-112">Int64</span></span>  | <span data-ttu-id="6ad95-113">Exchange 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-113">The number of active users on Exchange.</span></span> <span data-ttu-id="6ad95-114">任何可以读取和发送电子邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6ad95-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="6ad95-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="6ad95-115">exchangeInactive</span></span>         | <span data-ttu-id="6ad95-116">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-116">Int64</span></span>  | <span data-ttu-id="6ad95-117">Exchange 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="6ad95-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="6ad95-118">oneDriveActive</span></span>           | <span data-ttu-id="6ad95-119">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-119">Int64</span></span>  | <span data-ttu-id="6ad95-120">OneDrive 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="6ad95-121">任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6ad95-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="6ad95-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="6ad95-122">oneDriveInactive</span></span>         | <span data-ttu-id="6ad95-123">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-123">Int64</span></span>  | <span data-ttu-id="6ad95-124">OneDrive 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="6ad95-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="6ad95-125">sharePointActive</span></span>         | <span data-ttu-id="6ad95-126">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-126">Int64</span></span>  | <span data-ttu-id="6ad95-127">SharePoint 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="6ad95-128">任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6ad95-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="6ad95-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="6ad95-129">sharePointInactive</span></span>       | <span data-ttu-id="6ad95-130">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-130">Int64</span></span>  | <span data-ttu-id="6ad95-131">SharePoint 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="6ad95-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="6ad95-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="6ad95-133">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-133">Int64</span></span>  | <span data-ttu-id="6ad95-134">Skype for business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="6ad95-135">任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6ad95-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="6ad95-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="6ad95-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="6ad95-137">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-137">Int64</span></span>  | <span data-ttu-id="6ad95-138">Skype for business 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="6ad95-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="6ad95-139">yammerActive</span></span>             | <span data-ttu-id="6ad95-140">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-140">Int64</span></span>  | <span data-ttu-id="6ad95-141">Yammer 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-141">The number of active users on Yammer.</span></span> <span data-ttu-id="6ad95-142">任何可以发布、阅读或赞邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6ad95-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="6ad95-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="6ad95-143">yammerInactive</span></span>           | <span data-ttu-id="6ad95-144">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-144">Int64</span></span>  | <span data-ttu-id="6ad95-145">Yammer 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="6ad95-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="6ad95-146">teamsActive</span></span>              | <span data-ttu-id="6ad95-147">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-147">Int64</span></span>  | <span data-ttu-id="6ad95-148">Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="6ad95-149">任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="6ad95-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="6ad95-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="6ad95-150">teamsInactive</span></span>            | <span data-ttu-id="6ad95-151">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-151">Int64</span></span>  | <span data-ttu-id="6ad95-152">Microsoft 团队中的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="6ad95-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="6ad95-153">office365Active</span></span>          | <span data-ttu-id="6ad95-154">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-154">Int64</span></span>  | <span data-ttu-id="6ad95-155">Office 365 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="6ad95-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="6ad95-156">office365Inactive</span></span>        | <span data-ttu-id="6ad95-157">Int64</span><span class="sxs-lookup"><span data-stu-id="6ad95-157">Int64</span></span>  | <span data-ttu-id="6ad95-158">Office 365 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="6ad95-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="6ad95-159">reportPeriod</span></span>             | <span data-ttu-id="6ad95-160">字符串</span><span class="sxs-lookup"><span data-stu-id="6ad95-160">String</span></span> | <span data-ttu-id="6ad95-161">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="6ad95-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6ad95-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ad95-162">JSON representation</span></span>

<span data-ttu-id="6ad95-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ad95-163">The following is a JSON representation of the resource.</span></span>

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
