---
title: threatAssessmentRequest 资源类型
description: 用于表示威胁评估请求项目的抽象资源类型。
localization_priority: Normal
author: hafen-ms
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: df3f501ad281bcfced2e476b90e95b663fedef58
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48090891"
---
# <a name="threatassessmentrequest-resource-type"></a><span data-ttu-id="0757c-103">threatAssessmentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="0757c-103">threatAssessmentRequest resource type</span></span>

<span data-ttu-id="0757c-104">用于表示威胁评估请求项目的抽象资源类型。</span><span class="sxs-lookup"><span data-stu-id="0757c-104">An abstract resouce type used to represent a threat assessment request item.</span></span>

<span data-ttu-id="0757c-105">威胁评估请求可以是以下类型之一：</span><span class="sxs-lookup"><span data-stu-id="0757c-105">A threat assessment request can be one of the following types:</span></span>

* <span data-ttu-id="0757c-106">邮件 ([mailAssessmentRequest](mailAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="0757c-106">Mail ([mailAssessmentRequest](mailAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="0757c-107">电子邮件文件 ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="0757c-107">Email file ([emailFileAssessmentRequest](emailFileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="0757c-108">文件 ([fileAssessmentRequest](fileAssessmentRequest.md) 资源) </span><span class="sxs-lookup"><span data-stu-id="0757c-108">File ([fileAssessmentRequest](fileAssessmentRequest.md) resource)</span></span>
* <span data-ttu-id="0757c-109">[UrlAssessmentRequest](urlAssessmentRequest.md)资源的 URL () </span><span class="sxs-lookup"><span data-stu-id="0757c-109">URL ([urlAssessmentRequest](urlAssessmentRequest.md) resource)</span></span>

## <a name="methods"></a><span data-ttu-id="0757c-110">方法</span><span class="sxs-lookup"><span data-stu-id="0757c-110">Methods</span></span>

| <span data-ttu-id="0757c-111">方法</span><span class="sxs-lookup"><span data-stu-id="0757c-111">Method</span></span>       | <span data-ttu-id="0757c-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="0757c-112">Return Type</span></span> | <span data-ttu-id="0757c-113">说明</span><span class="sxs-lookup"><span data-stu-id="0757c-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0757c-114">列出 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="0757c-114">List threatAssessmentRequest</span></span>](../api/informationprotection-list-threatassessmentrequests.md) | <span data-ttu-id="0757c-115">[threatAssessmentRequest](threatassessmentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0757c-115">[threatAssessmentRequest](threatassessmentrequest.md) collection</span></span> | <span data-ttu-id="0757c-116">列出租户下的所有威胁评估请求。</span><span class="sxs-lookup"><span data-stu-id="0757c-116">List all threat assessment requests under tenant.</span></span> |
| [<span data-ttu-id="0757c-117">创建 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="0757c-117">Create threatAssessmentRequest</span></span>](../api/informationprotection-post-threatassessmentrequests.md) | [<span data-ttu-id="0757c-118">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="0757c-118">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="0757c-119">通过发布派生的资源类型创建新的威胁评估请求： [mailAssessmentRequest](../resources/mailAssessmentRequest.md)、 [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md)、 [fileAssessmentRequest](../resources/fileAssessmentRequest.md)、 [urlAssessmentRequest](../resources/urlAssessmentRequest.md)。</span><span class="sxs-lookup"><span data-stu-id="0757c-119">Create a new threat assessment request by posting a derived resource type: [mailAssessmentRequest](../resources/mailAssessmentRequest.md), [emailFileAssessmentRequest](../resources/emailFileAssessmentRequest.md), [fileAssessmentRequest](../resources/fileAssessmentRequest.md), [urlAssessmentRequest](../resources/urlAssessmentRequest.md).</span></span> |
| [<span data-ttu-id="0757c-120">获取 threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="0757c-120">Get threatAssessmentRequest</span></span>](../api/threatassessmentrequest-get.md) | [<span data-ttu-id="0757c-121">threatAssessmentRequest</span><span class="sxs-lookup"><span data-stu-id="0757c-121">threatAssessmentRequest</span></span>](threatassessmentrequest.md) | <span data-ttu-id="0757c-122">检索指定的 **threatAssessmentRequest** 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0757c-122">Retrieve the properties and relationships of a specified **threatAssessmentRequest** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="0757c-123">属性</span><span class="sxs-lookup"><span data-stu-id="0757c-123">Properties</span></span>

| <span data-ttu-id="0757c-124">属性</span><span class="sxs-lookup"><span data-stu-id="0757c-124">Property</span></span>     | <span data-ttu-id="0757c-125">类型</span><span class="sxs-lookup"><span data-stu-id="0757c-125">Type</span></span>        | <span data-ttu-id="0757c-126">说明</span><span class="sxs-lookup"><span data-stu-id="0757c-126">Description</span></span> |
| :-------------|:------------|:------------|
|<span data-ttu-id="0757c-127">category</span><span class="sxs-lookup"><span data-stu-id="0757c-127">category</span></span>|[<span data-ttu-id="0757c-128">threatCategory</span><span class="sxs-lookup"><span data-stu-id="0757c-128">threatCategory</span></span>](enums.md#threatcategory-values)|<span data-ttu-id="0757c-129">威胁类别。</span><span class="sxs-lookup"><span data-stu-id="0757c-129">The threat category.</span></span> <span data-ttu-id="0757c-130">可取值为：`spam`、`phishing`、`malware`。</span><span class="sxs-lookup"><span data-stu-id="0757c-130">Possible values are: `spam`, `phishing`, `malware`.</span></span>|
|<span data-ttu-id="0757c-131">contentType</span><span class="sxs-lookup"><span data-stu-id="0757c-131">contentType</span></span>|[<span data-ttu-id="0757c-132">threatAssessmentContentType</span><span class="sxs-lookup"><span data-stu-id="0757c-132">threatAssessmentContentType</span></span>](enums.md#threatassessmentcontenttype-values)|<span data-ttu-id="0757c-133">威胁评估的内容类型。</span><span class="sxs-lookup"><span data-stu-id="0757c-133">The content type of threat assessment.</span></span> <span data-ttu-id="0757c-134">可取值为：`mail`、`url`、`file`。</span><span class="sxs-lookup"><span data-stu-id="0757c-134">Possible values are: `mail`, `url`, `file`.</span></span>|
|<span data-ttu-id="0757c-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="0757c-135">createdBy</span></span>|[<span data-ttu-id="0757c-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="0757c-136">identitySet</span></span>](identityset.md)|<span data-ttu-id="0757c-137">威胁评估请求创建程序。</span><span class="sxs-lookup"><span data-stu-id="0757c-137">The threat assessment request creator.</span></span>|
|<span data-ttu-id="0757c-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0757c-138">createdDateTime</span></span>|<span data-ttu-id="0757c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0757c-139">DateTimeOffset</span></span>|<span data-ttu-id="0757c-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="0757c-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0757c-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="0757c-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="0757c-142">expectedAssessment</span><span class="sxs-lookup"><span data-stu-id="0757c-142">expectedAssessment</span></span>|[<span data-ttu-id="0757c-143">threatExpectedAssessment</span><span class="sxs-lookup"><span data-stu-id="0757c-143">threatExpectedAssessment</span></span>](enums.md#threatexpectedassessment-values)|<span data-ttu-id="0757c-144">来自提交者的预期评估。</span><span class="sxs-lookup"><span data-stu-id="0757c-144">The expected assessment from submitter.</span></span> <span data-ttu-id="0757c-145">可能的值是：`block`、`unblock`。</span><span class="sxs-lookup"><span data-stu-id="0757c-145">Possible values are: `block`, `unblock`.</span></span>|
|<span data-ttu-id="0757c-146">id</span><span class="sxs-lookup"><span data-stu-id="0757c-146">id</span></span>|<span data-ttu-id="0757c-147">String</span><span class="sxs-lookup"><span data-stu-id="0757c-147">String</span></span>|<span data-ttu-id="0757c-148">威胁评估请求 ID 是 GUID)  (全局唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0757c-148">The threat assessment request ID is a globally unique identifier (GUID).</span></span>|
|<span data-ttu-id="0757c-149">requestSource</span><span class="sxs-lookup"><span data-stu-id="0757c-149">requestSource</span></span>|[<span data-ttu-id="0757c-150">threatAssessmentRequestSource</span><span class="sxs-lookup"><span data-stu-id="0757c-150">threatAssessmentRequestSource</span></span>](enums.md#threatassessmentrequestsource-values)|<span data-ttu-id="0757c-151">威胁评估请求的来源。</span><span class="sxs-lookup"><span data-stu-id="0757c-151">The source of the threat assessment request.</span></span> <span data-ttu-id="0757c-152">可取值为：`user`、`administrator`。</span><span class="sxs-lookup"><span data-stu-id="0757c-152">Possible values are: `user`, `administrator`.</span></span>|
|<span data-ttu-id="0757c-153">status</span><span class="sxs-lookup"><span data-stu-id="0757c-153">status</span></span>|[<span data-ttu-id="0757c-154">threatAssessmentStatus</span><span class="sxs-lookup"><span data-stu-id="0757c-154">threatAssessmentStatus</span></span>](enums.md#threatassessmentstatus-values)|<span data-ttu-id="0757c-155">评估过程状态。</span><span class="sxs-lookup"><span data-stu-id="0757c-155">The assessment process status.</span></span> <span data-ttu-id="0757c-156">可取值为：`pending`、`completed`。</span><span class="sxs-lookup"><span data-stu-id="0757c-156">Possible values are: `pending`, `completed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0757c-157">关系</span><span class="sxs-lookup"><span data-stu-id="0757c-157">Relationships</span></span>

| <span data-ttu-id="0757c-158">关系</span><span class="sxs-lookup"><span data-stu-id="0757c-158">Relationship</span></span> | <span data-ttu-id="0757c-159">类型</span><span class="sxs-lookup"><span data-stu-id="0757c-159">Type</span></span>        | <span data-ttu-id="0757c-160">说明</span><span class="sxs-lookup"><span data-stu-id="0757c-160">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0757c-161">results</span><span class="sxs-lookup"><span data-stu-id="0757c-161">results</span></span>|<span data-ttu-id="0757c-162">[threatAssessmentResult](threatassessmentresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0757c-162">[threatAssessmentResult](threatassessmentresult.md) collection</span></span>|<span data-ttu-id="0757c-163">威胁评估结果的集合。</span><span class="sxs-lookup"><span data-stu-id="0757c-163">A collection of threat assessment results.</span></span> <span data-ttu-id="0757c-164">只读。</span><span class="sxs-lookup"><span data-stu-id="0757c-164">Read-only.</span></span> <span data-ttu-id="0757c-165">默认情况下，a 不 `GET /threatAssessmentRequests/{id}` 会返回此属性，除非您应用于该属性 `$expand` 。</span><span class="sxs-lookup"><span data-stu-id="0757c-165">By default, a `GET /threatAssessmentRequests/{id}` does not return this property unless you apply `$expand` on it.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0757c-166">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0757c-166">JSON representation</span></span>

<span data-ttu-id="0757c-167">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0757c-167">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.threatAssessmentRequest",
  "baseType": "",
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

