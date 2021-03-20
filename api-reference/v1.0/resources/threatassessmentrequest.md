---
title: threatAssessmentRequest 资源类型
description: 用于表示威胁评估请求项目的抽象集合类型。
localization_priority: Normal
author: hafen-ms
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: aeb3733ed3c93896d701851a928e216a2b9c7c7d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952499"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="9a879-103">threatAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a879-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="9a879-104">用于表示威胁评估请求项目的抽象集合类型。</span><span class="sxs-lookup"><span data-stu-id="9a879-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="9a879-105">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="9a879-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="9a879-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="9a879-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="9a879-107">emailFile [ (AssessmentRequest](emailFileAssessmentRequest.md)) </span><span class="sxs-lookup"><span data-stu-id="9a879-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="9a879-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="9a879-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="9a879-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="9a879-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="9a879-110">Methods</span><span class="sxs-lookup"><span data-stu-id="9a879-110">Methods</span></span>

| <span data-ttu-id="9a879-111">方法</span><span class="sxs-lookup"><span data-stu-id="9a879-111">Method</span></span>       | <span data-ttu-id="9a879-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a879-112">Return Type</span></span> | <span data-ttu-id="9a879-113">说明</span><span class="sxs-lookup"><span data-stu-id="9a879-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9a879-114">列出 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="9a879-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="9a879-115">[threatAssessmentRequest](threatassessmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a879-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="9a879-116">列出租户下的所有威胁评估请求。</span><span class="sxs-lookup"><span data-stu-id="9a879-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="9a879-117">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="9a879-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="9a879-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="9a879-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="9a879-119">通过发布派生的资源类型创建新的威胁评估请求[：mailAssessmentRequest](../resources/mailAssessmentRequest.md) [、emailFileAssessmentRequest、fileAssessmentRequest](../resources/emailFileAssessmentRequest.md) [、urlAssessmentRequest](../resources/urlAssessmentRequest.md)。 [](../resources/fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="9a879-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="9a879-120">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="9a879-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="9a879-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="9a879-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="9a879-122">检索指定 **threatAssessmentRequest** 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9a879-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="9a879-123">属性</span><span class="sxs-lookup"><span data-stu-id="9a879-123">Properties</span></span>

| <span data-ttu-id="9a879-124">属性</span><span class="sxs-lookup"><span data-stu-id="9a879-124">Property</span></span>     | <span data-ttu-id="9a879-125">类型</span><span class="sxs-lookup"><span data-stu-id="9a879-125">Type</span></span>        | <span data-ttu-id="9a879-126">说明</span><span class="sxs-lookup"><span data-stu-id="9a879-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="9a879-127">category</span><span class="sxs-lookup"><span data-stu-id="9a879-127">category</span></span>|[<span data-ttu-id="9a879-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="9a879-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="9a879-129">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="9a879-129">The threat category.</span></span> <span data-ttu-id="9a879-130">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="9a879-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="9a879-131">contentType</span><span class="sxs-lookup"><span data-stu-id="9a879-131">contentType</span></span>|[<span data-ttu-id="9a879-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="9a879-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="9a879-133">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="9a879-133">The content type of threat assessment.</span></span> <span data-ttu-id="9a879-134">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="9a879-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="9a879-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="9a879-135">createdBy</span></span>|[<span data-ttu-id="9a879-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="9a879-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="9a879-137">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="9a879-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="9a879-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9a879-138">createdDateTime</span></span>|<span data-ttu-id="9a879-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a879-139">DateTimeOffset</span></span>|<span data-ttu-id="9a879-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="9a879-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9a879-141">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="9a879-141">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="9a879-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="9a879-142">expectedAssessment</span></span>|[<span data-ttu-id="9a879-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="9a879-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="9a879-144">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="9a879-144">The expected assessment from submitter.</span></span> <span data-ttu-id="9a879-145">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="9a879-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="9a879-146">id</span><span class="sxs-lookup"><span data-stu-id="9a879-146">id</span></span>|<span data-ttu-id="9a879-147">String</span><span class="sxs-lookup"><span data-stu-id="9a879-147">String</span></span>|<span data-ttu-id="9a879-148">威胁评估请求 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="9a879-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="9a879-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="9a879-149">requestSource</span></span>|[<span data-ttu-id="9a879-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="9a879-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="9a879-151">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="9a879-151">The source of the threat assessment request.</span></span> <span data-ttu-id="9a879-152">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="9a879-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="9a879-153">状态</span><span class="sxs-lookup"><span data-stu-id="9a879-153">status</span></span>|[<span data-ttu-id="9a879-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="9a879-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="9a879-155">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="9a879-155">The assessment process status.</span></span> <span data-ttu-id="9a879-156">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="9a879-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a879-157">关系</span><span class="sxs-lookup"><span data-stu-id="9a879-157">Relationships</span></span>

| <span data-ttu-id="9a879-158">关系</span><span class="sxs-lookup"><span data-stu-id="9a879-158">Relationship</span></span> | <span data-ttu-id="9a879-159">类型</span><span class="sxs-lookup"><span data-stu-id="9a879-159">Type</span></span>        | <span data-ttu-id="9a879-160">说明</span><span class="sxs-lookup"><span data-stu-id="9a879-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a879-161">results</span><span class="sxs-lookup"><span data-stu-id="9a879-161">results</span></span>|<span data-ttu-id="9a879-162">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a879-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="9a879-163">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="9a879-163">A collection of threat assessment results.</span></span> <span data-ttu-id="9a879-164">只读。</span><span class="sxs-lookup"><span data-stu-id="9a879-164">Read-only.</span></span> <span data-ttu-id="9a879-165">默认情况下， `GET /threatAssessmentRequests/{id}` 除非对该属性应用 ，否则 不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="9a879-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9a879-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a879-166">JSON representation</span></span>

<span data-ttu-id="9a879-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a879-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "keyProperty": "id"
}-->

```json
{
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
  "description": "threatAssessmentRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

