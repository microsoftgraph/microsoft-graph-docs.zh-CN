---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 36fd043be3cef36951f7651d625f4a93d3b5f8cc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573891"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="f267a-103">office365ServicesUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="f267a-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="f267a-104">属性</span><span class="sxs-lookup"><span data-stu-id="f267a-104">Properties</span></span>

| <span data-ttu-id="f267a-105">属性</span><span class="sxs-lookup"><span data-stu-id="f267a-105">Property</span></span>                 | <span data-ttu-id="f267a-106">类型</span><span class="sxs-lookup"><span data-stu-id="f267a-106">Type</span></span>   | <span data-ttu-id="f267a-107">说明</span><span class="sxs-lookup"><span data-stu-id="f267a-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="f267a-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f267a-108">reportRefreshDate</span></span>        | <span data-ttu-id="f267a-109">Date</span><span class="sxs-lookup"><span data-stu-id="f267a-109">Date</span></span>   | <span data-ttu-id="f267a-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="f267a-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="f267a-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="f267a-111">exchangeActive</span></span>           | <span data-ttu-id="f267a-112">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-112">Int64</span></span>  | <span data-ttu-id="f267a-113">在 Exchange 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-113">The number of active users on Exchange.</span></span> <span data-ttu-id="f267a-114">任何用户都可以读取和发送电子邮件被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="f267a-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="f267a-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="f267a-115">exchangeInactive</span></span>         | <span data-ttu-id="f267a-116">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-116">Int64</span></span>  | <span data-ttu-id="f267a-117">在 Exchange 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="f267a-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="f267a-118">oneDriveActive</span></span>           | <span data-ttu-id="f267a-119">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-119">Int64</span></span>  | <span data-ttu-id="f267a-120">在 OneDrive 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="f267a-121">查看或编辑文件、 内部或外部，共享文件或同步文件的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="f267a-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="f267a-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="f267a-122">oneDriveInactive</span></span>         | <span data-ttu-id="f267a-123">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-123">Int64</span></span>  | <span data-ttu-id="f267a-124">Onedrive 非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="f267a-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="f267a-125">sharePointActive</span></span>         | <span data-ttu-id="f267a-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-126">Int64</span></span>  | <span data-ttu-id="f267a-127">在 SharePoint 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="f267a-128">查看或编辑文件、 共享文件内部或外部同步文件，或查看 SharePoint 页的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="f267a-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="f267a-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="f267a-129">sharePointInactive</span></span>       | <span data-ttu-id="f267a-130">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-130">Int64</span></span>  | <span data-ttu-id="f267a-131">在 SharePoint 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="f267a-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="f267a-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="f267a-133">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-133">Int64</span></span>  | <span data-ttu-id="f267a-134">Skype 的业务上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="f267a-135">组织或参加会议，或加入对等会话的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="f267a-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="f267a-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="f267a-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="f267a-137">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-137">Int64</span></span>  | <span data-ttu-id="f267a-138">Skype 的业务的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="f267a-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="f267a-139">yammerActive</span></span>             | <span data-ttu-id="f267a-140">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-140">Int64</span></span>  | <span data-ttu-id="f267a-141">Yammer 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-141">The number of active users on Yammer.</span></span> <span data-ttu-id="f267a-142">任何用户都可以发布、 读取或类似于邮件被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="f267a-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="f267a-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="f267a-143">yammerInactive</span></span>           | <span data-ttu-id="f267a-144">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-144">Int64</span></span>  | <span data-ttu-id="f267a-145">在 Yammer 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="f267a-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="f267a-146">teamsActive</span></span>              | <span data-ttu-id="f267a-147">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-147">Int64</span></span>  | <span data-ttu-id="f267a-148">在 Microsoft 团队的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="f267a-149">在工作组通道中发布消息、 私人聊天会话中发送的邮件或参加会议或进行呼叫的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="f267a-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="f267a-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="f267a-150">teamsInactive</span></span>            | <span data-ttu-id="f267a-151">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-151">Int64</span></span>  | <span data-ttu-id="f267a-152">在 Microsoft 团队的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="f267a-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="f267a-153">office365Active</span></span>          | <span data-ttu-id="f267a-154">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-154">Int64</span></span>  | <span data-ttu-id="f267a-155">Office 365 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="f267a-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="f267a-156">office365Inactive</span></span>        | <span data-ttu-id="f267a-157">Int64</span><span class="sxs-lookup"><span data-stu-id="f267a-157">Int64</span></span>  | <span data-ttu-id="f267a-158">Office 365 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="f267a-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="f267a-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f267a-159">reportPeriod</span></span>             | <span data-ttu-id="f267a-160">String</span><span class="sxs-lookup"><span data-stu-id="f267a-160">String</span></span> | <span data-ttu-id="f267a-161">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="f267a-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="f267a-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f267a-162">JSON representation</span></span>

<span data-ttu-id="f267a-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f267a-163">The following is a JSON representation of the resource.</span></span>

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
