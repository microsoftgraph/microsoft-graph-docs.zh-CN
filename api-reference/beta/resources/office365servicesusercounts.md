---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 80bfb483e7e15dcdaffb6a8ba8ed30c8bb508f5c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092354"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="e4be7-103">office365ServicesUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4be7-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="e4be7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4be7-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="e4be7-105">属性</span><span class="sxs-lookup"><span data-stu-id="e4be7-105">Properties</span></span>

| <span data-ttu-id="e4be7-106">属性</span><span class="sxs-lookup"><span data-stu-id="e4be7-106">Property</span></span>                 | <span data-ttu-id="e4be7-107">类型</span><span class="sxs-lookup"><span data-stu-id="e4be7-107">Type</span></span>   | <span data-ttu-id="e4be7-108">说明</span><span class="sxs-lookup"><span data-stu-id="e4be7-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="e4be7-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="e4be7-109">reportRefreshDate</span></span>        | <span data-ttu-id="e4be7-110">日期</span><span class="sxs-lookup"><span data-stu-id="e4be7-110">Date</span></span>   | <span data-ttu-id="e4be7-111">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="e4be7-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="e4be7-112">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="e4be7-112">exchangeActive</span></span>           | <span data-ttu-id="e4be7-113">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-113">Int64</span></span>  | <span data-ttu-id="e4be7-114">Exchange 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-114">The number of active users on Exchange.</span></span> <span data-ttu-id="e4be7-115">任何可以读取和发送电子邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="e4be7-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="e4be7-116">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="e4be7-116">exchangeInactive</span></span>         | <span data-ttu-id="e4be7-117">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-117">Int64</span></span>  | <span data-ttu-id="e4be7-118">Exchange 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="e4be7-119">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="e4be7-119">oneDriveActive</span></span>           | <span data-ttu-id="e4be7-120">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-120">Int64</span></span>  | <span data-ttu-id="e4be7-121">OneDrive 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="e4be7-122">任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="e4be7-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="e4be7-123">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="e4be7-123">oneDriveInactive</span></span>         | <span data-ttu-id="e4be7-124">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-124">Int64</span></span>  | <span data-ttu-id="e4be7-125">OneDrive 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="e4be7-126">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="e4be7-126">sharePointActive</span></span>         | <span data-ttu-id="e4be7-127">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-127">Int64</span></span>  | <span data-ttu-id="e4be7-128">SharePoint 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="e4be7-129">任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="e4be7-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="e4be7-130">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="e4be7-130">sharePointInactive</span></span>       | <span data-ttu-id="e4be7-131">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-131">Int64</span></span>  | <span data-ttu-id="e4be7-132">SharePoint 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="e4be7-133">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="e4be7-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="e4be7-134">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-134">Int64</span></span>  | <span data-ttu-id="e4be7-135">Skype For Business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="e4be7-136">任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="e4be7-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="e4be7-137">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="e4be7-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="e4be7-138">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-138">Int64</span></span>  | <span data-ttu-id="e4be7-139">Skype For Business 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="e4be7-140">yammerActive</span><span class="sxs-lookup"><span data-stu-id="e4be7-140">yammerActive</span></span>             | <span data-ttu-id="e4be7-141">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-141">Int64</span></span>  | <span data-ttu-id="e4be7-142">Yammer 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-142">The number of active users on Yammer.</span></span> <span data-ttu-id="e4be7-143">任何可以发布、阅读或赞邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="e4be7-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="e4be7-144">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="e4be7-144">yammerInactive</span></span>           | <span data-ttu-id="e4be7-145">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-145">Int64</span></span>  | <span data-ttu-id="e4be7-146">Yammer 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="e4be7-147">teamsActive</span><span class="sxs-lookup"><span data-stu-id="e4be7-147">teamsActive</span></span>              | <span data-ttu-id="e4be7-148">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-148">Int64</span></span>  | <span data-ttu-id="e4be7-149">Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="e4be7-150">任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="e4be7-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="e4be7-151">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="e4be7-151">teamsInactive</span></span>            | <span data-ttu-id="e4be7-152">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-152">Int64</span></span>  | <span data-ttu-id="e4be7-153">Microsoft 团队中的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="e4be7-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="e4be7-154">office365Active</span></span>          | <span data-ttu-id="e4be7-155">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-155">Int64</span></span>  | <span data-ttu-id="e4be7-156">Microsoft 365 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-156">The number of active users on Microsoft 365.</span></span>   |
| <span data-ttu-id="e4be7-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="e4be7-157">office365Inactive</span></span>        | <span data-ttu-id="e4be7-158">Int64</span><span class="sxs-lookup"><span data-stu-id="e4be7-158">Int64</span></span>  | <span data-ttu-id="e4be7-159">Microsoft 365 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-159">The number of inactive users on Microsoft 365.</span></span>     |
| <span data-ttu-id="e4be7-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="e4be7-160">reportPeriod</span></span>             | <span data-ttu-id="e4be7-161">字符串</span><span class="sxs-lookup"><span data-stu-id="e4be7-161">String</span></span> | <span data-ttu-id="e4be7-162">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="e4be7-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="e4be7-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4be7-163">JSON representation</span></span>

<span data-ttu-id="e4be7-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4be7-164">The following is a JSON representation of the resource.</span></span>

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


