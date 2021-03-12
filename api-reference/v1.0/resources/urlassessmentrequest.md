---
title: urlAssessmentRequest 资源类型
description: 用于创建和检索 URL 威胁评估。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5af4d3df971931a6119bd35a11ddbf94fefbbe4e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721703"
---
# <a name="urlassessmentrequest-resource-type"></a><span data-ttu-id="27497-103">urlAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="27497-103">urlAssessmentRequest resource type</span></span>

<span data-ttu-id="27497-104">用于创建和检索 URL 威胁评估，派生自 [threatAssessmentRequest](threatAssessmentRequest.md)。</span><span class="sxs-lookup"><span data-stu-id="27497-104">Used to create and retrieve a URL threat assessment, derived from [threatAssessmentRequest](threatAssessmentRequest.md).</span></span>

## <a name="methods"></a><span data-ttu-id="27497-105">Methods</span><span class="sxs-lookup"><span data-stu-id="27497-105">Methods</span></span>

| <span data-ttu-id="27497-106">方法</span><span class="sxs-lookup"><span data-stu-id="27497-106">Method</span></span>       | <span data-ttu-id="27497-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="27497-107">Return Type</span></span> | <span data-ttu-id="27497-108">说明</span><span class="sxs-lookup"><span data-stu-id="27497-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="27497-109">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="27497-109">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="27497-110">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="27497-110">urlAssessmentRequest</span></span>](urlAssessmentRequest.md) | <span data-ttu-id="27497-111">通过发布 **urlAssessmentRequest** 对象创建新的 URL 评估请求。</span><span class="sxs-lookup"><span data-stu-id="27497-111">Create a new URL assessment request by posting an **urlAssessmentRequest** object.</span></span> |
| [<span data-ttu-id="27497-112">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="27497-112">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="27497-113">urlAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="27497-113">urlAssessmentRequest</span></span>](urlassessmentrequest.md) | <span data-ttu-id="27497-114">读取 **urlAssessmentRequest** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="27497-114">Read the properties and relationships of a **urlAssessmentRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="27497-115">属性</span><span class="sxs-lookup"><span data-stu-id="27497-115">Properties</span></span>

| <span data-ttu-id="27497-116">属性</span><span class="sxs-lookup"><span data-stu-id="27497-116">Property</span></span>     | <span data-ttu-id="27497-117">类型</span><span class="sxs-lookup"><span data-stu-id="27497-117">Type</span></span>        | <span data-ttu-id="27497-118">说明</span><span class="sxs-lookup"><span data-stu-id="27497-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27497-119">url</span><span class="sxs-lookup"><span data-stu-id="27497-119">url</span></span>|<span data-ttu-id="27497-120">String</span><span class="sxs-lookup"><span data-stu-id="27497-120">String</span></span>|<span data-ttu-id="27497-121">URL 字符串。</span><span class="sxs-lookup"><span data-stu-id="27497-121">The URL string.</span></span>|
|<span data-ttu-id="27497-122">“类别”</span><span class="sxs-lookup"><span data-stu-id="27497-122">category</span></span>|[<span data-ttu-id="27497-123">threatCategory</span><span class="sxs-lookup"><span data-stu-id="27497-123">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="27497-124">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="27497-124">The threat category.</span></span> <span data-ttu-id="27497-125">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="27497-125">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="27497-126">contentType</span><span class="sxs-lookup"><span data-stu-id="27497-126">contentType</span></span>|[<span data-ttu-id="27497-127">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="27497-127">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="27497-128">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="27497-128">The content type of the threat assessment.</span></span> <span data-ttu-id="27497-129">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="27497-129">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="27497-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="27497-130">createdBy</span></span>|[<span data-ttu-id="27497-131">identitySet</span><span class="sxs-lookup"><span data-stu-id="27497-131">identitySet</span></span>](identityset.md)|<span data-ttu-id="27497-132">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="27497-132">The threat assessment request creator.</span></span>|
|<span data-ttu-id="27497-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27497-133">createdDateTime</span></span>|<span data-ttu-id="27497-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27497-134">DateTimeOffset</span></span>|<span data-ttu-id="27497-135">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="27497-135">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="27497-136">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="27497-136">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="27497-137">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="27497-137">expectedAssessment</span></span>|[<span data-ttu-id="27497-138">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="27497-138">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="27497-139">来自提交项的预期评估。</span><span class="sxs-lookup"><span data-stu-id="27497-139">The expected assessment from the ubmitter.</span></span> <span data-ttu-id="27497-140">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="27497-140">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="27497-141">id</span><span class="sxs-lookup"><span data-stu-id="27497-141">id</span></span>|<span data-ttu-id="27497-142">字符串</span><span class="sxs-lookup"><span data-stu-id="27497-142">String</span></span>|<span data-ttu-id="27497-143">威胁评估请求 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="27497-143">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="27497-144">requestSource</span><span class="sxs-lookup"><span data-stu-id="27497-144">requestSource</span></span>|[<span data-ttu-id="27497-145">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="27497-145">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="27497-146">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="27497-146">The source of the threat assessment request.</span></span> <span data-ttu-id="27497-147">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="27497-147">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="27497-148">状态</span><span class="sxs-lookup"><span data-stu-id="27497-148">status</span></span>|[<span data-ttu-id="27497-149">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="27497-149">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="27497-150">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="27497-150">The assessment process status.</span></span> <span data-ttu-id="27497-151">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="27497-151">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27497-152">关系</span><span class="sxs-lookup"><span data-stu-id="27497-152">Relationships</span></span>

| <span data-ttu-id="27497-153">关系</span><span class="sxs-lookup"><span data-stu-id="27497-153">Relationship</span></span> | <span data-ttu-id="27497-154">类型</span><span class="sxs-lookup"><span data-stu-id="27497-154">Type</span></span>        | <span data-ttu-id="27497-155">说明</span><span class="sxs-lookup"><span data-stu-id="27497-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="27497-156">results</span><span class="sxs-lookup"><span data-stu-id="27497-156">results</span></span>|<span data-ttu-id="27497-157">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="27497-157">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="27497-158">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="27497-158">A collection of threat assessment results.</span></span> <span data-ttu-id="27497-159">只读。</span><span class="sxs-lookup"><span data-stu-id="27497-159">Read-only.</span></span> <span data-ttu-id="27497-160">默认情况下， `GET /threatAssessmentRequests/{id}` 除非对该属性应用 ，否则 不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="27497-160">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="27497-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27497-161">JSON representation</span></span>

<span data-ttu-id="27497-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27497-162">The following is a JSON representation of the resource.</span></span>

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

