---
title: threatAssessmentRequest 资源类型
description: 用于表示威胁评估请求项的抽象威胁类型。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 00a180d1d78c47a50e44fc7606d65fa94cc8e3e2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721598"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="e3bfc-103">threatAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3bfc-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="e3bfc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3bfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3bfc-105">用于表示威胁评估请求项的抽象威胁类型。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-105">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="e3bfc-106">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="e3bfc-106">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="e3bfc-107">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="e3bfc-107">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="e3bfc-108">[emailFileAssessmentRequest](emailFileAssessmentRequest.md)资源 (电子邮件) </span><span class="sxs-lookup"><span data-stu-id="e3bfc-108">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="e3bfc-109">file ([fileAssessmentRequest](fileAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="e3bfc-109">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="e3bfc-110">URL ([urlAssessmentRequest](urlAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="e3bfc-110">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="e3bfc-111">方法</span><span class="sxs-lookup"><span data-stu-id="e3bfc-111">Methods</span></span>

| <span data-ttu-id="e3bfc-112">方法</span><span class="sxs-lookup"><span data-stu-id="e3bfc-112">Method</span></span>       | <span data-ttu-id="e3bfc-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3bfc-113">Return Type</span></span> | <span data-ttu-id="e3bfc-114">说明</span><span class="sxs-lookup"><span data-stu-id="e3bfc-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e3bfc-115">列出 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e3bfc-115">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="e3bfc-116">[threatAssessmentRequest](threatassessmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3bfc-116">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="e3bfc-117">列出租户下的所有威胁评估请求。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-117">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="e3bfc-118">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e3bfc-118">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="e3bfc-119">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e3bfc-119">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="e3bfc-120">通过发布派生的资源类型创建新的威胁评估请求[：mailAssessmentRequest](../resources/mailAssessmentRequest.md) [、emailFileAssessmentRequest、fileAssessmentRequest](../resources/emailFileAssessmentRequest.md) [、urlAssessmentRequest。](../resources/urlAssessmentRequest.md) [](../resources/fileAssessmentRequest.md)</span><span class="sxs-lookup"><span data-stu-id="e3bfc-120">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="e3bfc-121">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e3bfc-121">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="e3bfc-122">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="e3bfc-122">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="e3bfc-123">检索指定 **threatAssessmentRequest** 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-123">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3bfc-124">属性</span><span class="sxs-lookup"><span data-stu-id="e3bfc-124">Properties</span></span>

| <span data-ttu-id="e3bfc-125">属性</span><span class="sxs-lookup"><span data-stu-id="e3bfc-125">Property</span></span>     | <span data-ttu-id="e3bfc-126">类型</span><span class="sxs-lookup"><span data-stu-id="e3bfc-126">Type</span></span>        | <span data-ttu-id="e3bfc-127">说明</span><span class="sxs-lookup"><span data-stu-id="e3bfc-127">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="e3bfc-128">category</span><span class="sxs-lookup"><span data-stu-id="e3bfc-128">category</span></span>|[<span data-ttu-id="e3bfc-129">threatCategory</span><span class="sxs-lookup"><span data-stu-id="e3bfc-129">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="e3bfc-130">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-130">The threat category.</span></span> <span data-ttu-id="e3bfc-131">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-131">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="e3bfc-132">contentType</span><span class="sxs-lookup"><span data-stu-id="e3bfc-132">contentType</span></span>|[<span data-ttu-id="e3bfc-133">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="e3bfc-133">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="e3bfc-134">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-134">The content type of threat assessment.</span></span> <span data-ttu-id="e3bfc-135">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-135">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="e3bfc-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="e3bfc-136">createdBy</span></span>|[<span data-ttu-id="e3bfc-137">identitySet</span><span class="sxs-lookup"><span data-stu-id="e3bfc-137">identitySet</span></span>](identityset.md)|<span data-ttu-id="e3bfc-138">威胁评估请求创建者。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-138">The threat assessment request creator.</span></span>|
|<span data-ttu-id="e3bfc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3bfc-139">createdDateTime</span></span>|<span data-ttu-id="e3bfc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3bfc-140">DateTimeOffset</span></span>|<span data-ttu-id="e3bfc-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e3bfc-142">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-142">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e3bfc-143">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="e3bfc-143">expectedAssessment</span></span>|[<span data-ttu-id="e3bfc-144">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="e3bfc-144">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="e3bfc-145">提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-145">The expected assessment from submitter.</span></span> <span data-ttu-id="e3bfc-146">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-146">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="e3bfc-147">id</span><span class="sxs-lookup"><span data-stu-id="e3bfc-147">id</span></span>|<span data-ttu-id="e3bfc-148">String</span><span class="sxs-lookup"><span data-stu-id="e3bfc-148">String</span></span>|<span data-ttu-id="e3bfc-149">威胁评估请求 ID 是 GUID (全局唯一) 。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-149">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="e3bfc-150">requestSource</span><span class="sxs-lookup"><span data-stu-id="e3bfc-150">requestSource</span></span>|[<span data-ttu-id="e3bfc-151">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="e3bfc-151">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="e3bfc-152">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-152">The source of the threat assessment request.</span></span> <span data-ttu-id="e3bfc-153">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-153">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="e3bfc-154">状态</span><span class="sxs-lookup"><span data-stu-id="e3bfc-154">status</span></span>|[<span data-ttu-id="e3bfc-155">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="e3bfc-155">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="e3bfc-156">评估流程状态。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-156">The assessment process status.</span></span> <span data-ttu-id="e3bfc-157">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-157">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3bfc-158">关系</span><span class="sxs-lookup"><span data-stu-id="e3bfc-158">Relationships</span></span>

| <span data-ttu-id="e3bfc-159">关系</span><span class="sxs-lookup"><span data-stu-id="e3bfc-159">Relationship</span></span> | <span data-ttu-id="e3bfc-160">类型</span><span class="sxs-lookup"><span data-stu-id="e3bfc-160">Type</span></span>        | <span data-ttu-id="e3bfc-161">说明</span><span class="sxs-lookup"><span data-stu-id="e3bfc-161">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e3bfc-162">results</span><span class="sxs-lookup"><span data-stu-id="e3bfc-162">results</span></span>|<span data-ttu-id="e3bfc-163">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e3bfc-163">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="e3bfc-164">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-164">A collection of threat assessment results.</span></span> <span data-ttu-id="e3bfc-165">只读。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-165">Read-only.</span></span> <span data-ttu-id="e3bfc-166">默认情况下，除非 `GET /threatAssessmentRequests/{id}` 应用此属性，否则不会返回 `$expand` 此属性。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-166">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3bfc-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3bfc-167">JSON representation</span></span>

<span data-ttu-id="e3bfc-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3bfc-168">The following is a JSON representation of the resource.</span></span>

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


