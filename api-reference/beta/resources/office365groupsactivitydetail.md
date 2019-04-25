---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581448"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="2cde2-103">office365GroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cde2-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="2cde2-104">属性</span><span class="sxs-lookup"><span data-stu-id="2cde2-104">Properties</span></span>

| <span data-ttu-id="2cde2-105">属性</span><span class="sxs-lookup"><span data-stu-id="2cde2-105">Property</span></span>                          | <span data-ttu-id="2cde2-106">类型</span><span class="sxs-lookup"><span data-stu-id="2cde2-106">Type</span></span>    | <span data-ttu-id="2cde2-107">说明</span><span class="sxs-lookup"><span data-stu-id="2cde2-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="2cde2-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="2cde2-108">reportRefreshDate</span></span>                 | <span data-ttu-id="2cde2-109">Date</span><span class="sxs-lookup"><span data-stu-id="2cde2-109">Date</span></span>    | <span data-ttu-id="2cde2-110">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="2cde2-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="2cde2-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="2cde2-111">groupDisplayName</span></span>                  | <span data-ttu-id="2cde2-112">String</span><span class="sxs-lookup"><span data-stu-id="2cde2-112">String</span></span>  | <span data-ttu-id="2cde2-113">组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2cde2-113">The display name of the group.</span></span>           |
| <span data-ttu-id="2cde2-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="2cde2-114">isDeleted</span></span>                         | <span data-ttu-id="2cde2-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2cde2-115">Boolean</span></span> | <span data-ttu-id="2cde2-116">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="2cde2-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="2cde2-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2cde2-117">ownerPrincipalName</span></span>                | <span data-ttu-id="2cde2-118">String</span><span class="sxs-lookup"><span data-stu-id="2cde2-118">String</span></span>  | <span data-ttu-id="2cde2-119">组所有者的主体名称。</span><span class="sxs-lookup"><span data-stu-id="2cde2-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="2cde2-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="2cde2-120">lastActivityDate</span></span>                  | <span data-ttu-id="2cde2-121">Date</span><span class="sxs-lookup"><span data-stu-id="2cde2-121">Date</span></span>    | <span data-ttu-id="2cde2-122">以下应用场景的上次活动日期: 组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。</span><span class="sxs-lookup"><span data-stu-id="2cde2-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="2cde2-123">groupType</span><span class="sxs-lookup"><span data-stu-id="2cde2-123">groupType</span></span>                         | <span data-ttu-id="2cde2-124">String</span><span class="sxs-lookup"><span data-stu-id="2cde2-124">String</span></span>  | <span data-ttu-id="2cde2-125">组类型。</span><span class="sxs-lookup"><span data-stu-id="2cde2-125">The group type.</span></span> <span data-ttu-id="2cde2-126">可能的值是: **Public**或**Private**。</span><span class="sxs-lookup"><span data-stu-id="2cde2-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="2cde2-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-127">memberCount</span></span>                       | <span data-ttu-id="2cde2-128">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-128">Int64</span></span>   | <span data-ttu-id="2cde2-129">组成员计数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-129">The group member count.</span></span>                  |
| <span data-ttu-id="2cde2-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-130">externalMemberCount</span></span>               | <span data-ttu-id="2cde2-131">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-131">Int64</span></span>   | <span data-ttu-id="2cde2-132">group 外部成员计数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-132">The group external member count.</span></span>         |
| <span data-ttu-id="2cde2-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="2cde2-134">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-134">Int64</span></span>   | <span data-ttu-id="2cde2-135">组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="2cde2-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="2cde2-137">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-137">Int64</span></span>   | <span data-ttu-id="2cde2-138">SharePoint 组网站中的活动文件数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="2cde2-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="2cde2-140">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-140">Int64</span></span>   | <span data-ttu-id="2cde2-141">发布到 Yammer 组的邮件数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="2cde2-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="2cde2-143">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-143">Int64</span></span>   | <span data-ttu-id="2cde2-144">Yammer 组中读取的邮件数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="2cde2-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="2cde2-146">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-146">Int64</span></span>   | <span data-ttu-id="2cde2-147">Yammer 组中的已赞邮件数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="2cde2-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="2cde2-149">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-149">Int64</span></span>   | <span data-ttu-id="2cde2-150">组邮箱中的项目数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="2cde2-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="2cde2-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="2cde2-152">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-152">Int64</span></span>   | <span data-ttu-id="2cde2-153">组邮箱所使用的存储。</span><span class="sxs-lookup"><span data-stu-id="2cde2-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="2cde2-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="2cde2-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="2cde2-155">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-155">Int64</span></span>   | <span data-ttu-id="2cde2-156">SharePoint 组网站中的总文件数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="2cde2-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="2cde2-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="2cde2-158">Int64</span><span class="sxs-lookup"><span data-stu-id="2cde2-158">Int64</span></span>   | <span data-ttu-id="2cde2-159">SharePoint 组网站所使用的存储区。</span><span class="sxs-lookup"><span data-stu-id="2cde2-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="2cde2-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="2cde2-160">reportPeriod</span></span>                      | <span data-ttu-id="2cde2-161">String</span><span class="sxs-lookup"><span data-stu-id="2cde2-161">String</span></span>  | <span data-ttu-id="2cde2-162">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="2cde2-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="2cde2-163">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cde2-163">JSON representation</span></span>

<span data-ttu-id="2cde2-164">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cde2-164">The following is a JSON representation of the resource.</span></span>

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
