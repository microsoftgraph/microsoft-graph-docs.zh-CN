---
title: office365ServicesUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 975a70b040ac5886ea36219a5407f580a42aeadc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042405"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="47f5f-103">office365ServicesUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="47f5f-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="47f5f-104">属性</span><span class="sxs-lookup"><span data-stu-id="47f5f-104">Properties</span></span>

| <span data-ttu-id="47f5f-105">属性</span><span class="sxs-lookup"><span data-stu-id="47f5f-105">Property</span></span>                 | <span data-ttu-id="47f5f-106">类型</span><span class="sxs-lookup"><span data-stu-id="47f5f-106">Type</span></span>   | <span data-ttu-id="47f5f-107">说明</span><span class="sxs-lookup"><span data-stu-id="47f5f-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="47f5f-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="47f5f-108">reportRefreshDate</span></span>        | <span data-ttu-id="47f5f-109">日期</span><span class="sxs-lookup"><span data-stu-id="47f5f-109">Date</span></span>   | <span data-ttu-id="47f5f-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="47f5f-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="47f5f-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="47f5f-111">exchangeActive</span></span>           | <span data-ttu-id="47f5f-112">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-112">Int64</span></span>  | <span data-ttu-id="47f5f-113">在 Exchange 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-113">The number of active users on Exchange.</span></span> <span data-ttu-id="47f5f-114">任何用户都可以读取和发送电子邮件被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="47f5f-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="47f5f-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="47f5f-115">exchangeInactive</span></span>         | <span data-ttu-id="47f5f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-116">Int64</span></span>  | <span data-ttu-id="47f5f-117">在 Exchange 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="47f5f-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="47f5f-118">oneDriveActive</span></span>           | <span data-ttu-id="47f5f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-119">Int64</span></span>  | <span data-ttu-id="47f5f-120">在 OneDrive 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="47f5f-121">查看或编辑文件、 内部或外部，共享文件或同步文件的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="47f5f-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="47f5f-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="47f5f-122">oneDriveInactive</span></span>         | <span data-ttu-id="47f5f-123">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-123">Int64</span></span>  | <span data-ttu-id="47f5f-124">Onedrive 非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="47f5f-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="47f5f-125">sharePointActive</span></span>         | <span data-ttu-id="47f5f-126">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-126">Int64</span></span>  | <span data-ttu-id="47f5f-127">在 SharePoint 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="47f5f-128">查看或编辑文件、 共享文件内部或外部同步文件，或查看 SharePoint 页的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="47f5f-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="47f5f-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="47f5f-129">sharePointInactive</span></span>       | <span data-ttu-id="47f5f-130">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-130">Int64</span></span>  | <span data-ttu-id="47f5f-131">在 SharePoint 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="47f5f-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="47f5f-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="47f5f-133">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-133">Int64</span></span>  | <span data-ttu-id="47f5f-134">Skype 的业务上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="47f5f-135">组织或参加会议，或加入对等会话的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="47f5f-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="47f5f-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="47f5f-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="47f5f-137">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-137">Int64</span></span>  | <span data-ttu-id="47f5f-138">Skype 的业务的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="47f5f-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="47f5f-139">yammerActive</span></span>             | <span data-ttu-id="47f5f-140">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-140">Int64</span></span>  | <span data-ttu-id="47f5f-141">Yammer 上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-141">The number of active users on Yammer.</span></span> <span data-ttu-id="47f5f-142">任何用户都可以发布、 读取或类似于邮件被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="47f5f-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="47f5f-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="47f5f-143">yammerInactive</span></span>           | <span data-ttu-id="47f5f-144">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-144">Int64</span></span>  | <span data-ttu-id="47f5f-145">在 Yammer 上的非活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="47f5f-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="47f5f-146">teamsActive</span></span>              | <span data-ttu-id="47f5f-147">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-147">Int64</span></span>  | <span data-ttu-id="47f5f-148">团队上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-148">The number of active users on Teams.</span></span> <span data-ttu-id="47f5f-149">在工作组通道中发布消息、 私人聊天会话中发送的邮件或参加会议或进行呼叫的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="47f5f-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="47f5f-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="47f5f-150">teamsInactive</span></span>            | <span data-ttu-id="47f5f-151">Int64</span><span class="sxs-lookup"><span data-stu-id="47f5f-151">Int64</span></span>  | <span data-ttu-id="47f5f-152">团队上的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-152">The number of active users on Teams.</span></span>     |
| <span data-ttu-id="47f5f-153">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="47f5f-153">reportPeriod</span></span>             | <span data-ttu-id="47f5f-154">字符串</span><span class="sxs-lookup"><span data-stu-id="47f5f-154">String</span></span> | <span data-ttu-id="47f5f-155">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="47f5f-155">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="47f5f-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47f5f-156">JSON representation</span></span>

<span data-ttu-id="47f5f-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47f5f-157">The following is a JSON representation of the resource.</span></span>

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
  "reportPeriod": "String"
}
```
