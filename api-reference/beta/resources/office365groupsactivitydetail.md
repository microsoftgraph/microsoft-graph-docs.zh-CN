---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 2968a3a5459f286e4aac69e2fd606adc1b38e39b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951822"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="d98c8-103">office365GroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d98c8-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d98c8-104">属性</span><span class="sxs-lookup"><span data-stu-id="d98c8-104">Properties</span></span>

| <span data-ttu-id="d98c8-105">属性</span><span class="sxs-lookup"><span data-stu-id="d98c8-105">Property</span></span>                          | <span data-ttu-id="d98c8-106">类型</span><span class="sxs-lookup"><span data-stu-id="d98c8-106">Type</span></span>    | <span data-ttu-id="d98c8-107">说明</span><span class="sxs-lookup"><span data-stu-id="d98c8-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="d98c8-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d98c8-108">reportRefreshDate</span></span>                 | <span data-ttu-id="d98c8-109">日期</span><span class="sxs-lookup"><span data-stu-id="d98c8-109">Date</span></span>    | <span data-ttu-id="d98c8-110">内容最晚日期。</span><span class="sxs-lookup"><span data-stu-id="d98c8-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d98c8-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="d98c8-111">groupDisplayName</span></span>                  | <span data-ttu-id="d98c8-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d98c8-112">String</span></span>  | <span data-ttu-id="d98c8-113">组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d98c8-113">The display name of the group.</span></span>           |
| <span data-ttu-id="d98c8-114">被</span><span class="sxs-lookup"><span data-stu-id="d98c8-114">isDeleted</span></span>                         | <span data-ttu-id="d98c8-115">布尔</span><span class="sxs-lookup"><span data-stu-id="d98c8-115">Boolean</span></span> | <span data-ttu-id="d98c8-116">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="d98c8-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="d98c8-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d98c8-117">ownerPrincipalName</span></span>                | <span data-ttu-id="d98c8-118">字符串</span><span class="sxs-lookup"><span data-stu-id="d98c8-118">String</span></span>  | <span data-ttu-id="d98c8-119">组的所有者主体名称。</span><span class="sxs-lookup"><span data-stu-id="d98c8-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="d98c8-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d98c8-120">lastActivityDate</span></span>                  | <span data-ttu-id="d98c8-121">日期</span><span class="sxs-lookup"><span data-stu-id="d98c8-121">Date</span></span>    | <span data-ttu-id="d98c8-122">以下方案的最后一个活动日期： 组邮箱收到电子邮件;用户可以查看、 编辑、 共享，或同步中 SharePoint 文档库; 文件用户查看 SharePoint 页面; 例如：用户发布、 读取或喜欢 Yammer 组中的邮件。</span><span class="sxs-lookup"><span data-stu-id="d98c8-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="d98c8-123">groupType</span><span class="sxs-lookup"><span data-stu-id="d98c8-123">groupType</span></span>                         | <span data-ttu-id="d98c8-124">字符串</span><span class="sxs-lookup"><span data-stu-id="d98c8-124">String</span></span>  | <span data-ttu-id="d98c8-125">组类型。</span><span class="sxs-lookup"><span data-stu-id="d98c8-125">The group type.</span></span> <span data-ttu-id="d98c8-126">可能的值为：**公共**或**专用**。</span><span class="sxs-lookup"><span data-stu-id="d98c8-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="d98c8-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-127">memberCount</span></span>                       | <span data-ttu-id="d98c8-128">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-128">Int64</span></span>   | <span data-ttu-id="d98c8-129">组成员计数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-129">The group member count.</span></span>                  |
| <span data-ttu-id="d98c8-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-130">externalMemberCount</span></span>               | <span data-ttu-id="d98c8-131">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-131">Int64</span></span>   | <span data-ttu-id="d98c8-132">组外部成员计数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-132">The group external member count.</span></span>         |
| <span data-ttu-id="d98c8-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="d98c8-134">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-134">Int64</span></span>   | <span data-ttu-id="d98c8-135">组邮箱收到的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="d98c8-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="d98c8-137">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-137">Int64</span></span>   | <span data-ttu-id="d98c8-138">SharePoint 组网站中的活动文件数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="d98c8-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="d98c8-140">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-140">Int64</span></span>   | <span data-ttu-id="d98c8-141">发布到 Yammer 组的消息数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="d98c8-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="d98c8-143">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-143">Int64</span></span>   | <span data-ttu-id="d98c8-144">Yammer 组中读取的消息数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="d98c8-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="d98c8-146">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-146">Int64</span></span>   | <span data-ttu-id="d98c8-147">喜欢 Yammer 组中的消息数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="d98c8-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="d98c8-149">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-149">Int64</span></span>   | <span data-ttu-id="d98c8-150">组邮箱中的项目数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="d98c8-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d98c8-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="d98c8-152">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-152">Int64</span></span>   | <span data-ttu-id="d98c8-153">使用的组邮箱的存储。</span><span class="sxs-lookup"><span data-stu-id="d98c8-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="d98c8-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="d98c8-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="d98c8-155">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-155">Int64</span></span>   | <span data-ttu-id="d98c8-156">SharePoint 组网站中的文件总数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="d98c8-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d98c8-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="d98c8-158">Int64</span><span class="sxs-lookup"><span data-stu-id="d98c8-158">Int64</span></span>   | <span data-ttu-id="d98c8-159">使用 SharePoint 组网站的存储。</span><span class="sxs-lookup"><span data-stu-id="d98c8-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="d98c8-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d98c8-160">reportPeriod</span></span>                      | <span data-ttu-id="d98c8-161">字符串</span><span class="sxs-lookup"><span data-stu-id="d98c8-161">String</span></span>  | <span data-ttu-id="d98c8-162">报告涵盖天数。</span><span class="sxs-lookup"><span data-stu-id="d98c8-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d98c8-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d98c8-163">JSON representation</span></span>

<span data-ttu-id="d98c8-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d98c8-164">The following is a JSON representation of the resource.</span></span>

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
