---
title: teamsUserActivityUserDetail 资源类型
description: 表示有关用户 Microsoft Teams 用户活动的详细信息。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4afa7f17acac13eaa1c517953517fcfbe344aaa7
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766432"
---
# <a name="teamsuseractivityuserdetail-resource-type"></a><span data-ttu-id="42678-103">teamsUserActivityUserDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="42678-103">teamsUserActivityUserDetail resource type</span></span>

<span data-ttu-id="42678-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42678-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42678-105">表示有关用户 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="42678-105">Represents details about Microsoft Teams user activity by user.</span></span>

## <a name="properties"></a><span data-ttu-id="42678-106">属性</span><span class="sxs-lookup"><span data-stu-id="42678-106">Properties</span></span>

| <span data-ttu-id="42678-107">属性</span><span class="sxs-lookup"><span data-stu-id="42678-107">Property</span></span>                                 | <span data-ttu-id="42678-108">类型</span><span class="sxs-lookup"><span data-stu-id="42678-108">Type</span></span>              | <span data-ttu-id="42678-109">说明</span><span class="sxs-lookup"><span data-stu-id="42678-109">Description</span></span>                                                  |
| :--------------------------------------- | :---------------- | ------------------------------------------------------------ |
| <span data-ttu-id="42678-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="42678-110">reportRefreshDate</span></span>                        | <span data-ttu-id="42678-111">日期</span><span class="sxs-lookup"><span data-stu-id="42678-111">Date</span></span>              | <span data-ttu-id="42678-112">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="42678-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="42678-113">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="42678-113">userPrincipalName</span></span>                        | <span data-ttu-id="42678-114">String</span><span class="sxs-lookup"><span data-stu-id="42678-114">String</span></span>            | <span data-ttu-id="42678-115">用户的用户主体名称 (UPN)。</span><span class="sxs-lookup"><span data-stu-id="42678-115">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="42678-116">UPN 是用户基于 Internet 标准 RFC 822 的 Internet 式登录名。</span><span class="sxs-lookup"><span data-stu-id="42678-116">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="42678-117">按照惯例，此名称应映射到用户的电子邮件名称。</span><span class="sxs-lookup"><span data-stu-id="42678-117">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="42678-118">常规格式是 alias@domain，其中，domain 必须位于租户的已验证域集合中。</span><span class="sxs-lookup"><span data-stu-id="42678-118">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="42678-119">创建用户时此属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="42678-119">This property is required when a user is created.</span></span> |
| <span data-ttu-id="42678-120">isLicensed</span><span class="sxs-lookup"><span data-stu-id="42678-120">isLicensed</span></span>                               | <span data-ttu-id="42678-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="42678-121">Boolean</span></span>           | <span data-ttu-id="42678-122">是否已为用户分配 Teams 许可证。</span><span class="sxs-lookup"><span data-stu-id="42678-122">Whether the user has been assigned a Teams license.</span></span>          |
| <span data-ttu-id="42678-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="42678-123">lastActivityDate</span></span>                         | <span data-ttu-id="42678-124">日期</span><span class="sxs-lookup"><span data-stu-id="42678-124">Date</span></span>              | <span data-ttu-id="42678-125">用户上次参与 Microsoft Teams 活动的日期。</span><span class="sxs-lookup"><span data-stu-id="42678-125">The last date that the user participated in a Microsoft Teams activity.</span></span> |
| <span data-ttu-id="42678-126">isDeleted</span><span class="sxs-lookup"><span data-stu-id="42678-126">isDeleted</span></span>                                | <span data-ttu-id="42678-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="42678-127">Boolean</span></span>           | <span data-ttu-id="42678-128">此用户是已删除还是软删除。</span><span class="sxs-lookup"><span data-stu-id="42678-128">Whether this user has been deleted or soft deleted.</span></span>          |
| <span data-ttu-id="42678-129">deletedDate</span><span class="sxs-lookup"><span data-stu-id="42678-129">deletedDate</span></span>                              | <span data-ttu-id="42678-130">日期</span><span class="sxs-lookup"><span data-stu-id="42678-130">Date</span></span>              | <span data-ttu-id="42678-131">删除操作发生的日期。</span><span class="sxs-lookup"><span data-stu-id="42678-131">The date when the delete operation happened.</span></span> <span data-ttu-id="42678-132">如果用户尚未删除，则默认值为"null"。</span><span class="sxs-lookup"><span data-stu-id="42678-132">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="42678-133">assignedProducts</span><span class="sxs-lookup"><span data-stu-id="42678-133">assignedProducts</span></span>                         | <span data-ttu-id="42678-134">String 集合</span><span class="sxs-lookup"><span data-stu-id="42678-134">String collection</span></span> | <span data-ttu-id="42678-135">用户分配的产品。</span><span class="sxs-lookup"><span data-stu-id="42678-135">Products the user assigned with.</span></span>                             |
| <span data-ttu-id="42678-136">teamChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="42678-136">teamChatMessageCount</span></span>                     | <span data-ttu-id="42678-137">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-137">Int64</span></span>             | <span data-ttu-id="42678-138">用户在团队聊天中发布的唯一消息数。</span><span class="sxs-lookup"><span data-stu-id="42678-138">The number of unique messages that the user posted in a team chat.</span></span> |
| <span data-ttu-id="42678-139">privateChatMessageCount</span><span class="sxs-lookup"><span data-stu-id="42678-139">privateChatMessageCount</span></span>                  | <span data-ttu-id="42678-140">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-140">Int64</span></span>             | <span data-ttu-id="42678-141">用户在私人聊天中发布的唯一消息数。</span><span class="sxs-lookup"><span data-stu-id="42678-141">The number of unique messages that the user posted in a private chat.</span></span> |
| <span data-ttu-id="42678-142">callCount</span><span class="sxs-lookup"><span data-stu-id="42678-142">callCount</span></span>                                | <span data-ttu-id="42678-143">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-143">Int64</span></span>             | <span data-ttu-id="42678-144">用户参与的 1：1 呼叫数。</span><span class="sxs-lookup"><span data-stu-id="42678-144">The number of 1:1 calls that the user participated in.</span></span>       |
| <span data-ttu-id="42678-145">meetingCount</span><span class="sxs-lookup"><span data-stu-id="42678-145">meetingCount</span></span>                             | <span data-ttu-id="42678-146">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-146">Int64</span></span>             | <span data-ttu-id="42678-147">用户参与的联机会议数。</span><span class="sxs-lookup"><span data-stu-id="42678-147">The number of online meetings that the user participated in.</span></span> |
| <span data-ttu-id="42678-148">meetingsOrganizedCount</span><span class="sxs-lookup"><span data-stu-id="42678-148">meetingsOrganizedCount</span></span>                   | <span data-ttu-id="42678-149">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-149">Int64</span></span>             | <span data-ttu-id="42678-150">用户组织的一次性计划会议、定期会议、临时会议和未分类会议的总和。</span><span class="sxs-lookup"><span data-stu-id="42678-150">The sum of one-time scheduled, Recurring, ad hoc and unclassified meetings a user organized.</span></span> |
| <span data-ttu-id="42678-151">meetingsAttendedCount</span><span class="sxs-lookup"><span data-stu-id="42678-151">meetingsAttendedCount</span></span>                    | <span data-ttu-id="42678-152">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-152">Int64</span></span>             | <span data-ttu-id="42678-153">用户参与的一次性计划、定期、临时和未分类会议的总和。</span><span class="sxs-lookup"><span data-stu-id="42678-153">The sum of the one-time scheduled, recurring, ad hoc and unclassified meetings a user participated in.</span></span> |
| <span data-ttu-id="42678-154">adHocMeetingsOrganizedCount</span><span class="sxs-lookup"><span data-stu-id="42678-154">adHocMeetingsOrganizedCount</span></span>              | <span data-ttu-id="42678-155">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-155">Int64</span></span>             | <span data-ttu-id="42678-156">用户组织的临时会议的数量。</span><span class="sxs-lookup"><span data-stu-id="42678-156">The number of ad hoc meetings a user organized.</span></span>              |
| <span data-ttu-id="42678-157">adHocMeetingsAttendedCount</span><span class="sxs-lookup"><span data-stu-id="42678-157">adHocMeetingsAttendedCount</span></span>               | <span data-ttu-id="42678-158">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-158">Int64</span></span>             | <span data-ttu-id="42678-159">用户参与临时会议的数量。</span><span class="sxs-lookup"><span data-stu-id="42678-159">The number of ad hoc meetings a user participated in.</span></span>        |
| <span data-ttu-id="42678-160">scheduledOneTimeMeetingsOrganizedCount</span><span class="sxs-lookup"><span data-stu-id="42678-160">scheduledOneTimeMeetingsOrganizedCount</span></span>   | <span data-ttu-id="42678-161">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-161">Int64</span></span>             | <span data-ttu-id="42678-162">用户组织的一次计划会议的数量。</span><span class="sxs-lookup"><span data-stu-id="42678-162">The number of one-time scheduled meetings a user organized.</span></span>  |
| <span data-ttu-id="42678-163">scheduledOneTimeMeetingsAttendedCount</span><span class="sxs-lookup"><span data-stu-id="42678-163">scheduledOneTimeMeetingsAttendedCount</span></span>    | <span data-ttu-id="42678-164">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-164">Int64</span></span>             | <span data-ttu-id="42678-165">用户参与的一次计划会议的数量。</span><span class="sxs-lookup"><span data-stu-id="42678-165">The number of the one-time scheduled meetings a user participated in.</span></span> |
| <span data-ttu-id="42678-166">scheduledRecurringMeetingsOrganizedCount</span><span class="sxs-lookup"><span data-stu-id="42678-166">scheduledRecurringMeetingsOrganizedCount</span></span> | <span data-ttu-id="42678-167">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-167">Int64</span></span>             | <span data-ttu-id="42678-168">用户组织的定期会议数。</span><span class="sxs-lookup"><span data-stu-id="42678-168">The number of recurring meetings a user organized.</span></span>           |
| <span data-ttu-id="42678-169">scheduledRecurringMeetingsAttendedCount</span><span class="sxs-lookup"><span data-stu-id="42678-169">scheduledRecurringMeetingsAttendedCount</span></span>  | <span data-ttu-id="42678-170">Int64</span><span class="sxs-lookup"><span data-stu-id="42678-170">Int64</span></span>             | <span data-ttu-id="42678-171">用户参与的定期会议的数量。</span><span class="sxs-lookup"><span data-stu-id="42678-171">The number of the recurring meetings a user participated in.</span></span> |
| <span data-ttu-id="42678-172">audioDuration</span><span class="sxs-lookup"><span data-stu-id="42678-172">audioDuration</span></span>                            | <span data-ttu-id="42678-173">持续时间</span><span class="sxs-lookup"><span data-stu-id="42678-173">Duration</span></span>          | <span data-ttu-id="42678-174">用户参与的音频持续时间。</span><span class="sxs-lookup"><span data-stu-id="42678-174">Audio duration the user participated in.</span></span>                     |
| <span data-ttu-id="42678-175">videoDuration</span><span class="sxs-lookup"><span data-stu-id="42678-175">videoDuration</span></span>                            | <span data-ttu-id="42678-176">持续时间</span><span class="sxs-lookup"><span data-stu-id="42678-176">Duration</span></span>          | <span data-ttu-id="42678-177">用户参与的视频持续时间。</span><span class="sxs-lookup"><span data-stu-id="42678-177">Video duration the user participated in.</span></span>                     |
| <span data-ttu-id="42678-178">screenShareDuration</span><span class="sxs-lookup"><span data-stu-id="42678-178">screenShareDuration</span></span>                      | <span data-ttu-id="42678-179">持续时间</span><span class="sxs-lookup"><span data-stu-id="42678-179">Duration</span></span>          | <span data-ttu-id="42678-180">用户参与的屏幕共享持续时间。</span><span class="sxs-lookup"><span data-stu-id="42678-180">Screen sharing duration the user participated in.</span></span>            |
| <span data-ttu-id="42678-181">hasOtherAction</span><span class="sxs-lookup"><span data-stu-id="42678-181">hasOtherAction</span></span>                           | <span data-ttu-id="42678-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="42678-182">Boolean</span></span>           | <span data-ttu-id="42678-183">用户处于活动状态，但执行了除报告中提供的公开操作类型外的其他活动 (发送或回复频道消息和聊天消息、安排或参与一对一通话和会议) 。</span><span class="sxs-lookup"><span data-stu-id="42678-183">The User is active but has performed other activities than exposed action types offered in the report (sending or replying to channel messages and chat messages, scheduling or participating in 1:1 calls and meetings).</span></span> <span data-ttu-id="42678-184">示例操作包括用户更改 Teams 状态或 Teams 状态消息或打开频道消息帖子但不回复的情况。</span><span class="sxs-lookup"><span data-stu-id="42678-184">Examples actions are when a user changes the Teams status or the Teams status message or opens a Channel Message post but does not reply.</span></span> |
| <span data-ttu-id="42678-185">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="42678-185">reportPeriod</span></span>                             | <span data-ttu-id="42678-186">String</span><span class="sxs-lookup"><span data-stu-id="42678-186">String</span></span>            | <span data-ttu-id="42678-187">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="42678-187">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="42678-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42678-188">JSON representation</span></span>

<span data-ttu-id="42678-189">下面是资源的 JSON 表示。</span><span class="sxs-lookup"><span data-stu-id="42678-189">The following is a JSON representaion of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "assignedProducts": ["String"],
  "teamChatMessageCount": 1024, 
  "privateChatMessageCount": 1024, 
  "callCount": 1024, 
  "meetingCount": 1024, 
  "meetingsOrganizedCount": 1024, 
  "meetingsAttendedCount": 1024, 
  "adHocMeetingsOrganizedCount": 1024, 
  "adHocMeetingsAttendedCount": 1024, 
  "scheduledOneTimeMeetingsOrganizedCount": 1024, 
  "scheduledOneTimeMeetingsAttendedCount": 1024, 
  "scheduledRecurringMeetingsOrganizedCount": 1024, 
  "scheduledRecurringMeetingsAttendedCount": 1024, 
  "audioDuration": "Duration", 
  "videoDuration": "Duration", 
  "screenShareDuration": "Duration", 
  "hasOtherAction": true, 
  "reportPeriod": "String"
}
```


