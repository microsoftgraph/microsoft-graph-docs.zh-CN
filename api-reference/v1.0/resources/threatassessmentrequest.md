---
title: threatAssessmentRequest 资源类型
description: 用于表示威胁评估请求项的抽象请求类型。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e316591f4f9db189b1b21dc2d9c3b8d83358c5da
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158959"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="756af-103">threatAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="756af-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="756af-104">用于表示威胁评估请求项的抽象请求类型。</span><span class="sxs-lookup"><span data-stu-id="756af-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="756af-105">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="756af-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="756af-106">mail ([mailAssessmentRequest](mailAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="756af-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="756af-107">email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource) </span><span class="sxs-lookup"><span data-stu-id="756af-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="756af-108">file ([fileAssessmentRequest](fileAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="756af-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="756af-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="756af-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="756af-110">方法</span><span class="sxs-lookup"><span data-stu-id="756af-110">Methods</span></span>

| <span data-ttu-id="756af-111">方法</span><span class="sxs-lookup"><span data-stu-id="756af-111">Method</span></span>       | <span data-ttu-id="756af-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="756af-112">Return Type</span></span> | <span data-ttu-id="756af-113">说明</span><span class="sxs-lookup"><span data-stu-id="756af-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="756af-114">列出 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="756af-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="756af-115">[threatAssessmentRequest](threatassessmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="756af-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="756af-116">列出租户下的所有威胁评估请求。</span><span class="sxs-lookup"><span data-stu-id="756af-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="756af-117">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="756af-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="756af-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="756af-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="756af-119">通过发布派生的资源类型创建新的威胁评估请求[：mailAssessmentRequest](../resources/mailAssessmentRequest.md) [、emailFileAssessmentRequest、fileAssessmentRequest](../resources/emailFileAssessmentRequest.md) [、urlAssessmentRequest。](../resources/urlAssessmentRequest.md) [](../resources/fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="756af-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="756af-120">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="756af-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="756af-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="756af-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="756af-122">检索指定 **threatAssessmentRequest** 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="756af-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="756af-123">属性</span><span class="sxs-lookup"><span data-stu-id="756af-123">Properties</span></span>

| <span data-ttu-id="756af-124">属性</span><span class="sxs-lookup"><span data-stu-id="756af-124">Property</span></span>     | <span data-ttu-id="756af-125">类型</span><span class="sxs-lookup"><span data-stu-id="756af-125">Type</span></span>        | <span data-ttu-id="756af-126">说明</span><span class="sxs-lookup"><span data-stu-id="756af-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="756af-127">category</span><span class="sxs-lookup"><span data-stu-id="756af-127">category</span></span>|[<span data-ttu-id="756af-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="756af-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="756af-129">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="756af-129">The threat category.</span></span> <span data-ttu-id="756af-130">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="756af-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="756af-131">contentType</span><span class="sxs-lookup"><span data-stu-id="756af-131">contentType</span></span>|[<span data-ttu-id="756af-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="756af-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="756af-133">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="756af-133">The content type of threat assessment.</span></span> <span data-ttu-id="756af-134">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="756af-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="756af-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="756af-135">createdBy</span></span>|[<span data-ttu-id="756af-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="756af-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="756af-137">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="756af-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="756af-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="756af-138">createdDateTime</span></span>|<span data-ttu-id="756af-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="756af-139">DateTimeOffset</span></span>|<span data-ttu-id="756af-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="756af-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="756af-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="756af-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="756af-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="756af-142">expectedAssessment</span></span>|[<span data-ttu-id="756af-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="756af-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="756af-144">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="756af-144">The expected assessment from submitter.</span></span> <span data-ttu-id="756af-145">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="756af-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="756af-146">id</span><span class="sxs-lookup"><span data-stu-id="756af-146">id</span></span>|<span data-ttu-id="756af-147">String</span><span class="sxs-lookup"><span data-stu-id="756af-147">String</span></span>|<span data-ttu-id="756af-148">威胁评估请求 ID 是 GUID (全局) 。</span><span class="sxs-lookup"><span data-stu-id="756af-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="756af-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="756af-149">requestSource</span></span>|[<span data-ttu-id="756af-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="756af-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="756af-151">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="756af-151">The source of the threat assessment request.</span></span> <span data-ttu-id="756af-152">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="756af-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="756af-153">status</span><span class="sxs-lookup"><span data-stu-id="756af-153">status</span></span>|[<span data-ttu-id="756af-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="756af-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="756af-155">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="756af-155">The assessment process status.</span></span> <span data-ttu-id="756af-156">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="756af-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="756af-157">关系</span><span class="sxs-lookup"><span data-stu-id="756af-157">Relationships</span></span>

| <span data-ttu-id="756af-158">关系</span><span class="sxs-lookup"><span data-stu-id="756af-158">Relationship</span></span> | <span data-ttu-id="756af-159">类型</span><span class="sxs-lookup"><span data-stu-id="756af-159">Type</span></span>        | <span data-ttu-id="756af-160">说明</span><span class="sxs-lookup"><span data-stu-id="756af-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="756af-161">results</span><span class="sxs-lookup"><span data-stu-id="756af-161">results</span></span>|<span data-ttu-id="756af-162">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="756af-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="756af-163">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="756af-163">A collection of threat assessment results.</span></span> <span data-ttu-id="756af-164">只读。</span><span class="sxs-lookup"><span data-stu-id="756af-164">Read-only.</span></span> <span data-ttu-id="756af-165">默认情况下，除非对该属性应用， `GET /threatAssessmentRequests/{id}` 否则不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="756af-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="756af-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="756af-166">JSON representation</span></span>

<span data-ttu-id="756af-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="756af-167">The following is a JSON representation of the resource.</span></span>

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

