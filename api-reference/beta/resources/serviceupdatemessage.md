---
title: serviceUpdateMessage 资源类型
description: 表示服务中的更改通知。
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: e8bea9b3c44f99d5be0d87b01d47db4505873681
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109093"
---
# <a name="serviceupdatemessage-resource-type"></a><span data-ttu-id="78294-103">serviceUpdateMessage 资源类型</span><span class="sxs-lookup"><span data-stu-id="78294-103">serviceUpdateMessage resource type</span></span>

<span data-ttu-id="78294-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78294-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78294-105">表示有关服务中更改的公告。</span><span class="sxs-lookup"><span data-stu-id="78294-105">Represents the announcements about changes in a service.</span></span>

<span data-ttu-id="78294-106">表示公告，如产品的主要更新、新功能;例如，发布新的Windows功能。</span><span class="sxs-lookup"><span data-stu-id="78294-106">Represents announcements such as major updates, new features in a product; for example, the publication of a new Windows feature.</span></span>

<span data-ttu-id="78294-107">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="78294-107">Inherits from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="78294-108">方法</span><span class="sxs-lookup"><span data-stu-id="78294-108">Methods</span></span>
|<span data-ttu-id="78294-109">方法</span><span class="sxs-lookup"><span data-stu-id="78294-109">Method</span></span>|<span data-ttu-id="78294-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="78294-110">Return type</span></span>|<span data-ttu-id="78294-111">说明</span><span class="sxs-lookup"><span data-stu-id="78294-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78294-112">获取 serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="78294-112">Get serviceUpdateMessage</span></span>](../api/serviceupdatemessage-get.md)|[<span data-ttu-id="78294-113">serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="78294-113">serviceUpdateMessage</span></span>](../resources/serviceupdatemessage.md)|<span data-ttu-id="78294-114">检索 [serviceUpdateMessage 对象的属性和](../resources/serviceupdatemessage.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="78294-114">Retrieve the properties and relationships of a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object.</span></span> |
|[<span data-ttu-id="78294-115">markRead</span><span class="sxs-lookup"><span data-stu-id="78294-115">markRead</span></span>](../api/serviceupdatemessage-markread.md)|<span data-ttu-id="78294-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="78294-116">Boolean</span></span>|<span data-ttu-id="78294-117">将 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的列表标记为 **已** 登录用户的已读。</span><span class="sxs-lookup"><span data-stu-id="78294-117">Mark a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s as **read** for the signed in user.</span></span>|
|[<span data-ttu-id="78294-118">markUnread</span><span class="sxs-lookup"><span data-stu-id="78294-118">markUnread</span></span>](../api/serviceupdatemessage-markunread.md)|<span data-ttu-id="78294-119">布尔值</span><span class="sxs-lookup"><span data-stu-id="78294-119">Boolean</span></span>|<span data-ttu-id="78294-120">对于登录用户，将 [serviceUpdateMessage](../resources/serviceupdatemessage.md)**列表标记为未** 读。</span><span class="sxs-lookup"><span data-stu-id="78294-120">Mark a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s as **unread** for the signed in user.</span></span>|
|[<span data-ttu-id="78294-121">archive</span><span class="sxs-lookup"><span data-stu-id="78294-121">archive</span></span>](../api/serviceupdatemessage-archive.md)|<span data-ttu-id="78294-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="78294-122">Boolean</span></span>|<span data-ttu-id="78294-123">存档已登录 [用户的 serviceUpdateMessage](../resources/serviceupdatemessage.md)列表。</span><span class="sxs-lookup"><span data-stu-id="78294-123">Archive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|
|[<span data-ttu-id="78294-124">unarchive</span><span class="sxs-lookup"><span data-stu-id="78294-124">unarchive</span></span>](../api/serviceupdatemessage-unarchive.md)|<span data-ttu-id="78294-125">布尔值</span><span class="sxs-lookup"><span data-stu-id="78294-125">Boolean</span></span>|<span data-ttu-id="78294-126">取消存档已登录用户的 [serviceUpdateMessage](../resources/serviceupdatemessage.md)列表。</span><span class="sxs-lookup"><span data-stu-id="78294-126">Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|
|[<span data-ttu-id="78294-127">favorite</span><span class="sxs-lookup"><span data-stu-id="78294-127">favorite</span></span>](../api/serviceupdatemessage-favorite.md)|<span data-ttu-id="78294-128">布尔值</span><span class="sxs-lookup"><span data-stu-id="78294-128">Boolean</span></span>|<span data-ttu-id="78294-129">将 [serviceUpdateMessage](../resources/serviceupdatemessage.md)列表的状态更改为为登录用户收藏。</span><span class="sxs-lookup"><span data-stu-id="78294-129">Change the status of a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s to favorite for the signed in user.</span></span>|
|[<span data-ttu-id="78294-130">unfavorite</span><span class="sxs-lookup"><span data-stu-id="78294-130">unfavorite</span></span>](../api/serviceupdatemessage-unfavorite.md)|<span data-ttu-id="78294-131">布尔值</span><span class="sxs-lookup"><span data-stu-id="78294-131">Boolean</span></span>|<span data-ttu-id="78294-132">删除已登录用户的 [serviceUpdateMessage](../resources/serviceupdatemessage.md)的收藏夹状态。</span><span class="sxs-lookup"><span data-stu-id="78294-132">Remove the favorite status of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|

## <a name="properties"></a><span data-ttu-id="78294-133">属性</span><span class="sxs-lookup"><span data-stu-id="78294-133">Properties</span></span>
|<span data-ttu-id="78294-134">属性</span><span class="sxs-lookup"><span data-stu-id="78294-134">Property</span></span>|<span data-ttu-id="78294-135">类型</span><span class="sxs-lookup"><span data-stu-id="78294-135">Type</span></span>|<span data-ttu-id="78294-136">说明</span><span class="sxs-lookup"><span data-stu-id="78294-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78294-137">actionRequiredByDateTime</span><span class="sxs-lookup"><span data-stu-id="78294-137">actionRequiredByDateTime</span></span>|<span data-ttu-id="78294-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78294-138">DateTimeOffset</span></span>|<span data-ttu-id="78294-139">邮件操作的预期截止时间。</span><span class="sxs-lookup"><span data-stu-id="78294-139">The expected deadline of the action for the message.</span></span>|
|<span data-ttu-id="78294-140">body</span><span class="sxs-lookup"><span data-stu-id="78294-140">body</span></span>|[<span data-ttu-id="78294-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="78294-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="78294-142">服务邮件正文的内容类型和内容。</span><span class="sxs-lookup"><span data-stu-id="78294-142">The content type and content of the service message body.</span></span>|
|<span data-ttu-id="78294-143">“类别”</span><span class="sxs-lookup"><span data-stu-id="78294-143">category</span></span>|<span data-ttu-id="78294-144">serviceUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="78294-144">serviceUpdateCategory</span></span>|<span data-ttu-id="78294-145">服务邮件类别。</span><span class="sxs-lookup"><span data-stu-id="78294-145">The service message category.</span></span> <span data-ttu-id="78294-146">可取值为：`preventOrFixIssue`、`planForChange`、`stayInformed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="78294-146">Possible values are: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="78294-147">详细信息</span><span class="sxs-lookup"><span data-stu-id="78294-147">details</span></span>|<span data-ttu-id="78294-148">collection ([keyValuePair](../resources/keyvaluepair.md)) </span><span class="sxs-lookup"><span data-stu-id="78294-148">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="78294-149">有关服务邮件的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="78294-149">Additional details about service message.</span></span> <span data-ttu-id="78294-150">此属性不支持筛选器。</span><span class="sxs-lookup"><span data-stu-id="78294-150">This property doesn't support filters.</span></span> <span data-ttu-id="78294-151">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="78294-151">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="78294-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="78294-152">endDateTime</span></span>|<span data-ttu-id="78294-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78294-153">DateTimeOffset</span></span>|<span data-ttu-id="78294-154">服务消息的结束时间。</span><span class="sxs-lookup"><span data-stu-id="78294-154">The end time of the service message.</span></span> <span data-ttu-id="78294-155">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="78294-155">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="78294-156">id</span><span class="sxs-lookup"><span data-stu-id="78294-156">id</span></span>|<span data-ttu-id="78294-157">字符串</span><span class="sxs-lookup"><span data-stu-id="78294-157">String</span></span>|<span data-ttu-id="78294-158">服务消息的 ID。</span><span class="sxs-lookup"><span data-stu-id="78294-158">The id of the service message.</span></span> <span data-ttu-id="78294-159">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="78294-159">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="78294-160">isMajorChange</span><span class="sxs-lookup"><span data-stu-id="78294-160">isMajorChange</span></span>|<span data-ttu-id="78294-161">布尔值</span><span class="sxs-lookup"><span data-stu-id="78294-161">Boolean</span></span>|<span data-ttu-id="78294-162">指示消息是否描述服务的主要更新。</span><span class="sxs-lookup"><span data-stu-id="78294-162">Indicates whether the message describes a major update for the service.</span></span>|
|<span data-ttu-id="78294-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78294-163">lastModifiedDateTime</span></span>|<span data-ttu-id="78294-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78294-164">DateTimeOffset</span></span>|<span data-ttu-id="78294-165">服务邮件的上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="78294-165">The last modified time of the service message.</span></span> <span data-ttu-id="78294-166">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="78294-166">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="78294-167">服务</span><span class="sxs-lookup"><span data-stu-id="78294-167">services</span></span>|<span data-ttu-id="78294-168">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="78294-168">Collection(string)</span></span>|<span data-ttu-id="78294-169">服务消息影响的服务。</span><span class="sxs-lookup"><span data-stu-id="78294-169">The affected services by the service message.</span></span>|
|<span data-ttu-id="78294-170">severity</span><span class="sxs-lookup"><span data-stu-id="78294-170">severity</span></span>|<span data-ttu-id="78294-171">serviceUpdateSeverity</span><span class="sxs-lookup"><span data-stu-id="78294-171">serviceUpdateSeverity</span></span>|<span data-ttu-id="78294-172">服务邮件的严重性。</span><span class="sxs-lookup"><span data-stu-id="78294-172">The severity of the service message.</span></span> <span data-ttu-id="78294-173">可取值为：`normal`、`high`、`critical`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="78294-173">Possible values are: `normal`, `high`, `critical`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="78294-174">startDateTime</span><span class="sxs-lookup"><span data-stu-id="78294-174">startDateTime</span></span>|<span data-ttu-id="78294-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78294-175">DateTimeOffset</span></span>|<span data-ttu-id="78294-176">服务消息的开始时间。</span><span class="sxs-lookup"><span data-stu-id="78294-176">The start time of the service message.</span></span> <span data-ttu-id="78294-177">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="78294-177">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="78294-178">标记</span><span class="sxs-lookup"><span data-stu-id="78294-178">tags</span></span>|<span data-ttu-id="78294-179">集合 (字符串) </span><span class="sxs-lookup"><span data-stu-id="78294-179">Collection(string)</span></span>|<span data-ttu-id="78294-180">服务邮件的标记集合。</span><span class="sxs-lookup"><span data-stu-id="78294-180">A collection of tags for the service message.</span></span>|
|<span data-ttu-id="78294-181">title</span><span class="sxs-lookup"><span data-stu-id="78294-181">title</span></span>|<span data-ttu-id="78294-182">String</span><span class="sxs-lookup"><span data-stu-id="78294-182">String</span></span>|<span data-ttu-id="78294-183">服务消息的标题。</span><span class="sxs-lookup"><span data-stu-id="78294-183">The title of the service message.</span></span> <span data-ttu-id="78294-184">继承自 [serviceAnnouncementBase](../resources/serviceannouncementbase.md)。</span><span class="sxs-lookup"><span data-stu-id="78294-184">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="78294-185">viewPoint</span><span class="sxs-lookup"><span data-stu-id="78294-185">viewPoint</span></span>|[<span data-ttu-id="78294-186">serviceUpdateMessageViewpoint</span><span class="sxs-lookup"><span data-stu-id="78294-186">serviceUpdateMessageViewpoint</span></span>](../resources/serviceupdatemessageviewpoint.md)|<span data-ttu-id="78294-187">表示服务消息的用户视图点数据。</span><span class="sxs-lookup"><span data-stu-id="78294-187">Represents user view points data of the service message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78294-188">关系</span><span class="sxs-lookup"><span data-stu-id="78294-188">Relationships</span></span>
<span data-ttu-id="78294-189">无。</span><span class="sxs-lookup"><span data-stu-id="78294-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78294-190">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78294-190">JSON representation</span></span>
<span data-ttu-id="78294-191">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78294-191">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessage",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "category": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "isMajorChange": "Boolean",
  "actionRequiredByDateTime": "String (timestamp)",
  "services": [
    "String"
  ],
  "viewPoint": {
    "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
  }
}
```

