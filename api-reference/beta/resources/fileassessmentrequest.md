---
title: fileAssessmentRequest 资源类型
description: 用于创建和检索文件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 51211fd4ab732525423617bb3bdcb6c00091ac86
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945653"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="1ffaf-103">fileAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ffaf-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="1ffaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ffaf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ffaf-105">用于创建和检索派生自 [threatAssessmentRequest](threatAssessmentRequest.md)的文件威胁评估。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-105">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="1ffaf-106">该文件可以是在电子邮件附件中收到的文本文件、Word 文档或二进制文件。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-106">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="1ffaf-107">Methods</span><span class="sxs-lookup"><span data-stu-id="1ffaf-107">Methods</span></span>

| <span data-ttu-id="1ffaf-108">方法</span><span class="sxs-lookup"><span data-stu-id="1ffaf-108">Method</span></span>       | <span data-ttu-id="1ffaf-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1ffaf-109">Return Type</span></span> | <span data-ttu-id="1ffaf-110">说明</span><span class="sxs-lookup"><span data-stu-id="1ffaf-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1ffaf-111">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="1ffaf-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="1ffaf-112">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="1ffaf-112">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="1ffaf-113">通过发布 **fileAssessmentRequest** 对象创建新的文件评估请求。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-113">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="1ffaf-114">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="1ffaf-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="1ffaf-115">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="1ffaf-115">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="1ffaf-116">读取 **fileAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-116">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1ffaf-117">属性</span><span class="sxs-lookup"><span data-stu-id="1ffaf-117">Properties</span></span>

| <span data-ttu-id="1ffaf-118">属性</span><span class="sxs-lookup"><span data-stu-id="1ffaf-118">Property</span></span>     | <span data-ttu-id="1ffaf-119">类型</span><span class="sxs-lookup"><span data-stu-id="1ffaf-119">Type</span></span>        | <span data-ttu-id="1ffaf-120">说明</span><span class="sxs-lookup"><span data-stu-id="1ffaf-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ffaf-121">contentData</span><span class="sxs-lookup"><span data-stu-id="1ffaf-121">contentData</span></span>|<span data-ttu-id="1ffaf-122">String</span><span class="sxs-lookup"><span data-stu-id="1ffaf-122">String</span></span>|<span data-ttu-id="1ffaf-123">Base64 编码文件内容。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-123">Base64 encoded file content.</span></span> <span data-ttu-id="1ffaf-124">文件内容无法取回，因为它未存储。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="1ffaf-125">fileName</span><span class="sxs-lookup"><span data-stu-id="1ffaf-125">fileName</span></span>|<span data-ttu-id="1ffaf-126">String</span><span class="sxs-lookup"><span data-stu-id="1ffaf-126">String</span></span>|<span data-ttu-id="1ffaf-127">文件名。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-127">The file name.</span></span>|
|<span data-ttu-id="1ffaf-128">“类别”</span><span class="sxs-lookup"><span data-stu-id="1ffaf-128">category</span></span>|[<span data-ttu-id="1ffaf-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="1ffaf-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="1ffaf-130">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-130">The threat category.</span></span> <span data-ttu-id="1ffaf-131">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="1ffaf-132">contentType</span><span class="sxs-lookup"><span data-stu-id="1ffaf-132">contentType</span></span>|[<span data-ttu-id="1ffaf-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="1ffaf-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="1ffaf-134">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-134">The content type of threat assessment.</span></span> <span data-ttu-id="1ffaf-135">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="1ffaf-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="1ffaf-136">createdBy</span></span>|[<span data-ttu-id="1ffaf-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="1ffaf-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="1ffaf-138">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="1ffaf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ffaf-139">createdDateTime</span></span>|<span data-ttu-id="1ffaf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ffaf-140">DateTimeOffset</span></span>|<span data-ttu-id="1ffaf-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ffaf-142">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="1ffaf-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="1ffaf-143">expectedAssessment</span></span>|[<span data-ttu-id="1ffaf-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="1ffaf-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="1ffaf-145">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-145">The expected assessment from submitter.</span></span> <span data-ttu-id="1ffaf-146">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="1ffaf-147">id</span><span class="sxs-lookup"><span data-stu-id="1ffaf-147">id</span></span>|<span data-ttu-id="1ffaf-148">String</span><span class="sxs-lookup"><span data-stu-id="1ffaf-148">String</span></span>|<span data-ttu-id="1ffaf-149">威胁评估请求 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="1ffaf-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="1ffaf-150">requestSource</span></span>|[<span data-ttu-id="1ffaf-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="1ffaf-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="1ffaf-152">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-152">The source of threat assessment request.</span></span> <span data-ttu-id="1ffaf-153">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="1ffaf-154">状态</span><span class="sxs-lookup"><span data-stu-id="1ffaf-154">status</span></span>|[<span data-ttu-id="1ffaf-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="1ffaf-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="1ffaf-156">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-156">The assessment process status.</span></span> <span data-ttu-id="1ffaf-157">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ffaf-158">关系</span><span class="sxs-lookup"><span data-stu-id="1ffaf-158">Relationships</span></span>

| <span data-ttu-id="1ffaf-159">关系</span><span class="sxs-lookup"><span data-stu-id="1ffaf-159">Relationship</span></span> | <span data-ttu-id="1ffaf-160">类型</span><span class="sxs-lookup"><span data-stu-id="1ffaf-160">Type</span></span>        | <span data-ttu-id="1ffaf-161">说明</span><span class="sxs-lookup"><span data-stu-id="1ffaf-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1ffaf-162">results</span><span class="sxs-lookup"><span data-stu-id="1ffaf-162">results</span></span>|<span data-ttu-id="1ffaf-163">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ffaf-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="1ffaf-164">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-164">A collection of threat assessment results.</span></span> <span data-ttu-id="1ffaf-165">只读。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-165">Read-only.</span></span> <span data-ttu-id="1ffaf-166">默认情况下， `GET /threatAssessmentRequests/{id}` 除非对该属性应用 ，否则 不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1ffaf-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ffaf-167">JSON representation</span></span>

<span data-ttu-id="1ffaf-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ffaf-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "contentData": "String",
  "fileName": "String",
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
  "description": "fileAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


