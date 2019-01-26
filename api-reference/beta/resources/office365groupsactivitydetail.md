---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575116"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="cb3a4-103">office365GroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb3a4-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="cb3a4-104">属性</span><span class="sxs-lookup"><span data-stu-id="cb3a4-104">Properties</span></span>

| <span data-ttu-id="cb3a4-105">属性</span><span class="sxs-lookup"><span data-stu-id="cb3a4-105">Property</span></span>                          | <span data-ttu-id="cb3a4-106">类型</span><span class="sxs-lookup"><span data-stu-id="cb3a4-106">Type</span></span>    | <span data-ttu-id="cb3a4-107">说明</span><span class="sxs-lookup"><span data-stu-id="cb3a4-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="cb3a4-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="cb3a4-108">reportRefreshDate</span></span>                 | <span data-ttu-id="cb3a4-109">Date</span><span class="sxs-lookup"><span data-stu-id="cb3a4-109">Date</span></span>    | <span data-ttu-id="cb3a4-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="cb3a4-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="cb3a4-111">groupDisplayName</span></span>                  | <span data-ttu-id="cb3a4-112">String</span><span class="sxs-lookup"><span data-stu-id="cb3a4-112">String</span></span>  | <span data-ttu-id="cb3a4-113">组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-113">The display name of the group.</span></span>           |
| <span data-ttu-id="cb3a4-114">被</span><span class="sxs-lookup"><span data-stu-id="cb3a4-114">isDeleted</span></span>                         | <span data-ttu-id="cb3a4-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="cb3a4-115">Boolean</span></span> | <span data-ttu-id="cb3a4-116">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="cb3a4-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cb3a4-117">ownerPrincipalName</span></span>                | <span data-ttu-id="cb3a4-118">String</span><span class="sxs-lookup"><span data-stu-id="cb3a4-118">String</span></span>  | <span data-ttu-id="cb3a4-119">组的所有者主体名称。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="cb3a4-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="cb3a4-120">lastActivityDate</span></span>                  | <span data-ttu-id="cb3a4-121">Date</span><span class="sxs-lookup"><span data-stu-id="cb3a4-121">Date</span></span>    | <span data-ttu-id="cb3a4-122">以下方案的最后一个活动日期： 组邮箱收到电子邮件;用户可以查看、 编辑、 共享，或同步中 SharePoint 文档库; 文件用户查看 SharePoint 页面; 例如：用户发布、 读取或喜欢 Yammer 组中的邮件。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="cb3a4-123">groupType</span><span class="sxs-lookup"><span data-stu-id="cb3a4-123">groupType</span></span>                         | <span data-ttu-id="cb3a4-124">String</span><span class="sxs-lookup"><span data-stu-id="cb3a4-124">String</span></span>  | <span data-ttu-id="cb3a4-125">组类型。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-125">The group type.</span></span> <span data-ttu-id="cb3a4-126">可能的值为：**公共**或**专用**。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="cb3a4-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-127">memberCount</span></span>                       | <span data-ttu-id="cb3a4-128">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-128">Int64</span></span>   | <span data-ttu-id="cb3a4-129">组成员计数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-129">The group member count.</span></span>                  |
| <span data-ttu-id="cb3a4-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-130">externalMemberCount</span></span>               | <span data-ttu-id="cb3a4-131">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-131">Int64</span></span>   | <span data-ttu-id="cb3a4-132">组外部成员计数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-132">The group external member count.</span></span>         |
| <span data-ttu-id="cb3a4-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="cb3a4-134">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-134">Int64</span></span>   | <span data-ttu-id="cb3a4-135">组邮箱收到的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="cb3a4-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="cb3a4-137">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-137">Int64</span></span>   | <span data-ttu-id="cb3a4-138">SharePoint 组网站中的活动文件数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="cb3a4-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="cb3a4-140">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-140">Int64</span></span>   | <span data-ttu-id="cb3a4-141">发布到 Yammer 组的消息数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="cb3a4-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="cb3a4-143">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-143">Int64</span></span>   | <span data-ttu-id="cb3a4-144">Yammer 组中读取的消息数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="cb3a4-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="cb3a4-146">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-146">Int64</span></span>   | <span data-ttu-id="cb3a4-147">喜欢 Yammer 组中的消息数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="cb3a4-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="cb3a4-149">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-149">Int64</span></span>   | <span data-ttu-id="cb3a4-150">组邮箱中的项目数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="cb3a4-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="cb3a4-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="cb3a4-152">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-152">Int64</span></span>   | <span data-ttu-id="cb3a4-153">使用的组邮箱的存储。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="cb3a4-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="cb3a4-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="cb3a4-155">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-155">Int64</span></span>   | <span data-ttu-id="cb3a4-156">SharePoint 组网站中的文件总数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="cb3a4-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="cb3a4-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="cb3a4-158">Int64</span><span class="sxs-lookup"><span data-stu-id="cb3a4-158">Int64</span></span>   | <span data-ttu-id="cb3a4-159">使用 SharePoint 组网站的存储。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="cb3a4-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="cb3a4-160">reportPeriod</span></span>                      | <span data-ttu-id="cb3a4-161">String</span><span class="sxs-lookup"><span data-stu-id="cb3a4-161">String</span></span>  | <span data-ttu-id="cb3a4-162">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="cb3a4-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb3a4-163">JSON representation</span></span>

<span data-ttu-id="cb3a4-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb3a4-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
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
