---
title: office365ActiveUserCounts 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 887f9b08d7f46aac023fbd0f34e6174e5f422760
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882717"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="eaa69-103">office365ActiveUserCounts 资源类型</span><span class="sxs-lookup"><span data-stu-id="eaa69-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="eaa69-104">属性</span><span class="sxs-lookup"><span data-stu-id="eaa69-104">Properties</span></span>

| <span data-ttu-id="eaa69-105">属性</span><span class="sxs-lookup"><span data-stu-id="eaa69-105">Property</span></span>          | <span data-ttu-id="eaa69-106">类型</span><span class="sxs-lookup"><span data-stu-id="eaa69-106">Type</span></span>   | <span data-ttu-id="eaa69-107">Description</span><span class="sxs-lookup"><span data-stu-id="eaa69-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="eaa69-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="eaa69-108">reportRefreshDate</span></span> | <span data-ttu-id="eaa69-109">日期</span><span class="sxs-lookup"><span data-stu-id="eaa69-109">Date</span></span>   | <span data-ttu-id="eaa69-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="eaa69-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="eaa69-111">office365</span><span class="sxs-lookup"><span data-stu-id="eaa69-111">office365</span></span>         | <span data-ttu-id="eaa69-112">Int64</span><span class="sxs-lookup"><span data-stu-id="eaa69-112">Int64</span></span>  | <span data-ttu-id="eaa69-113">Office 365 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-113">The number of active users in Office 365.</span></span> <span data-ttu-id="eaa69-114">此数值包括 Exchange、 OneDrive、 SharePoint、 Skype 的业务、 Yammer，和 Microsoft 团队中的所有活动的用户。</span><span class="sxs-lookup"><span data-stu-id="eaa69-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="eaa69-115">您可以找到各自属性说明中的每个产品的活动用户定义。</span><span class="sxs-lookup"><span data-stu-id="eaa69-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="eaa69-116">exchange</span><span class="sxs-lookup"><span data-stu-id="eaa69-116">exchange</span></span>          | <span data-ttu-id="eaa69-117">Int64</span><span class="sxs-lookup"><span data-stu-id="eaa69-117">Int64</span></span>  | <span data-ttu-id="eaa69-118">Exchange 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-118">The number of active users in Exchange.</span></span> <span data-ttu-id="eaa69-119">任何用户都可以读取和发送电子邮件被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="eaa69-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="eaa69-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="eaa69-120">oneDrive</span></span>          | <span data-ttu-id="eaa69-121">Int64</span><span class="sxs-lookup"><span data-stu-id="eaa69-121">Int64</span></span>  | <span data-ttu-id="eaa69-122">OneDrive 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="eaa69-123">查看或编辑文件、 内部或外部，共享文件或同步文件的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="eaa69-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="eaa69-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="eaa69-124">sharePoint</span></span>        | <span data-ttu-id="eaa69-125">Int64</span><span class="sxs-lookup"><span data-stu-id="eaa69-125">Int64</span></span>  | <span data-ttu-id="eaa69-126">在 SharePoint 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="eaa69-127">查看或编辑文件、 共享文件内部或外部同步文件，或查看 SharePoint 页的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="eaa69-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="eaa69-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="eaa69-128">skypeForBusiness</span></span>  | <span data-ttu-id="eaa69-129">Int64</span><span class="sxs-lookup"><span data-stu-id="eaa69-129">Int64</span></span>  | <span data-ttu-id="eaa69-130">Skype 的企业中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="eaa69-131">组织或参加会议，或加入对等会话的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="eaa69-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="eaa69-132">yammer</span><span class="sxs-lookup"><span data-stu-id="eaa69-132">yammer</span></span>            | <span data-ttu-id="eaa69-133">Int64</span><span class="sxs-lookup"><span data-stu-id="eaa69-133">Int64</span></span>  | <span data-ttu-id="eaa69-134">Yammer 中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-134">The number of active users in Yammer.</span></span> <span data-ttu-id="eaa69-135">任何用户都可以发布、 读取或类似于邮件被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="eaa69-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="eaa69-136">团队</span><span class="sxs-lookup"><span data-stu-id="eaa69-136">teams</span></span>             | <span data-ttu-id="eaa69-137">Int64</span><span class="sxs-lookup"><span data-stu-id="eaa69-137">Int64</span></span>  | <span data-ttu-id="eaa69-138">在 Microsoft 团队中的活动用户数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="eaa69-139">在工作组通道中发布消息、 私人聊天会话中发送的邮件或参加会议或进行呼叫的任何用户被视为活动用户。</span><span class="sxs-lookup"><span data-stu-id="eaa69-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="eaa69-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="eaa69-140">reportDate</span></span>        | <span data-ttu-id="eaa69-141">日期</span><span class="sxs-lookup"><span data-stu-id="eaa69-141">Date</span></span>   | <span data-ttu-id="eaa69-142">多个用户在其处于活动状态日期。</span><span class="sxs-lookup"><span data-stu-id="eaa69-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="eaa69-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="eaa69-143">reportPeriod</span></span>      | <span data-ttu-id="eaa69-144">字符串</span><span class="sxs-lookup"><span data-stu-id="eaa69-144">String</span></span> | <span data-ttu-id="eaa69-145">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="eaa69-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="eaa69-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eaa69-146">JSON representation</span></span>

<span data-ttu-id="eaa69-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eaa69-147">The following is a JSON representation of the resource.</span></span>

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
