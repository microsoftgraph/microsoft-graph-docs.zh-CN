---
title: mailAssessmentRequest 资源类型
description: 用于创建和检索邮件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3e45cddeb7d0a9814a1feb6732828ef7363602bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961270"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="2289f-103">mailAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2289f-103">mailAssessmentRequest resource type</span></span>

<span data-ttu-id="2289f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2289f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2289f-105">用于创建和检索邮件威胁评估，派生自 [threatAssessmentRequest](threatAssessmentRequest.md)。</span><span class="sxs-lookup"><span data-stu-id="2289f-105">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="2289f-106">创建邮件威胁评估请求时，邮件应由 中指定的用户接收 `recipientEmail` 。</span><span class="sxs-lookup"><span data-stu-id="2289f-106">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="2289f-107">[Mail.Read](/graph/permissions-reference#mail-permissions) (Mail.Read 或 Mail.Read.Shared) 的委派邮件权限将重新进行重新quried，以访问用户接收或其他人共享的邮件。</span><span class="sxs-lookup"><span data-stu-id="2289f-107">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="2289f-108">Methods</span><span class="sxs-lookup"><span data-stu-id="2289f-108">Methods</span></span>

| <span data-ttu-id="2289f-109">方法</span><span class="sxs-lookup"><span data-stu-id="2289f-109">Method</span></span>       | <span data-ttu-id="2289f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2289f-110">Return Type</span></span> | <span data-ttu-id="2289f-111">说明</span><span class="sxs-lookup"><span data-stu-id="2289f-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2289f-112">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2289f-112">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="2289f-113">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2289f-113">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="2289f-114">通过发布 **mailAssessmentRequest** 对象创建新的邮件评估请求。</span><span class="sxs-lookup"><span data-stu-id="2289f-114">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="2289f-115">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2289f-115">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="2289f-116">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2289f-116">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="2289f-117">读取 **mailAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2289f-117">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="2289f-118">属性</span><span class="sxs-lookup"><span data-stu-id="2289f-118">Properties</span></span>

| <span data-ttu-id="2289f-119">属性</span><span class="sxs-lookup"><span data-stu-id="2289f-119">Property</span></span>     | <span data-ttu-id="2289f-120">类型</span><span class="sxs-lookup"><span data-stu-id="2289f-120">Type</span></span>        | <span data-ttu-id="2289f-121">说明</span><span class="sxs-lookup"><span data-stu-id="2289f-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2289f-122">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="2289f-122">destinationRoutingReason</span></span>|[<span data-ttu-id="2289f-123">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="2289f-123">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="2289f-124">邮件路由到目标的原因。</span><span class="sxs-lookup"><span data-stu-id="2289f-124">The reason for mail routed to its destination.</span></span> <span data-ttu-id="2289f-125">可能的值是 `none` `mailFlowRule` `safeSender` ：、、、、、、、、、、 `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `autoPurgeToInbox` `autoPurgeToJunk` `autoPurgeToDeleted` `outbound` `notJunk` `junk` 。</span><span class="sxs-lookup"><span data-stu-id="2289f-125">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="2289f-126">messageUri</span><span class="sxs-lookup"><span data-stu-id="2289f-126">messageUri</span></span>|<span data-ttu-id="2289f-127">String</span><span class="sxs-lookup"><span data-stu-id="2289f-127">String</span></span>|<span data-ttu-id="2289f-128">要评估的邮件的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="2289f-128">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="2289f-129">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="2289f-129">recipientEmail</span></span>|<span data-ttu-id="2289f-130">String</span><span class="sxs-lookup"><span data-stu-id="2289f-130">String</span></span>|<span data-ttu-id="2289f-131">其策略用于评估邮件的邮件收件人。</span><span class="sxs-lookup"><span data-stu-id="2289f-131">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="2289f-132">“类别”</span><span class="sxs-lookup"><span data-stu-id="2289f-132">category</span></span>|[<span data-ttu-id="2289f-133">threatCategory</span><span class="sxs-lookup"><span data-stu-id="2289f-133">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="2289f-134">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="2289f-134">The threat category.</span></span> <span data-ttu-id="2289f-135">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="2289f-135">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="2289f-136">contentType</span><span class="sxs-lookup"><span data-stu-id="2289f-136">contentType</span></span>|[<span data-ttu-id="2289f-137">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="2289f-137">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="2289f-138">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="2289f-138">The content type of threat assessment.</span></span> <span data-ttu-id="2289f-139">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="2289f-139">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="2289f-140">createdBy</span><span class="sxs-lookup"><span data-stu-id="2289f-140">createdBy</span></span>|[<span data-ttu-id="2289f-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="2289f-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="2289f-142">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="2289f-142">The threat assessment request creator.</span></span>|
|<span data-ttu-id="2289f-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2289f-143">createdDateTime</span></span>|<span data-ttu-id="2289f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2289f-144">DateTimeOffset</span></span>|<span data-ttu-id="2289f-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2289f-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2289f-146">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="2289f-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="2289f-147">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2289f-147">expectedAssessment</span></span>|[<span data-ttu-id="2289f-148">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2289f-148">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="2289f-149">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="2289f-149">The expected assessment from submitter.</span></span> <span data-ttu-id="2289f-150">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="2289f-150">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="2289f-151">id</span><span class="sxs-lookup"><span data-stu-id="2289f-151">id</span></span>|<span data-ttu-id="2289f-152">String</span><span class="sxs-lookup"><span data-stu-id="2289f-152">String</span></span>|<span data-ttu-id="2289f-153">威胁评估请求 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="2289f-153">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="2289f-154">requestSource</span><span class="sxs-lookup"><span data-stu-id="2289f-154">requestSource</span></span>|[<span data-ttu-id="2289f-155">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="2289f-155">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="2289f-156">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="2289f-156">The source of threat assessment request.</span></span> <span data-ttu-id="2289f-157">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="2289f-157">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="2289f-158">状态</span><span class="sxs-lookup"><span data-stu-id="2289f-158">status</span></span>|[<span data-ttu-id="2289f-159">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="2289f-159">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="2289f-160">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="2289f-160">The assessment process status.</span></span> <span data-ttu-id="2289f-161">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="2289f-161">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2289f-162">关系</span><span class="sxs-lookup"><span data-stu-id="2289f-162">Relationships</span></span>

| <span data-ttu-id="2289f-163">关系</span><span class="sxs-lookup"><span data-stu-id="2289f-163">Relationship</span></span> | <span data-ttu-id="2289f-164">类型</span><span class="sxs-lookup"><span data-stu-id="2289f-164">Type</span></span>        | <span data-ttu-id="2289f-165">说明</span><span class="sxs-lookup"><span data-stu-id="2289f-165">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2289f-166">results</span><span class="sxs-lookup"><span data-stu-id="2289f-166">results</span></span>|<span data-ttu-id="2289f-167">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2289f-167">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="2289f-168">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="2289f-168">A collection of threat assessment results.</span></span> <span data-ttu-id="2289f-169">只读。</span><span class="sxs-lookup"><span data-stu-id="2289f-169">Read-only.</span></span> <span data-ttu-id="2289f-170">默认情况下， `GET /threatAssessmentRequests/{id}` 除非对该属性应用 ，否则 不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="2289f-170">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2289f-171">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2289f-171">JSON representation</span></span>

<span data-ttu-id="2289f-172">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2289f-172">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "destinationRoutingReason": "String",
  "messageUri": "String",
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
  "description": "mailAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


