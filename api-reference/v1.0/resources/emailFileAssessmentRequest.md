---
title: emailFileAssessmentRequest 资源类型
description: 用于创建和检索电子邮件文件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 30b9f279d543e134d5464fed9753728a4bc04682
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069111"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="f5b00-103">emailFileAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5b00-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="f5b00-104">用于创建和检索从 [threatAssessmentRequest](threatAssessmentRequest.md)派生的电子邮件文件威胁评估。</span><span class="sxs-lookup"><span data-stu-id="f5b00-104">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="f5b00-105">电子邮件文件可以是 .eml 文件类型。</span><span class="sxs-lookup"><span data-stu-id="f5b00-105">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="f5b00-106">方法</span><span class="sxs-lookup"><span data-stu-id="f5b00-106">Methods</span></span>

| <span data-ttu-id="f5b00-107">方法</span><span class="sxs-lookup"><span data-stu-id="f5b00-107">Method</span></span>       | <span data-ttu-id="f5b00-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f5b00-108">Return Type</span></span> | <span data-ttu-id="f5b00-109">说明</span><span class="sxs-lookup"><span data-stu-id="f5b00-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f5b00-110">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f5b00-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="f5b00-111">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f5b00-111">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="f5b00-112">通过发布 **emailFileAssessmentRequest** 对象创建新的电子邮件文件评估请求。</span><span class="sxs-lookup"><span data-stu-id="f5b00-112">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="f5b00-113">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f5b00-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="f5b00-114">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="f5b00-114">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="f5b00-115">读取 **emailFileAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f5b00-115">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f5b00-116">属性</span><span class="sxs-lookup"><span data-stu-id="f5b00-116">Properties</span></span>

| <span data-ttu-id="f5b00-117">属性</span><span class="sxs-lookup"><span data-stu-id="f5b00-117">Property</span></span>     | <span data-ttu-id="f5b00-118">类型</span><span class="sxs-lookup"><span data-stu-id="f5b00-118">Type</span></span>        | <span data-ttu-id="f5b00-119">说明</span><span class="sxs-lookup"><span data-stu-id="f5b00-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5b00-120">contentData</span><span class="sxs-lookup"><span data-stu-id="f5b00-120">contentData</span></span>|<span data-ttu-id="f5b00-121">String</span><span class="sxs-lookup"><span data-stu-id="f5b00-121">String</span></span>|<span data-ttu-id="f5b00-122">Base64 编码的 .eml 电子邮件文件内容。</span><span class="sxs-lookup"><span data-stu-id="f5b00-122">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="f5b00-123">由于未存储文件内容，因此无法将其取回。</span><span class="sxs-lookup"><span data-stu-id="f5b00-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="f5b00-124">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="f5b00-124">destinationRoutingReason</span></span>|[<span data-ttu-id="f5b00-125">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="f5b00-125">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="f5b00-126">邮件路由到其目标的原因。</span><span class="sxs-lookup"><span data-stu-id="f5b00-126">The reason for mail routed to its destination.</span></span> <span data-ttu-id="f5b00-127">可能的值为：、、、、、、、、、、、、、、 `none` `mailFlowRule` `safeSender` `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` 。</span><span class="sxs-lookup"><span data-stu-id="f5b00-127">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="f5b00-128">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="f5b00-128">recipientEmail</span></span>|<span data-ttu-id="f5b00-129">String</span><span class="sxs-lookup"><span data-stu-id="f5b00-129">String</span></span>|<span data-ttu-id="f5b00-130">其策略用于评估邮件的邮件收件人。</span><span class="sxs-lookup"><span data-stu-id="f5b00-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="f5b00-131">“类别”</span><span class="sxs-lookup"><span data-stu-id="f5b00-131">category</span></span>|[<span data-ttu-id="f5b00-132">threatCategory</span><span class="sxs-lookup"><span data-stu-id="f5b00-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="f5b00-133">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="f5b00-133">The threat category.</span></span> <span data-ttu-id="f5b00-134">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="f5b00-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="f5b00-135">contentType</span><span class="sxs-lookup"><span data-stu-id="f5b00-135">contentType</span></span>|[<span data-ttu-id="f5b00-136">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="f5b00-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="f5b00-137">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="f5b00-137">The content type of threat assessment.</span></span> <span data-ttu-id="f5b00-138">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="f5b00-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="f5b00-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="f5b00-139">createdBy</span></span>|[<span data-ttu-id="f5b00-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="f5b00-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="f5b00-141">威胁评估请求创建程序。</span><span class="sxs-lookup"><span data-stu-id="f5b00-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="f5b00-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5b00-142">createdDateTime</span></span>|<span data-ttu-id="f5b00-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5b00-143">DateTimeOffset</span></span>|<span data-ttu-id="f5b00-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f5b00-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f5b00-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="f5b00-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="f5b00-146">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="f5b00-146">expectedAssessment</span></span>|[<span data-ttu-id="f5b00-147">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="f5b00-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="f5b00-148">来自提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="f5b00-148">The expected assessment from submitter.</span></span> <span data-ttu-id="f5b00-149">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="f5b00-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="f5b00-150">id</span><span class="sxs-lookup"><span data-stu-id="f5b00-150">id</span></span>|<span data-ttu-id="f5b00-151">String</span><span class="sxs-lookup"><span data-stu-id="f5b00-151">String</span></span>|<span data-ttu-id="f5b00-152">威胁评估请求 ID 是 GUID)  (全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f5b00-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="f5b00-153">requestSource</span><span class="sxs-lookup"><span data-stu-id="f5b00-153">requestSource</span></span>|[<span data-ttu-id="f5b00-154">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="f5b00-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="f5b00-155">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="f5b00-155">The source of threat assessment request.</span></span> <span data-ttu-id="f5b00-156">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="f5b00-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="f5b00-157">status</span><span class="sxs-lookup"><span data-stu-id="f5b00-157">status</span></span>|[<span data-ttu-id="f5b00-158">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="f5b00-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="f5b00-159">评估过程状态。</span><span class="sxs-lookup"><span data-stu-id="f5b00-159">The assessment process status.</span></span> <span data-ttu-id="f5b00-160">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="f5b00-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5b00-161">关系</span><span class="sxs-lookup"><span data-stu-id="f5b00-161">Relationships</span></span>

| <span data-ttu-id="f5b00-162">关系</span><span class="sxs-lookup"><span data-stu-id="f5b00-162">Relationship</span></span> | <span data-ttu-id="f5b00-163">类型</span><span class="sxs-lookup"><span data-stu-id="f5b00-163">Type</span></span>        | <span data-ttu-id="f5b00-164">说明</span><span class="sxs-lookup"><span data-stu-id="f5b00-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5b00-165">results</span><span class="sxs-lookup"><span data-stu-id="f5b00-165">results</span></span>|<span data-ttu-id="f5b00-166">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f5b00-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="f5b00-167">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="f5b00-167">A collection of threat assessment results.</span></span> <span data-ttu-id="f5b00-168">只读。</span><span class="sxs-lookup"><span data-stu-id="f5b00-168">Read-only.</span></span> <span data-ttu-id="f5b00-169">默认情况下，a 不 `GET /threatAssessmentRequests/{id}` 会返回此属性，除非您应用于该属性 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="f5b00-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5b00-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5b00-170">JSON representation</span></span>

<span data-ttu-id="f5b00-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5b00-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "destinationRoutingReason": "String",
  "recipientEmail": "String",
  "category": "String",
  "contentType": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "expectedAssessment": "String",
  "id": "String (identifier)",
  "requestSource": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailFileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

