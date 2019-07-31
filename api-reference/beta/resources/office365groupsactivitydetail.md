---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: dfc45c4973194d26c1830f8c36d3bf3b407d2e3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009501"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="ae319-103">office365GroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae319-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="ae319-104">属性</span><span class="sxs-lookup"><span data-stu-id="ae319-104">Properties</span></span>

| <span data-ttu-id="ae319-105">属性</span><span class="sxs-lookup"><span data-stu-id="ae319-105">Property</span></span>                          | <span data-ttu-id="ae319-106">类型</span><span class="sxs-lookup"><span data-stu-id="ae319-106">Type</span></span>    | <span data-ttu-id="ae319-107">说明</span><span class="sxs-lookup"><span data-stu-id="ae319-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="ae319-108">groupId</span><span class="sxs-lookup"><span data-stu-id="ae319-108">groupId</span></span>                           | <span data-ttu-id="ae319-109">String</span><span class="sxs-lookup"><span data-stu-id="ae319-109">String</span></span>  | <span data-ttu-id="ae319-110">组 id。</span><span class="sxs-lookup"><span data-stu-id="ae319-110">The group id.</span></span>          |
| <span data-ttu-id="ae319-111">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="ae319-111">reportRefreshDate</span></span>                 | <span data-ttu-id="ae319-112">日期</span><span class="sxs-lookup"><span data-stu-id="ae319-112">Date</span></span>    | <span data-ttu-id="ae319-113">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="ae319-113">The latest date of the content.</span></span>          |
| <span data-ttu-id="ae319-114">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="ae319-114">groupDisplayName</span></span>                  | <span data-ttu-id="ae319-115">String</span><span class="sxs-lookup"><span data-stu-id="ae319-115">String</span></span>  | <span data-ttu-id="ae319-116">组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ae319-116">The display name of the group.</span></span>           |
| <span data-ttu-id="ae319-117">isDeleted</span><span class="sxs-lookup"><span data-stu-id="ae319-117">isDeleted</span></span>                         | <span data-ttu-id="ae319-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae319-118">Boolean</span></span> | <span data-ttu-id="ae319-119">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="ae319-119">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="ae319-120">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae319-120">ownerPrincipalName</span></span>                | <span data-ttu-id="ae319-121">String</span><span class="sxs-lookup"><span data-stu-id="ae319-121">String</span></span>  | <span data-ttu-id="ae319-122">组所有者的主体名称。</span><span class="sxs-lookup"><span data-stu-id="ae319-122">The group owner principal name.</span></span>          |
| <span data-ttu-id="ae319-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="ae319-123">lastActivityDate</span></span>                  | <span data-ttu-id="ae319-124">日期</span><span class="sxs-lookup"><span data-stu-id="ae319-124">Date</span></span>    | <span data-ttu-id="ae319-125">以下应用场景的上次活动日期: 组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。</span><span class="sxs-lookup"><span data-stu-id="ae319-125">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="ae319-126">groupType</span><span class="sxs-lookup"><span data-stu-id="ae319-126">groupType</span></span>                         | <span data-ttu-id="ae319-127">String</span><span class="sxs-lookup"><span data-stu-id="ae319-127">String</span></span>  | <span data-ttu-id="ae319-128">组类型。</span><span class="sxs-lookup"><span data-stu-id="ae319-128">The group type.</span></span> <span data-ttu-id="ae319-129">可能的值是: **Public**或**Private**。</span><span class="sxs-lookup"><span data-stu-id="ae319-129">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="ae319-130">memberCount</span><span class="sxs-lookup"><span data-stu-id="ae319-130">memberCount</span></span>                       | <span data-ttu-id="ae319-131">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-131">Int64</span></span>   | <span data-ttu-id="ae319-132">组成员计数。</span><span class="sxs-lookup"><span data-stu-id="ae319-132">The group member count.</span></span>                  |
| <span data-ttu-id="ae319-133">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="ae319-133">externalMemberCount</span></span>               | <span data-ttu-id="ae319-134">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-134">Int64</span></span>   | <span data-ttu-id="ae319-135">Group 外部成员计数。</span><span class="sxs-lookup"><span data-stu-id="ae319-135">The group external member count.</span></span>         |
| <span data-ttu-id="ae319-136">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="ae319-136">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="ae319-137">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-137">Int64</span></span>   | <span data-ttu-id="ae319-138">组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="ae319-138">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="ae319-139">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="ae319-139">sharePointActiveFileCount</span></span>         | <span data-ttu-id="ae319-140">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-140">Int64</span></span>   | <span data-ttu-id="ae319-141">SharePoint 组网站中的活动文件数。</span><span class="sxs-lookup"><span data-stu-id="ae319-141">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="ae319-142">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="ae319-142">yammerPostedMessageCount</span></span>          | <span data-ttu-id="ae319-143">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-143">Int64</span></span>   | <span data-ttu-id="ae319-144">发布到 Yammer 组的邮件数。</span><span class="sxs-lookup"><span data-stu-id="ae319-144">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="ae319-145">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="ae319-145">yammerReadMessageCount</span></span>            | <span data-ttu-id="ae319-146">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-146">Int64</span></span>   | <span data-ttu-id="ae319-147">Yammer 组中读取的邮件数。</span><span class="sxs-lookup"><span data-stu-id="ae319-147">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="ae319-148">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="ae319-148">yammerLikedMessageCount</span></span>           | <span data-ttu-id="ae319-149">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-149">Int64</span></span>   | <span data-ttu-id="ae319-150">Yammer 组中的已赞邮件数。</span><span class="sxs-lookup"><span data-stu-id="ae319-150">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="ae319-151">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="ae319-151">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="ae319-152">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-152">Int64</span></span>   | <span data-ttu-id="ae319-153">组邮箱中的项目数。</span><span class="sxs-lookup"><span data-stu-id="ae319-153">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="ae319-154">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ae319-154">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="ae319-155">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-155">Int64</span></span>   | <span data-ttu-id="ae319-156">组邮箱所使用的存储。</span><span class="sxs-lookup"><span data-stu-id="ae319-156">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="ae319-157">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="ae319-157">sharePointTotalFileCount</span></span>          | <span data-ttu-id="ae319-158">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-158">Int64</span></span>   | <span data-ttu-id="ae319-159">SharePoint 组网站中的总文件数。</span><span class="sxs-lookup"><span data-stu-id="ae319-159">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="ae319-160">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="ae319-160">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="ae319-161">Int64</span><span class="sxs-lookup"><span data-stu-id="ae319-161">Int64</span></span>   | <span data-ttu-id="ae319-162">SharePoint 组网站所使用的存储区。</span><span class="sxs-lookup"><span data-stu-id="ae319-162">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="ae319-163">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="ae319-163">reportPeriod</span></span>                      | <span data-ttu-id="ae319-164">String</span><span class="sxs-lookup"><span data-stu-id="ae319-164">String</span></span>  | <span data-ttu-id="ae319-165">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="ae319-165">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="ae319-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae319-166">JSON representation</span></span>

<span data-ttu-id="ae319-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae319-167">The following is a JSON representation of the resource.</span></span>

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
