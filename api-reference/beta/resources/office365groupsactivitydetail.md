---
title: office365GroupsActivityDetail 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: d517763fdfcbf046c36fc944d229b9a15b0cb8fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522447"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="d9c79-103">office365GroupsActivityDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9c79-103">office365GroupsActivityDetail resource type</span></span>

<span data-ttu-id="d9c79-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d9c79-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="d9c79-105">属性</span><span class="sxs-lookup"><span data-stu-id="d9c79-105">Properties</span></span>

| <span data-ttu-id="d9c79-106">属性</span><span class="sxs-lookup"><span data-stu-id="d9c79-106">Property</span></span>                          | <span data-ttu-id="d9c79-107">类型</span><span class="sxs-lookup"><span data-stu-id="d9c79-107">Type</span></span>    | <span data-ttu-id="d9c79-108">说明</span><span class="sxs-lookup"><span data-stu-id="d9c79-108">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="d9c79-109">groupId</span><span class="sxs-lookup"><span data-stu-id="d9c79-109">groupId</span></span>                           | <span data-ttu-id="d9c79-110">String</span><span class="sxs-lookup"><span data-stu-id="d9c79-110">String</span></span>  | <span data-ttu-id="d9c79-111">组 id。</span><span class="sxs-lookup"><span data-stu-id="d9c79-111">The group id.</span></span>          |
| <span data-ttu-id="d9c79-112">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d9c79-112">reportRefreshDate</span></span>                 | <span data-ttu-id="d9c79-113">日期</span><span class="sxs-lookup"><span data-stu-id="d9c79-113">Date</span></span>    | <span data-ttu-id="d9c79-114">内容的最新日期。</span><span class="sxs-lookup"><span data-stu-id="d9c79-114">The latest date of the content.</span></span>          |
| <span data-ttu-id="d9c79-115">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="d9c79-115">groupDisplayName</span></span>                  | <span data-ttu-id="d9c79-116">String</span><span class="sxs-lookup"><span data-stu-id="d9c79-116">String</span></span>  | <span data-ttu-id="d9c79-117">组的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d9c79-117">The display name of the group.</span></span>           |
| <span data-ttu-id="d9c79-118">isDeleted</span><span class="sxs-lookup"><span data-stu-id="d9c79-118">isDeleted</span></span>                         | <span data-ttu-id="d9c79-119">布尔</span><span class="sxs-lookup"><span data-stu-id="d9c79-119">Boolean</span></span> | <span data-ttu-id="d9c79-120">此用户是否已被删除或软删除。</span><span class="sxs-lookup"><span data-stu-id="d9c79-120">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="d9c79-121">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d9c79-121">ownerPrincipalName</span></span>                | <span data-ttu-id="d9c79-122">String</span><span class="sxs-lookup"><span data-stu-id="d9c79-122">String</span></span>  | <span data-ttu-id="d9c79-123">组所有者的主体名称。</span><span class="sxs-lookup"><span data-stu-id="d9c79-123">The group owner principal name.</span></span>          |
| <span data-ttu-id="d9c79-124">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="d9c79-124">lastActivityDate</span></span>                  | <span data-ttu-id="d9c79-125">日期</span><span class="sxs-lookup"><span data-stu-id="d9c79-125">Date</span></span>    | <span data-ttu-id="d9c79-126">以下应用场景的上次活动日期：组邮箱收到电子邮件;用户在 SharePoint 文档库中查看、编辑、共享或同步文件;用户查看了 SharePoint 页面;用户在 Yammer 组中投递、阅读或赞了邮件。</span><span class="sxs-lookup"><span data-stu-id="d9c79-126">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="d9c79-127">groupType</span><span class="sxs-lookup"><span data-stu-id="d9c79-127">groupType</span></span>                         | <span data-ttu-id="d9c79-128">String</span><span class="sxs-lookup"><span data-stu-id="d9c79-128">String</span></span>  | <span data-ttu-id="d9c79-129">组类型。</span><span class="sxs-lookup"><span data-stu-id="d9c79-129">The group type.</span></span> <span data-ttu-id="d9c79-130">可能的值是： **Public**或**Private**。</span><span class="sxs-lookup"><span data-stu-id="d9c79-130">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="d9c79-131">memberCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-131">memberCount</span></span>                       | <span data-ttu-id="d9c79-132">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-132">Int64</span></span>   | <span data-ttu-id="d9c79-133">组成员计数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-133">The group member count.</span></span>                  |
| <span data-ttu-id="d9c79-134">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-134">externalMemberCount</span></span>               | <span data-ttu-id="d9c79-135">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-135">Int64</span></span>   | <span data-ttu-id="d9c79-136">Group 外部成员计数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-136">The group external member count.</span></span>         |
| <span data-ttu-id="d9c79-137">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-137">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="d9c79-138">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-138">Int64</span></span>   | <span data-ttu-id="d9c79-139">组邮箱接收的电子邮件数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-139">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="d9c79-140">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-140">sharePointActiveFileCount</span></span>         | <span data-ttu-id="d9c79-141">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-141">Int64</span></span>   | <span data-ttu-id="d9c79-142">SharePoint 组网站中的活动文件数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-142">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="d9c79-143">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-143">yammerPostedMessageCount</span></span>          | <span data-ttu-id="d9c79-144">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-144">Int64</span></span>   | <span data-ttu-id="d9c79-145">发布到 Yammer 组的邮件数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-145">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="d9c79-146">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-146">yammerReadMessageCount</span></span>            | <span data-ttu-id="d9c79-147">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-147">Int64</span></span>   | <span data-ttu-id="d9c79-148">Yammer 组中读取的邮件数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-148">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="d9c79-149">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-149">yammerLikedMessageCount</span></span>           | <span data-ttu-id="d9c79-150">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-150">Int64</span></span>   | <span data-ttu-id="d9c79-151">Yammer 组中的已赞邮件数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-151">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="d9c79-152">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-152">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="d9c79-153">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-153">Int64</span></span>   | <span data-ttu-id="d9c79-154">组邮箱中的项目数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-154">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="d9c79-155">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d9c79-155">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="d9c79-156">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-156">Int64</span></span>   | <span data-ttu-id="d9c79-157">组邮箱所使用的存储。</span><span class="sxs-lookup"><span data-stu-id="d9c79-157">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="d9c79-158">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="d9c79-158">sharePointTotalFileCount</span></span>          | <span data-ttu-id="d9c79-159">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-159">Int64</span></span>   | <span data-ttu-id="d9c79-160">SharePoint 组网站中的总文件数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-160">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="d9c79-161">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="d9c79-161">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="d9c79-162">Int64</span><span class="sxs-lookup"><span data-stu-id="d9c79-162">Int64</span></span>   | <span data-ttu-id="d9c79-163">SharePoint 组网站所使用的存储区。</span><span class="sxs-lookup"><span data-stu-id="d9c79-163">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="d9c79-164">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d9c79-164">reportPeriod</span></span>                      | <span data-ttu-id="d9c79-165">String</span><span class="sxs-lookup"><span data-stu-id="d9c79-165">String</span></span>  | <span data-ttu-id="d9c79-166">报告覆盖的天数。</span><span class="sxs-lookup"><span data-stu-id="d9c79-166">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d9c79-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9c79-167">JSON representation</span></span>

<span data-ttu-id="d9c79-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9c79-168">The following is a JSON representation of the resource.</span></span>

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
