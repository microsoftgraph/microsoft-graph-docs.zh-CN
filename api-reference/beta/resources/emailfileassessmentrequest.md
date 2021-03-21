---
title: emailFileAssessmentRequest 资源类型
description: 用于创建和检索电子邮件文件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 77c95b18056487f94a5cb75b946d0ee8f75e46f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960444"
---
# <a name="emailfileassessmentrequest-resource-type"></a><span data-ttu-id="63c3c-103">emailFileAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="63c3c-103">emailFileAssessmentRequest resource type</span></span>

<span data-ttu-id="63c3c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63c3c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63c3c-105">用于创建和检索电子邮件文件威胁评估，派生自 [threatAssessmentRequest](threatAssessmentRequest.md)。</span><span class="sxs-lookup"><span data-stu-id="63c3c-105">Used to create and retrieve an email file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="63c3c-106">电子邮件文件可以是 .eml 文件类型。</span><span class="sxs-lookup"><span data-stu-id="63c3c-106">The email file can be an .eml file type.</span></span>

## <a name="methods"></a><span data-ttu-id="63c3c-107">Methods</span><span class="sxs-lookup"><span data-stu-id="63c3c-107">Methods</span></span>

| <span data-ttu-id="63c3c-108">方法</span><span class="sxs-lookup"><span data-stu-id="63c3c-108">Method</span></span>       | <span data-ttu-id="63c3c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="63c3c-109">Return Type</span></span> | <span data-ttu-id="63c3c-110">说明</span><span class="sxs-lookup"><span data-stu-id="63c3c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="63c3c-111">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="63c3c-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="63c3c-112">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="63c3c-112">emailFileAssessmentRequest</span></span>](emailFileAssessmentRequest.md) | <span data-ttu-id="63c3c-113">通过发布 **emailFileAssessmentRequest** 对象创建新的电子邮件文件评估请求。</span><span class="sxs-lookup"><span data-stu-id="63c3c-113">Create a new email file assessment request by posting an **emailFileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="63c3c-114">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="63c3c-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="63c3c-115">emailFileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="63c3c-115">emailFileAssessmentRequest</span></span>](emailfileassessmentrequest.md) | <span data-ttu-id="63c3c-116">读取 **emailFileAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="63c3c-116">Read the properties and relationships of an **emailFileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="63c3c-117">属性</span><span class="sxs-lookup"><span data-stu-id="63c3c-117">Properties</span></span>

| <span data-ttu-id="63c3c-118">属性</span><span class="sxs-lookup"><span data-stu-id="63c3c-118">Property</span></span>     | <span data-ttu-id="63c3c-119">类型</span><span class="sxs-lookup"><span data-stu-id="63c3c-119">Type</span></span>        | <span data-ttu-id="63c3c-120">说明</span><span class="sxs-lookup"><span data-stu-id="63c3c-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63c3c-121">contentData</span><span class="sxs-lookup"><span data-stu-id="63c3c-121">contentData</span></span>|<span data-ttu-id="63c3c-122">String</span><span class="sxs-lookup"><span data-stu-id="63c3c-122">String</span></span>|<span data-ttu-id="63c3c-123">Base64 编码的 .eml 电子邮件文件内容。</span><span class="sxs-lookup"><span data-stu-id="63c3c-123">Base64 encoded .eml email file content.</span></span> <span data-ttu-id="63c3c-124">文件内容无法取回，因为它未存储。</span><span class="sxs-lookup"><span data-stu-id="63c3c-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="63c3c-125">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="63c3c-125">destinationRoutingReason</span></span>|[<span data-ttu-id="63c3c-126">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="63c3c-126">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="63c3c-127">邮件路由到目标的原因。</span><span class="sxs-lookup"><span data-stu-id="63c3c-127">The reason for mail routed to its destination.</span></span> <span data-ttu-id="63c3c-128">可能的值是 `none` `mailFlowRule` `safeSender` ：、、、、、、、、、、 `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` 。</span><span class="sxs-lookup"><span data-stu-id="63c3c-128">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="63c3c-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="63c3c-129">recipientEmail</span></span>|<span data-ttu-id="63c3c-130">String</span><span class="sxs-lookup"><span data-stu-id="63c3c-130">String</span></span>|<span data-ttu-id="63c3c-131">其策略用于评估邮件的邮件收件人。</span><span class="sxs-lookup"><span data-stu-id="63c3c-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="63c3c-132">“类别”</span><span class="sxs-lookup"><span data-stu-id="63c3c-132">category</span></span>|[<span data-ttu-id="63c3c-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="63c3c-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="63c3c-134">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="63c3c-134">The threat category.</span></span> <span data-ttu-id="63c3c-135">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="63c3c-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="63c3c-136">contentType</span><span class="sxs-lookup"><span data-stu-id="63c3c-136">contentType</span></span>|[<span data-ttu-id="63c3c-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="63c3c-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="63c3c-138">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="63c3c-138">The content type of threat assessment.</span></span> <span data-ttu-id="63c3c-139">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="63c3c-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="63c3c-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="63c3c-140">createdBy</span></span>|[<span data-ttu-id="63c3c-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="63c3c-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="63c3c-142">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="63c3c-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="63c3c-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="63c3c-143">createdDateTime</span></span>|<span data-ttu-id="63c3c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="63c3c-144">DateTimeOffset</span></span>|<span data-ttu-id="63c3c-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="63c3c-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="63c3c-146">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="63c3c-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="63c3c-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="63c3c-147">expectedAssessment</span></span>|[<span data-ttu-id="63c3c-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="63c3c-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="63c3c-149">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="63c3c-149">The expected assessment from submitter.</span></span> <span data-ttu-id="63c3c-150">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="63c3c-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="63c3c-151">id</span><span class="sxs-lookup"><span data-stu-id="63c3c-151">id</span></span>|<span data-ttu-id="63c3c-152">String</span><span class="sxs-lookup"><span data-stu-id="63c3c-152">String</span></span>|<span data-ttu-id="63c3c-153">威胁评估请求 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="63c3c-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="63c3c-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="63c3c-154">requestSource</span></span>|[<span data-ttu-id="63c3c-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="63c3c-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="63c3c-156">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="63c3c-156">The source of threat assessment request.</span></span> <span data-ttu-id="63c3c-157">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="63c3c-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="63c3c-158">状态</span><span class="sxs-lookup"><span data-stu-id="63c3c-158">status</span></span>|[<span data-ttu-id="63c3c-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="63c3c-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="63c3c-160">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="63c3c-160">The assessment process status.</span></span> <span data-ttu-id="63c3c-161">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="63c3c-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63c3c-162">关系</span><span class="sxs-lookup"><span data-stu-id="63c3c-162">Relationships</span></span>

| <span data-ttu-id="63c3c-163">关系</span><span class="sxs-lookup"><span data-stu-id="63c3c-163">Relationship</span></span> | <span data-ttu-id="63c3c-164">类型</span><span class="sxs-lookup"><span data-stu-id="63c3c-164">Type</span></span>        | <span data-ttu-id="63c3c-165">说明</span><span class="sxs-lookup"><span data-stu-id="63c3c-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63c3c-166">results</span><span class="sxs-lookup"><span data-stu-id="63c3c-166">results</span></span>|<span data-ttu-id="63c3c-167">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="63c3c-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="63c3c-168">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="63c3c-168">A collection of threat assessment results.</span></span> <span data-ttu-id="63c3c-169">只读。</span><span class="sxs-lookup"><span data-stu-id="63c3c-169">Read-only.</span></span> <span data-ttu-id="63c3c-170">默认情况下， `GET /threatAssessmentRequests/{id}` 除非对该属性应用 ，否则 不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="63c3c-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63c3c-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63c3c-171">JSON representation</span></span>

<span data-ttu-id="63c3c-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63c3c-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
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


