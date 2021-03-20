---
title: urlAssessmentRequest 资源类型
description: 用于创建和检索 URL 威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3d206e14f61bf273f8764a34e3d5ef6cbd154190
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950252"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="dce68-103">urlAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="dce68-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="dce68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dce68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dce68-105">用于创建和检索 URL 威胁评估，派生自 [threatAssessmentRequest](threatAssessmentRequest.md)。</span><span class="sxs-lookup"><span data-stu-id="dce68-105">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dce68-106">Methods</span><span class="sxs-lookup"><span data-stu-id="dce68-106">Methods</span></span>

| <span data-ttu-id="dce68-107">方法</span><span class="sxs-lookup"><span data-stu-id="dce68-107">Method</span></span>       | <span data-ttu-id="dce68-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="dce68-108">Return Type</span></span> | <span data-ttu-id="dce68-109">说明</span><span class="sxs-lookup"><span data-stu-id="dce68-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dce68-110">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dce68-110">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="dce68-111">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dce68-111">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="dce68-112">通过发布 **urlAssessmentRequest** 对象创建新的 URL 评估请求。</span><span class="sxs-lookup"><span data-stu-id="dce68-112">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="dce68-113">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dce68-113">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="dce68-114">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="dce68-114">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="dce68-115">读取 **urlAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dce68-115">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dce68-116">属性</span><span class="sxs-lookup"><span data-stu-id="dce68-116">Properties</span></span>

| <span data-ttu-id="dce68-117">属性</span><span class="sxs-lookup"><span data-stu-id="dce68-117">Property</span></span>     | <span data-ttu-id="dce68-118">类型</span><span class="sxs-lookup"><span data-stu-id="dce68-118">Type</span></span>        | <span data-ttu-id="dce68-119">说明</span><span class="sxs-lookup"><span data-stu-id="dce68-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dce68-120">url</span><span class="sxs-lookup"><span data-stu-id="dce68-120">url</span></span>|<span data-ttu-id="dce68-121">String</span><span class="sxs-lookup"><span data-stu-id="dce68-121">String</span></span>|<span data-ttu-id="dce68-122">URL 字符串。</span><span class="sxs-lookup"><span data-stu-id="dce68-122">The URL string.</span></span>|
|<span data-ttu-id="dce68-123">“类别”</span><span class="sxs-lookup"><span data-stu-id="dce68-123">category</span></span>|[<span data-ttu-id="dce68-124">threatCategory</span><span class="sxs-lookup"><span data-stu-id="dce68-124">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="dce68-125">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="dce68-125">The threat category.</span></span> <span data-ttu-id="dce68-126">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="dce68-126">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="dce68-127">contentType</span><span class="sxs-lookup"><span data-stu-id="dce68-127">contentType</span></span>|[<span data-ttu-id="dce68-128">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="dce68-128">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="dce68-129">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="dce68-129">The content type of the threat assessment.</span></span> <span data-ttu-id="dce68-130">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="dce68-130">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="dce68-131">createdBy</span><span class="sxs-lookup"><span data-stu-id="dce68-131">createdBy</span></span>|[<span data-ttu-id="dce68-132">identitySet</span><span class="sxs-lookup"><span data-stu-id="dce68-132">identitySet</span></span>](identityset.md)|<span data-ttu-id="dce68-133">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="dce68-133">The threat assessment request creator.</span></span>|
|<span data-ttu-id="dce68-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dce68-134">createdDateTime</span></span>|<span data-ttu-id="dce68-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dce68-135">DateTimeOffset</span></span>|<span data-ttu-id="dce68-136">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="dce68-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dce68-137">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="dce68-137">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="dce68-138">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="dce68-138">expectedAssessment</span></span>|[<span data-ttu-id="dce68-139">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="dce68-139">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="dce68-140">来自提交项的预期评估。</span><span class="sxs-lookup"><span data-stu-id="dce68-140">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="dce68-141">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="dce68-141">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="dce68-142">id</span><span class="sxs-lookup"><span data-stu-id="dce68-142">id</span></span>|<span data-ttu-id="dce68-143">String</span><span class="sxs-lookup"><span data-stu-id="dce68-143">String</span></span>|<span data-ttu-id="dce68-144">威胁评估请求 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="dce68-144">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="dce68-145">requestSource</span><span class="sxs-lookup"><span data-stu-id="dce68-145">requestSource</span></span>|[<span data-ttu-id="dce68-146">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="dce68-146">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="dce68-147">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="dce68-147">The source of the threat assessment request.</span></span> <span data-ttu-id="dce68-148">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="dce68-148">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="dce68-149">状态</span><span class="sxs-lookup"><span data-stu-id="dce68-149">status</span></span>|[<span data-ttu-id="dce68-150">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="dce68-150">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="dce68-151">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="dce68-151">The assessment process status.</span></span> <span data-ttu-id="dce68-152">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="dce68-152">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dce68-153">关系</span><span class="sxs-lookup"><span data-stu-id="dce68-153">Relationships</span></span>

| <span data-ttu-id="dce68-154">关系</span><span class="sxs-lookup"><span data-stu-id="dce68-154">Relationship</span></span> | <span data-ttu-id="dce68-155">类型</span><span class="sxs-lookup"><span data-stu-id="dce68-155">Type</span></span>        | <span data-ttu-id="dce68-156">说明</span><span class="sxs-lookup"><span data-stu-id="dce68-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dce68-157">results</span><span class="sxs-lookup"><span data-stu-id="dce68-157">results</span></span>|<span data-ttu-id="dce68-158">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dce68-158">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="dce68-159">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="dce68-159">A collection of threat assessment results.</span></span> <span data-ttu-id="dce68-160">只读。</span><span class="sxs-lookup"><span data-stu-id="dce68-160">Read-only.</span></span> <span data-ttu-id="dce68-161">默认情况下， `GET /threatAssessmentRequests/{id}` 除非对该属性应用 ，否则 不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="dce68-161">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dce68-162">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dce68-162">JSON representation</span></span>

<span data-ttu-id="dce68-163">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dce68-163">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.urlAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
  "url": "String",
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
  "description": "urlAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


