---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 5958ab3cb05767465b0866078d378208f1b466e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009466"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="410e4-103">office365ServicesUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="410e4-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="410e4-104">属性</span><span class="sxs-lookup"><span data-stu-id="410e4-104">Properties</span></span>

| <span data-ttu-id="410e4-105">属性</span><span class="sxs-lookup"><span data-stu-id="410e4-105">Property</span></span>                 | <span data-ttu-id="410e4-106">类型</span><span class="sxs-lookup"><span data-stu-id="410e4-106">Type</span></span>   | <span data-ttu-id="410e4-107">说明</span><span class="sxs-lookup"><span data-stu-id="410e4-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="410e4-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="410e4-108">reportRefreshDate</span></span>        | <span data-ttu-id="410e4-109">日期</span><span class="sxs-lookup"><span data-stu-id="410e4-109">Date</span></span>   | <span data-ttu-id="410e4-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="410e4-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="410e4-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="410e4-111">exchangeActive</span></span>           | <span data-ttu-id="410e4-112">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-112">Int64</span></span>  | <span data-ttu-id="410e4-113">Exchange 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-113">The number of active users on Exchange.</span></span> <span data-ttu-id="410e4-114">任何可以读取和发送电子邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="410e4-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="410e4-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="410e4-115">exchangeInactive</span></span>         | <span data-ttu-id="410e4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-116">Int64</span></span>  | <span data-ttu-id="410e4-117">Exchange 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="410e4-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="410e4-118">oneDriveActive</span></span>           | <span data-ttu-id="410e4-119">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-119">Int64</span></span>  | <span data-ttu-id="410e4-120">OneDrive 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="410e4-121">任何查看或编辑文件、内部或外部共享文件或已同步文件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="410e4-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="410e4-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="410e4-122">oneDriveInactive</span></span>         | <span data-ttu-id="410e4-123">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-123">Int64</span></span>  | <span data-ttu-id="410e4-124">OneDrive 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="410e4-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="410e4-125">sharePointActive</span></span>         | <span data-ttu-id="410e4-126">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-126">Int64</span></span>  | <span data-ttu-id="410e4-127">SharePoint 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="410e4-128">任何查看或编辑过文件、内部或外部共享文件、同步文件或查看 SharePoint 页面的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="410e4-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="410e4-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="410e4-129">sharePointInactive</span></span>       | <span data-ttu-id="410e4-130">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-130">Int64</span></span>  | <span data-ttu-id="410e4-131">SharePoint 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="410e4-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="410e4-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="410e4-133">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-133">Int64</span></span>  | <span data-ttu-id="410e4-134">Skype For Business 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="410e4-135">任何组织或参加过会议的用户或加入的对等会话都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="410e4-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="410e4-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="410e4-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="410e4-137">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-137">Int64</span></span>  | <span data-ttu-id="410e4-138">Skype For Business 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="410e4-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="410e4-139">yammerActive</span></span>             | <span data-ttu-id="410e4-140">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-140">Int64</span></span>  | <span data-ttu-id="410e4-141">Yammer 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-141">The number of active users on Yammer.</span></span> <span data-ttu-id="410e4-142">任何可以发布、阅读或赞邮件的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="410e4-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="410e4-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="410e4-143">yammerInactive</span></span>           | <span data-ttu-id="410e4-144">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-144">Int64</span></span>  | <span data-ttu-id="410e4-145">Yammer 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="410e4-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="410e4-146">teamsActive</span></span>              | <span data-ttu-id="410e4-147">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-147">Int64</span></span>  | <span data-ttu-id="410e4-148">Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="410e4-149">任何在团队频道中投递了邮件、在私人聊天会话中发送的邮件或参与会议或呼叫的用户都被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="410e4-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="410e4-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="410e4-150">teamsInactive</span></span>            | <span data-ttu-id="410e4-151">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-151">Int64</span></span>  | <span data-ttu-id="410e4-152">Microsoft 团队中的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="410e4-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="410e4-153">office365Active</span></span>          | <span data-ttu-id="410e4-154">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-154">Int64</span></span>  | <span data-ttu-id="410e4-155">Office 365 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="410e4-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="410e4-156">office365Inactive</span></span>        | <span data-ttu-id="410e4-157">Int64</span><span class="sxs-lookup"><span data-stu-id="410e4-157">Int64</span></span>  | <span data-ttu-id="410e4-158">Office 365 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="410e4-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="410e4-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="410e4-159">reportPeriod</span></span>             | <span data-ttu-id="410e4-160">String</span><span class="sxs-lookup"><span data-stu-id="410e4-160">String</span></span> | <span data-ttu-id="410e4-161">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="410e4-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="410e4-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="410e4-162">JSON representation</span></span>

<span data-ttu-id="410e4-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="410e4-163">The following is a JSON representation of the resource.</span></span>

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
