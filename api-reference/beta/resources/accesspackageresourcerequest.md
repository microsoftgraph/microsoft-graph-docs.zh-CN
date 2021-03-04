---
title: accessPackageResourceRequest 资源类型
description: 访问包资源请求是向目录添加资源的请求，以便可以在目录的一个或多个访问包中使用资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7e045a327869432eb58d135262da1a3f4fa91307
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433255"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="e2350-103">accessPackageResourceRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2350-103">accessPackageResourceRequest resource type</span></span>

<span data-ttu-id="e2350-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2350-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2350-105">在 [Azure AD](entitlementmanagement-root.md)权利管理中，访问包资源请求是向目录添加资源的请求，以便资源的角色可在目录的一个或多个访问包中使用，或者从访问包不再需要的目录中删除资源。</span><span class="sxs-lookup"><span data-stu-id="e2350-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages, or to remove a resource from a catalog that is no longer needed by the access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="e2350-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e2350-106">Methods</span></span>

| <span data-ttu-id="e2350-107">方法</span><span class="sxs-lookup"><span data-stu-id="e2350-107">Method</span></span>       | <span data-ttu-id="e2350-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e2350-108">Return Type</span></span> | <span data-ttu-id="e2350-109">说明</span><span class="sxs-lookup"><span data-stu-id="e2350-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e2350-110">列出 accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="e2350-110">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="e2350-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e2350-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="e2350-112">检索 **accessPackageResourceRequest 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="e2350-112">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="e2350-113">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="e2350-113">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="e2350-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="e2350-114">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="e2350-115">创建新的 **accessPackageResourceRequest** 对象。</span><span class="sxs-lookup"><span data-stu-id="e2350-115">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e2350-116">属性</span><span class="sxs-lookup"><span data-stu-id="e2350-116">Properties</span></span>

| <span data-ttu-id="e2350-117">属性</span><span class="sxs-lookup"><span data-stu-id="e2350-117">Property</span></span>     | <span data-ttu-id="e2350-118">类型</span><span class="sxs-lookup"><span data-stu-id="e2350-118">Type</span></span>        | <span data-ttu-id="e2350-119">说明</span><span class="sxs-lookup"><span data-stu-id="e2350-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2350-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="e2350-120">catalogId</span></span>|<span data-ttu-id="e2350-121">String</span><span class="sxs-lookup"><span data-stu-id="e2350-121">String</span></span>|<span data-ttu-id="e2350-122">访问包目录的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e2350-122">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="e2350-123">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e2350-123">expirationDateTime</span></span>|<span data-ttu-id="e2350-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2350-124">DateTimeOffset</span></span>|<span data-ttu-id="e2350-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e2350-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e2350-127">id</span><span class="sxs-lookup"><span data-stu-id="e2350-127">id</span></span>|<span data-ttu-id="e2350-128">String</span><span class="sxs-lookup"><span data-stu-id="e2350-128">String</span></span>| <span data-ttu-id="e2350-129">只读。</span><span class="sxs-lookup"><span data-stu-id="e2350-129">Read-only.</span></span>|
|<span data-ttu-id="e2350-130">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="e2350-130">isValidationOnly</span></span>|<span data-ttu-id="e2350-131">布尔</span><span class="sxs-lookup"><span data-stu-id="e2350-131">Boolean</span></span>|<span data-ttu-id="e2350-132">如果设置，则不添加资源。</span><span class="sxs-lookup"><span data-stu-id="e2350-132">If set, does not add the resource.</span></span>|
|<span data-ttu-id="e2350-133">justification</span><span class="sxs-lookup"><span data-stu-id="e2350-133">justification</span></span>|<span data-ttu-id="e2350-134">String</span><span class="sxs-lookup"><span data-stu-id="e2350-134">String</span></span>|<span data-ttu-id="e2350-135">请求者添加或删除资源的理由。</span><span class="sxs-lookup"><span data-stu-id="e2350-135">The requestor's justification for adding or removing the resource.</span></span>|
|<span data-ttu-id="e2350-136">requestState</span><span class="sxs-lookup"><span data-stu-id="e2350-136">requestState</span></span>|<span data-ttu-id="e2350-137">String</span><span class="sxs-lookup"><span data-stu-id="e2350-137">String</span></span>| <span data-ttu-id="e2350-138">服务能否将资源添加到目录的结果。</span><span class="sxs-lookup"><span data-stu-id="e2350-138">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="e2350-139">该值是 `Delivered` 添加或删除资源。</span><span class="sxs-lookup"><span data-stu-id="e2350-139">The value is `Delivered` if the resource was added or removed.</span></span> <span data-ttu-id="e2350-140">只读。</span><span class="sxs-lookup"><span data-stu-id="e2350-140">Read-Only.</span></span>|
|<span data-ttu-id="e2350-141">requestStatus</span><span class="sxs-lookup"><span data-stu-id="e2350-141">requestStatus</span></span>|<span data-ttu-id="e2350-142">String</span><span class="sxs-lookup"><span data-stu-id="e2350-142">String</span></span>|<span data-ttu-id="e2350-143">只读。</span><span class="sxs-lookup"><span data-stu-id="e2350-143">Read-only.</span></span>|
|<span data-ttu-id="e2350-144">requestType</span><span class="sxs-lookup"><span data-stu-id="e2350-144">requestType</span></span>|<span data-ttu-id="e2350-145">String</span><span class="sxs-lookup"><span data-stu-id="e2350-145">String</span></span>|<span data-ttu-id="e2350-146">`AdminAdd`用于添加资源（如果调用方是管理员或资源所有者） `AdminRemove` 或删除资源。</span><span class="sxs-lookup"><span data-stu-id="e2350-146">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner, or `AdminRemove` to remove a resource.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e2350-147">关系</span><span class="sxs-lookup"><span data-stu-id="e2350-147">Relationships</span></span>

| <span data-ttu-id="e2350-148">关系</span><span class="sxs-lookup"><span data-stu-id="e2350-148">Relationship</span></span> | <span data-ttu-id="e2350-149">类型</span><span class="sxs-lookup"><span data-stu-id="e2350-149">Type</span></span>        | <span data-ttu-id="e2350-150">说明</span><span class="sxs-lookup"><span data-stu-id="e2350-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e2350-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e2350-151">accessPackageResource</span></span>|[<span data-ttu-id="e2350-152">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="e2350-152">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="e2350-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="e2350-153">Nullable.</span></span>|
|<span data-ttu-id="e2350-154">requestor</span><span class="sxs-lookup"><span data-stu-id="e2350-154">requestor</span></span>|[<span data-ttu-id="e2350-155">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="e2350-155">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="e2350-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="e2350-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e2350-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2350-158">JSON representation</span></span>

<span data-ttu-id="e2350-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2350-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "keyProperty": "id"
}-->

```json
{
  "catalogId": "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
  "expirationDateTime": "String (timestamp)",
  "id": "1fe272f0-d463-42aa-a9a8-b07ab50a1c4d",
  "isValidationOnly": false,
  "justification": "String",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "requestType": "AdminAdd"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


