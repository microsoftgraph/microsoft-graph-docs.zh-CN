---
title: mailAssessmentRequest 资源类型
description: 用于创建和检索邮件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c910c0c9f2ab33a70684d8a66e890a2587eccc0
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867165"
---
# <a name="mailassessmentrequest-resource-type"></a><span data-ttu-id="2ad0e-103">mailAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ad0e-103">mailAssessmentRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ad0e-104">用于创建和检索从[threatAssessmentRequest](threatAssessmentRequest.md)派生的邮件威胁评估。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-104">Used to create and retrieve a mail threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="2ad0e-105">当您创建邮件威胁评估请求时，邮件应由中`recipientEmail`指定的用户接收。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-105">When you create a mail threat assessment request, the mail should be received by the user specified in `recipientEmail`.</span></span> <span data-ttu-id="2ad0e-106">委派的[邮件权限](/graph/permissions-reference#mail-permissions)（Mail. Read 或 mail）是 requried，用于访问用户接收的邮件或由其他人共享的邮件。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-106">Delegated [Mail permissions](/graph/permissions-reference#mail-permissions) (Mail.Read or Mail.Read.Shared) are requried to access the mail received by the user or shared by someone else.</span></span>

## <a name="methods"></a><span data-ttu-id="2ad0e-107">方法</span><span class="sxs-lookup"><span data-stu-id="2ad0e-107">Methods</span></span>

| <span data-ttu-id="2ad0e-108">方法</span><span class="sxs-lookup"><span data-stu-id="2ad0e-108">Method</span></span>       | <span data-ttu-id="2ad0e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ad0e-109">Return Type</span></span> | <span data-ttu-id="2ad0e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ad0e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2ad0e-111">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2ad0e-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="2ad0e-112">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2ad0e-112">mailAssessmentRequest</span></span>](mailAssessmentRequest.md) | <span data-ttu-id="2ad0e-113">通过发布**mailAssessmentRequest**对象创建新的邮件评估请求。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-113">Create a new mail assessment request by posting a **mailAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="2ad0e-114">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2ad0e-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="2ad0e-115">mailAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="2ad0e-115">mailAssessmentRequest</span></span>](mailassessmentrequest.md) | <span data-ttu-id="2ad0e-116">读取**mailAssessmentRequest**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-116">Read the properties and relationships of a **mailAssessmentRequest** object.</span></span> |


## <a name="properties"></a><span data-ttu-id="2ad0e-117">属性</span><span class="sxs-lookup"><span data-stu-id="2ad0e-117">Properties</span></span>

| <span data-ttu-id="2ad0e-118">属性</span><span class="sxs-lookup"><span data-stu-id="2ad0e-118">Property</span></span>     | <span data-ttu-id="2ad0e-119">类型</span><span class="sxs-lookup"><span data-stu-id="2ad0e-119">Type</span></span>        | <span data-ttu-id="2ad0e-120">说明</span><span class="sxs-lookup"><span data-stu-id="2ad0e-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ad0e-121">destinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="2ad0e-121">destinationRoutingReason</span></span>|[<span data-ttu-id="2ad0e-122">mailDestinationRoutingReason</span><span class="sxs-lookup"><span data-stu-id="2ad0e-122">mailDestinationRoutingReason</span></span>](enums.md#maildestinationroutingreason-values)|<span data-ttu-id="2ad0e-123">邮件路由到其目标的原因。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-123">The reason for mail routed to its destination.</span></span> <span data-ttu-id="2ad0e-124">可能的值为`none`： `mailFlowRule`、 `safeSender`、 `blockedSender` `advancedSpamFiltering` `domainAllowList` `domainBlockList` `notInAddressBook` `firstTimeSender` `junk`、、 `autoPurgeToJunk`、、、、、、、、、、。 `autoPurgeToInbox` `autoPurgeToDeleted` `outbound` `notJunk`</span><span class="sxs-lookup"><span data-stu-id="2ad0e-124">Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`.</span></span>|
|<span data-ttu-id="2ad0e-125">messageUri</span><span class="sxs-lookup"><span data-stu-id="2ad0e-125">messageUri</span></span>|<span data-ttu-id="2ad0e-126">String</span><span class="sxs-lookup"><span data-stu-id="2ad0e-126">String</span></span>|<span data-ttu-id="2ad0e-127">要进行评估的邮件邮件的资源 URI。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-127">The resource URI of the mail message for assessment.</span></span>|
|<span data-ttu-id="2ad0e-128">recipientEmail</span><span class="sxs-lookup"><span data-stu-id="2ad0e-128">recipientEmail</span></span>|<span data-ttu-id="2ad0e-129">String</span><span class="sxs-lookup"><span data-stu-id="2ad0e-129">String</span></span>|<span data-ttu-id="2ad0e-130">其策略用于评估邮件的邮件收件人。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-130">The mail recipient whose policies are used to assess the mail.</span></span>|
|<span data-ttu-id="2ad0e-131">“类别”</span><span class="sxs-lookup"><span data-stu-id="2ad0e-131">category</span></span>|[<span data-ttu-id="2ad0e-132">threatCategory</span><span class="sxs-lookup"><span data-stu-id="2ad0e-132">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="2ad0e-133">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-133">The threat category.</span></span> <span data-ttu-id="2ad0e-134">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-134">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="2ad0e-135">contentType</span><span class="sxs-lookup"><span data-stu-id="2ad0e-135">contentType</span></span>|[<span data-ttu-id="2ad0e-136">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="2ad0e-136">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="2ad0e-137">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-137">The content type of threat assessment.</span></span> <span data-ttu-id="2ad0e-138">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-138">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="2ad0e-139">createdBy</span><span class="sxs-lookup"><span data-stu-id="2ad0e-139">createdBy</span></span>|[<span data-ttu-id="2ad0e-140">identitySet</span><span class="sxs-lookup"><span data-stu-id="2ad0e-140">identitySet</span></span>](identityset.md)|<span data-ttu-id="2ad0e-141">威胁评估请求创建程序。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-141">The threat assessment request creator.</span></span>|
|<span data-ttu-id="2ad0e-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ad0e-142">createdDateTime</span></span>|<span data-ttu-id="2ad0e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ad0e-143">DateTimeOffset</span></span>|<span data-ttu-id="2ad0e-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2ad0e-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2ad0e-146">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2ad0e-146">expectedAssessment</span></span>|[<span data-ttu-id="2ad0e-147">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="2ad0e-147">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="2ad0e-148">来自提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-148">The expected assessment from submitter.</span></span> <span data-ttu-id="2ad0e-149">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-149">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="2ad0e-150">id</span><span class="sxs-lookup"><span data-stu-id="2ad0e-150">id</span></span>|<span data-ttu-id="2ad0e-151">String</span><span class="sxs-lookup"><span data-stu-id="2ad0e-151">String</span></span>|<span data-ttu-id="2ad0e-152">威胁评估请求 ID 是一个全局唯一标识符（GUID）。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-152">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="2ad0e-153">requestSource</span><span class="sxs-lookup"><span data-stu-id="2ad0e-153">requestSource</span></span>|[<span data-ttu-id="2ad0e-154">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="2ad0e-154">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="2ad0e-155">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-155">The source of threat assessment request.</span></span> <span data-ttu-id="2ad0e-156">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-156">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="2ad0e-157">状态</span><span class="sxs-lookup"><span data-stu-id="2ad0e-157">status</span></span>|[<span data-ttu-id="2ad0e-158">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="2ad0e-158">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="2ad0e-159">评估过程状态。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-159">The assessment process status.</span></span> <span data-ttu-id="2ad0e-160">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-160">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ad0e-161">关系</span><span class="sxs-lookup"><span data-stu-id="2ad0e-161">Relationships</span></span>

| <span data-ttu-id="2ad0e-162">关系</span><span class="sxs-lookup"><span data-stu-id="2ad0e-162">Relationship</span></span> | <span data-ttu-id="2ad0e-163">类型</span><span class="sxs-lookup"><span data-stu-id="2ad0e-163">Type</span></span>        | <span data-ttu-id="2ad0e-164">说明</span><span class="sxs-lookup"><span data-stu-id="2ad0e-164">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ad0e-165">results</span><span class="sxs-lookup"><span data-stu-id="2ad0e-165">results</span></span>|<span data-ttu-id="2ad0e-166">[threatAssessmentResult](threatassessmentresult.md)集合</span><span class="sxs-lookup"><span data-stu-id="2ad0e-166">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="2ad0e-167">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-167">A collection of threat assessment results.</span></span> <span data-ttu-id="2ad0e-168">只读。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-168">Read-only.</span></span> <span data-ttu-id="2ad0e-169">默认情况下， `GET /threatAssessmentRequests/{id}` a 不会返回此属性，除非`$expand`您应用于该属性。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-169">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ad0e-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ad0e-170">JSON representation</span></span>

<span data-ttu-id="2ad0e-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ad0e-171">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "",
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
