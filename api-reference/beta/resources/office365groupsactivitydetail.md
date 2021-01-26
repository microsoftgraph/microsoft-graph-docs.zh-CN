---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: fe2df5614525f27b294bed93be7f3f9cd8170b30
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981506"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="c1e42-103">office365GroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1e42-103">office365GroupsActivityDetail resource type</span></span>

<span data-ttu-id="c1e42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1e42-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="c1e42-105">属性</span><span class="sxs-lookup"><span data-stu-id="c1e42-105">Properties</span></span>

| <span data-ttu-id="c1e42-106">属性</span><span class="sxs-lookup"><span data-stu-id="c1e42-106">Property</span></span>                          | <span data-ttu-id="c1e42-107">类型</span><span class="sxs-lookup"><span data-stu-id="c1e42-107">Type</span></span>    | <span data-ttu-id="c1e42-108">说明</span><span class="sxs-lookup"><span data-stu-id="c1e42-108">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="c1e42-109">groupId</span><span class="sxs-lookup"><span data-stu-id="c1e42-109">groupId</span></span>                           | <span data-ttu-id="c1e42-110">String</span><span class="sxs-lookup"><span data-stu-id="c1e42-110">String</span></span>  | <span data-ttu-id="c1e42-111">组 ID。</span><span class="sxs-lookup"><span data-stu-id="c1e42-111">The group id.</span></span>          |
| <span data-ttu-id="c1e42-112">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="c1e42-112">reportRefreshDate</span></span>                 | <span data-ttu-id="c1e42-113">日期</span><span class="sxs-lookup"><span data-stu-id="c1e42-113">Date</span></span>    | <span data-ttu-id="c1e42-114">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="c1e42-114">The latest date of the content.</span></span>          |
| <span data-ttu-id="c1e42-115">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="c1e42-115">groupDisplayName</span></span>                  | <span data-ttu-id="c1e42-116">String</span><span class="sxs-lookup"><span data-stu-id="c1e42-116">String</span></span>  | <span data-ttu-id="c1e42-117">组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c1e42-117">The display name of the group.</span></span>           |
| <span data-ttu-id="c1e42-118">isDeleted</span><span class="sxs-lookup"><span data-stu-id="c1e42-118">isDeleted</span></span>                         | <span data-ttu-id="c1e42-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1e42-119">Boolean</span></span> | <span data-ttu-id="c1e42-120">此用户是已删除还是软删除。</span><span class="sxs-lookup"><span data-stu-id="c1e42-120">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="c1e42-121">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c1e42-121">ownerPrincipalName</span></span>                | <span data-ttu-id="c1e42-122">String</span><span class="sxs-lookup"><span data-stu-id="c1e42-122">String</span></span>  | <span data-ttu-id="c1e42-123">组所有者主体名称。</span><span class="sxs-lookup"><span data-stu-id="c1e42-123">The group owner principal name.</span></span>          |
| <span data-ttu-id="c1e42-124">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="c1e42-124">lastActivityDate</span></span>                  | <span data-ttu-id="c1e42-125">日期</span><span class="sxs-lookup"><span data-stu-id="c1e42-125">Date</span></span>    | <span data-ttu-id="c1e42-126">以下方案的最后一个活动日期：组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步的文件;用户查看的 SharePoint 页面;用户发布、阅读或喜欢的 Yammer 组中的消息。</span><span class="sxs-lookup"><span data-stu-id="c1e42-126">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="c1e42-127">groupType</span><span class="sxs-lookup"><span data-stu-id="c1e42-127">groupType</span></span>                         | <span data-ttu-id="c1e42-128">String</span><span class="sxs-lookup"><span data-stu-id="c1e42-128">String</span></span>  | <span data-ttu-id="c1e42-129">组类型。</span><span class="sxs-lookup"><span data-stu-id="c1e42-129">The group type.</span></span> <span data-ttu-id="c1e42-130">可能的值是 **：Public** 或 **Private。**</span><span class="sxs-lookup"><span data-stu-id="c1e42-130">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="c1e42-131">memberCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-131">memberCount</span></span>                       | <span data-ttu-id="c1e42-132">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-132">Int64</span></span>   | <span data-ttu-id="c1e42-133">组的成员计数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-133">The group member count.</span></span>                  |
| <span data-ttu-id="c1e42-134">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-134">externalMemberCount</span></span>               | <span data-ttu-id="c1e42-135">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-135">Int64</span></span>   | <span data-ttu-id="c1e42-136">组外部成员计数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-136">The group external member count.</span></span>         |
| <span data-ttu-id="c1e42-137">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-137">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="c1e42-138">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-138">Int64</span></span>   | <span data-ttu-id="c1e42-139">组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-139">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="c1e42-140">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-140">sharePointActiveFileCount</span></span>         | <span data-ttu-id="c1e42-141">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-141">Int64</span></span>   | <span data-ttu-id="c1e42-142">SharePoint 组网站中的活动文件数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-142">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="c1e42-143">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-143">yammerPostedMessageCount</span></span>          | <span data-ttu-id="c1e42-144">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-144">Int64</span></span>   | <span data-ttu-id="c1e42-145">张贴到 Yammer 组的消息数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-145">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="c1e42-146">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-146">yammerReadMessageCount</span></span>            | <span data-ttu-id="c1e42-147">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-147">Int64</span></span>   | <span data-ttu-id="c1e42-148">Yammer 组中读取的消息数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-148">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="c1e42-149">yammer已用MessageCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-149">yammerLikedMessageCount</span></span>           | <span data-ttu-id="c1e42-150">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-150">Int64</span></span>   | <span data-ttu-id="c1e42-151">Yammer 组中喜欢的消息数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-151">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="c1e42-152">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-152">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="c1e42-153">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-153">Int64</span></span>   | <span data-ttu-id="c1e42-154">组邮箱中的项目数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-154">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="c1e42-155">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c1e42-155">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="c1e42-156">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-156">Int64</span></span>   | <span data-ttu-id="c1e42-157">组邮箱所使用的存储。</span><span class="sxs-lookup"><span data-stu-id="c1e42-157">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="c1e42-158">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="c1e42-158">sharePointTotalFileCount</span></span>          | <span data-ttu-id="c1e42-159">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-159">Int64</span></span>   | <span data-ttu-id="c1e42-160">SharePoint 组网站中的文件总数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-160">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="c1e42-161">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="c1e42-161">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="c1e42-162">Int64</span><span class="sxs-lookup"><span data-stu-id="c1e42-162">Int64</span></span>   | <span data-ttu-id="c1e42-163">SharePoint 组网站所使用的存储。</span><span class="sxs-lookup"><span data-stu-id="c1e42-163">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="c1e42-164">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="c1e42-164">reportPeriod</span></span>                      | <span data-ttu-id="c1e42-165">String</span><span class="sxs-lookup"><span data-stu-id="c1e42-165">String</span></span>  | <span data-ttu-id="c1e42-166">报告涵盖的天数。</span><span class="sxs-lookup"><span data-stu-id="c1e42-166">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="c1e42-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1e42-167">JSON representation</span></span>

<span data-ttu-id="c1e42-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1e42-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```


