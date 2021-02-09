---
title: fileAssessmentRequest 资源类型
description: 用于创建和检索文件威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b61fadf340371b800e1dc093be012ba67f3eaf1b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50154943"
---
# <a name="fileassessmentrequest-resource-type"></a><span data-ttu-id="a2ecf-103">fileAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2ecf-103">fileAssessmentRequest resource type</span></span>

<span data-ttu-id="a2ecf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ecf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2ecf-105">用于创建和检索派生自 [threatAssessmentRequest](threatAssessmentRequest.md)的文件威胁评估。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-105">Used to create and retrieve a file threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

<span data-ttu-id="a2ecf-106">该文件可以是在电子邮件附件中收到的文本文件、Word 文档或二进制文件。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-106">The file can be a text file or Word document or binary file received in an email attachment.</span></span>

## <a name="methods"></a><span data-ttu-id="a2ecf-107">方法</span><span class="sxs-lookup"><span data-stu-id="a2ecf-107">Methods</span></span>

| <span data-ttu-id="a2ecf-108">方法</span><span class="sxs-lookup"><span data-stu-id="a2ecf-108">Method</span></span>       | <span data-ttu-id="a2ecf-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a2ecf-109">Return Type</span></span> | <span data-ttu-id="a2ecf-110">说明</span><span class="sxs-lookup"><span data-stu-id="a2ecf-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a2ecf-111">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a2ecf-111">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="a2ecf-112">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a2ecf-112">fileAssessmentRequest</span></span>](fileAssessmentRequest.md) | <span data-ttu-id="a2ecf-113">通过发布 **fileAssessmentRequest** 对象创建新的文件评估请求。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-113">Create a new file assessment request by posting a **fileAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="a2ecf-114">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a2ecf-114">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="a2ecf-115">fileAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="a2ecf-115">fileAssessmentRequest</span></span>](fileassessmentrequest.md) | <span data-ttu-id="a2ecf-116">读取 **fileAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-116">Read the properties and relationships of a **fileAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a2ecf-117">属性</span><span class="sxs-lookup"><span data-stu-id="a2ecf-117">Properties</span></span>

| <span data-ttu-id="a2ecf-118">属性</span><span class="sxs-lookup"><span data-stu-id="a2ecf-118">Property</span></span>     | <span data-ttu-id="a2ecf-119">类型</span><span class="sxs-lookup"><span data-stu-id="a2ecf-119">Type</span></span>        | <span data-ttu-id="a2ecf-120">说明</span><span class="sxs-lookup"><span data-stu-id="a2ecf-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2ecf-121">contentData</span><span class="sxs-lookup"><span data-stu-id="a2ecf-121">contentData</span></span>|<span data-ttu-id="a2ecf-122">String</span><span class="sxs-lookup"><span data-stu-id="a2ecf-122">String</span></span>|<span data-ttu-id="a2ecf-123">Base64 编码的文件内容。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-123">Base64 encoded file content.</span></span> <span data-ttu-id="a2ecf-124">文件内容无法取回，因为它未存储。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-124">The file content cannot fetch back because it isn't stored.</span></span>|
|<span data-ttu-id="a2ecf-125">fileName</span><span class="sxs-lookup"><span data-stu-id="a2ecf-125">fileName</span></span>|<span data-ttu-id="a2ecf-126">String</span><span class="sxs-lookup"><span data-stu-id="a2ecf-126">String</span></span>|<span data-ttu-id="a2ecf-127">文件名。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-127">The file name.</span></span>|
|<span data-ttu-id="a2ecf-128">“类别”</span><span class="sxs-lookup"><span data-stu-id="a2ecf-128">category</span></span>|[<span data-ttu-id="a2ecf-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="a2ecf-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="a2ecf-130">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-130">The threat category.</span></span> <span data-ttu-id="a2ecf-131">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="a2ecf-132">contentType</span><span class="sxs-lookup"><span data-stu-id="a2ecf-132">contentType</span></span>|[<span data-ttu-id="a2ecf-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="a2ecf-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="a2ecf-134">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-134">The content type of threat assessment.</span></span> <span data-ttu-id="a2ecf-135">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="a2ecf-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="a2ecf-136">createdBy</span></span>|[<span data-ttu-id="a2ecf-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="a2ecf-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="a2ecf-138">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="a2ecf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ecf-139">createdDateTime</span></span>|<span data-ttu-id="a2ecf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ecf-140">DateTimeOffset</span></span>|<span data-ttu-id="a2ecf-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a2ecf-142">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a2ecf-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="a2ecf-143">expectedAssessment</span></span>|[<span data-ttu-id="a2ecf-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="a2ecf-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="a2ecf-145">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-145">The expected assessment from submitter.</span></span> <span data-ttu-id="a2ecf-146">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="a2ecf-147">id</span><span class="sxs-lookup"><span data-stu-id="a2ecf-147">id</span></span>|<span data-ttu-id="a2ecf-148">String</span><span class="sxs-lookup"><span data-stu-id="a2ecf-148">String</span></span>|<span data-ttu-id="a2ecf-149">威胁评估请求 ID 是 GUID (全局) 。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="a2ecf-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="a2ecf-150">requestSource</span></span>|[<span data-ttu-id="a2ecf-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="a2ecf-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="a2ecf-152">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-152">The source of threat assessment request.</span></span> <span data-ttu-id="a2ecf-153">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="a2ecf-154">status</span><span class="sxs-lookup"><span data-stu-id="a2ecf-154">status</span></span>|[<span data-ttu-id="a2ecf-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="a2ecf-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="a2ecf-156">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-156">The assessment process status.</span></span> <span data-ttu-id="a2ecf-157">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2ecf-158">关系</span><span class="sxs-lookup"><span data-stu-id="a2ecf-158">Relationships</span></span>

| <span data-ttu-id="a2ecf-159">关系</span><span class="sxs-lookup"><span data-stu-id="a2ecf-159">Relationship</span></span> | <span data-ttu-id="a2ecf-160">类型</span><span class="sxs-lookup"><span data-stu-id="a2ecf-160">Type</span></span>        | <span data-ttu-id="a2ecf-161">说明</span><span class="sxs-lookup"><span data-stu-id="a2ecf-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a2ecf-162">results</span><span class="sxs-lookup"><span data-stu-id="a2ecf-162">results</span></span>|<span data-ttu-id="a2ecf-163">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a2ecf-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="a2ecf-164">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-164">A collection of threat assessment results.</span></span> <span data-ttu-id="a2ecf-165">只读。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-165">Read-only.</span></span> <span data-ttu-id="a2ecf-166">默认情况下，除非对该属性应用， `GET /threatAssessmentRequests/{id}` 否则不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2ecf-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2ecf-167">JSON representation</span></span>

<span data-ttu-id="a2ecf-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2ecf-168">The following is a JSON representation of the resource.</span></span>

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


