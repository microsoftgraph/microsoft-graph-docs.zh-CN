---
title: fileAssessmentRequest 资源类型
description: 用于创建和检索文件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 22142bacd6ebff4cad2d3856de168f89b8b2b3d4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154738"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="dedc6-103">fileAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="dedc6-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="dedc6-104">用于创建和检索派生自 [threatAssessmentRequest](threatAssessmentRequest.md)的文件威胁评估。</span><span class="sxs-lookup"><span data-stu-id="dedc6-104">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="dedc6-105">该文件可以是文本文件、Word 文档或电子邮件附件中收到的二进制文件。</span><span class="sxs-lookup"><span data-stu-id="dedc6-105">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="dedc6-106">方法</span><span class="sxs-lookup"><span data-stu-id="dedc6-106">Methods</span></span>

| <span data-ttu-id="dedc6-107">方法</span><span class="sxs-lookup"><span data-stu-id="dedc6-107">Method</span></span>       | <span data-ttu-id="dedc6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dedc6-108">Return Type</span></span> | <span data-ttu-id="dedc6-109">说明</span><span class="sxs-lookup"><span data-stu-id="dedc6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dedc6-110">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dedc6-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="dedc6-111">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dedc6-111">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="dedc6-112">通过发布 **fileAssessmentRequest** 对象创建新的文件评估请求。</span><span class="sxs-lookup"><span data-stu-id="dedc6-112">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="dedc6-113">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dedc6-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="dedc6-114">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dedc6-114">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="dedc6-115">读取 **fileAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dedc6-115">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dedc6-116">属性</span><span class="sxs-lookup"><span data-stu-id="dedc6-116">Properties</span></span>

| <span data-ttu-id="dedc6-117">属性</span><span class="sxs-lookup"><span data-stu-id="dedc6-117">Property</span></span>     | <span data-ttu-id="dedc6-118">类型</span><span class="sxs-lookup"><span data-stu-id="dedc6-118">Type</span></span>        | <span data-ttu-id="dedc6-119">说明</span><span class="sxs-lookup"><span data-stu-id="dedc6-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dedc6-120">contentData</span><span class="sxs-lookup"><span data-stu-id="dedc6-120">contentData</span></span>|<span data-ttu-id="dedc6-121">String</span><span class="sxs-lookup"><span data-stu-id="dedc6-121">String</span></span>|<span data-ttu-id="dedc6-122">Base64 编码的文件内容。</span><span class="sxs-lookup"><span data-stu-id="dedc6-122">Base64 encoded file content.</span></span> <span data-ttu-id="dedc6-123">文件内容无法取回，因为它未存储。</span><span class="sxs-lookup"><span data-stu-id="dedc6-123">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="dedc6-124">fileName</span><span class="sxs-lookup"><span data-stu-id="dedc6-124">fileName</span></span>|<span data-ttu-id="dedc6-125">String</span><span class="sxs-lookup"><span data-stu-id="dedc6-125">String</span></span>|<span data-ttu-id="dedc6-126">文件名。</span><span class="sxs-lookup"><span data-stu-id="dedc6-126">The file name.</span></span>|
|<span data-ttu-id="dedc6-127">“类别”</span><span class="sxs-lookup"><span data-stu-id="dedc6-127">category</span></span>|[<span data-ttu-id="dedc6-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="dedc6-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="dedc6-129">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="dedc6-129">The threat category.</span></span> <span data-ttu-id="dedc6-130">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="dedc6-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="dedc6-131">contentType</span><span class="sxs-lookup"><span data-stu-id="dedc6-131">contentType</span></span>|[<span data-ttu-id="dedc6-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="dedc6-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="dedc6-133">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="dedc6-133">The content type of threat assessment.</span></span> <span data-ttu-id="dedc6-134">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="dedc6-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="dedc6-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="dedc6-135">createdBy</span></span>|[<span data-ttu-id="dedc6-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="dedc6-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="dedc6-137">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="dedc6-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="dedc6-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dedc6-138">createdDateTime</span></span>|<span data-ttu-id="dedc6-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dedc6-139">DateTimeOffset</span></span>|<span data-ttu-id="dedc6-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="dedc6-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dedc6-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="dedc6-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="dedc6-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="dedc6-142">expectedAssessment</span></span>|[<span data-ttu-id="dedc6-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="dedc6-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="dedc6-144">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="dedc6-144">The expected assessment from submitter.</span></span> <span data-ttu-id="dedc6-145">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="dedc6-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="dedc6-146">id</span><span class="sxs-lookup"><span data-stu-id="dedc6-146">id</span></span>|<span data-ttu-id="dedc6-147">String</span><span class="sxs-lookup"><span data-stu-id="dedc6-147">String</span></span>|<span data-ttu-id="dedc6-148">威胁评估请求 ID 是 GUID (全局) 。</span><span class="sxs-lookup"><span data-stu-id="dedc6-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="dedc6-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="dedc6-149">requestSource</span></span>|[<span data-ttu-id="dedc6-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="dedc6-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="dedc6-151">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="dedc6-151">The source of threat assessment request.</span></span> <span data-ttu-id="dedc6-152">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="dedc6-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="dedc6-153">status</span><span class="sxs-lookup"><span data-stu-id="dedc6-153">status</span></span>|[<span data-ttu-id="dedc6-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="dedc6-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="dedc6-155">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="dedc6-155">The assessment process status.</span></span> <span data-ttu-id="dedc6-156">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="dedc6-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dedc6-157">关系</span><span class="sxs-lookup"><span data-stu-id="dedc6-157">Relationships</span></span>

| <span data-ttu-id="dedc6-158">关系</span><span class="sxs-lookup"><span data-stu-id="dedc6-158">Relationship</span></span> | <span data-ttu-id="dedc6-159">类型</span><span class="sxs-lookup"><span data-stu-id="dedc6-159">Type</span></span>        | <span data-ttu-id="dedc6-160">说明</span><span class="sxs-lookup"><span data-stu-id="dedc6-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dedc6-161">results</span><span class="sxs-lookup"><span data-stu-id="dedc6-161">results</span></span>|<span data-ttu-id="dedc6-162">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dedc6-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="dedc6-163">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="dedc6-163">A collection of threat assessment results.</span></span> <span data-ttu-id="dedc6-164">只读。</span><span class="sxs-lookup"><span data-stu-id="dedc6-164">Read-only.</span></span> <span data-ttu-id="dedc6-165">默认情况下，除非对该属性应用， `GET /threatAssessmentRequests/{id}` 否则不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="dedc6-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dedc6-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dedc6-166">JSON representation</span></span>

<span data-ttu-id="dedc6-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dedc6-167">The following is a JSON representation of the resource.</span></span>

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

