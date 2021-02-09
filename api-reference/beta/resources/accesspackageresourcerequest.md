---
title: accessPackageResourceRequest 资源类型
description: 访问包资源请求是请求将资源添加到目录，以便资源的角色可在目录的一个或多个访问包中使用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 16198df73c51b1b5f7cb7f8c7748da4816800890
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158581"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="98f8b-103">accessPackageResourceRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="98f8b-103">accessPackageResourceRequest resource type</span></span>

<span data-ttu-id="98f8b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98f8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98f8b-105">在 [Azure AD](entitlementmanagement-root.md)权利管理中，访问包资源请求是请求将资源添加到目录，以便资源的角色可在目录的一个或多个访问包中使用，或者从访问包不再需要的目录中删除资源。</span><span class="sxs-lookup"><span data-stu-id="98f8b-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages, or to remove a resource from a catalog that is no longer needed by the access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="98f8b-106">方法</span><span class="sxs-lookup"><span data-stu-id="98f8b-106">Methods</span></span>

| <span data-ttu-id="98f8b-107">方法</span><span class="sxs-lookup"><span data-stu-id="98f8b-107">Method</span></span>       | <span data-ttu-id="98f8b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="98f8b-108">Return Type</span></span> | <span data-ttu-id="98f8b-109">说明</span><span class="sxs-lookup"><span data-stu-id="98f8b-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="98f8b-110">列出 accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="98f8b-110">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="98f8b-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="98f8b-111">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="98f8b-112">检索 **accessPackageResourceRequest 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="98f8b-112">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="98f8b-113">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="98f8b-113">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="98f8b-114">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="98f8b-114">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="98f8b-115">创建新的 **accessPackageResourceRequest** 对象。</span><span class="sxs-lookup"><span data-stu-id="98f8b-115">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="98f8b-116">属性</span><span class="sxs-lookup"><span data-stu-id="98f8b-116">Properties</span></span>

| <span data-ttu-id="98f8b-117">属性</span><span class="sxs-lookup"><span data-stu-id="98f8b-117">Property</span></span>     | <span data-ttu-id="98f8b-118">类型</span><span class="sxs-lookup"><span data-stu-id="98f8b-118">Type</span></span>        | <span data-ttu-id="98f8b-119">说明</span><span class="sxs-lookup"><span data-stu-id="98f8b-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98f8b-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="98f8b-120">catalogId</span></span>|<span data-ttu-id="98f8b-121">String</span><span class="sxs-lookup"><span data-stu-id="98f8b-121">String</span></span>|<span data-ttu-id="98f8b-122">访问包目录的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="98f8b-122">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="98f8b-123">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="98f8b-123">expirationDateTime</span></span>|<span data-ttu-id="98f8b-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98f8b-124">DateTimeOffset</span></span>|<span data-ttu-id="98f8b-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="98f8b-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="98f8b-127">id</span><span class="sxs-lookup"><span data-stu-id="98f8b-127">id</span></span>|<span data-ttu-id="98f8b-128">String</span><span class="sxs-lookup"><span data-stu-id="98f8b-128">String</span></span>| <span data-ttu-id="98f8b-129">只读。</span><span class="sxs-lookup"><span data-stu-id="98f8b-129">Read-only.</span></span>|
|<span data-ttu-id="98f8b-130">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="98f8b-130">isValidationOnly</span></span>|<span data-ttu-id="98f8b-131">布尔</span><span class="sxs-lookup"><span data-stu-id="98f8b-131">Boolean</span></span>|<span data-ttu-id="98f8b-132">如果设置，则不添加资源。</span><span class="sxs-lookup"><span data-stu-id="98f8b-132">If set, does not add the resource.</span></span>|
|<span data-ttu-id="98f8b-133">justification</span><span class="sxs-lookup"><span data-stu-id="98f8b-133">justification</span></span>|<span data-ttu-id="98f8b-134">String</span><span class="sxs-lookup"><span data-stu-id="98f8b-134">String</span></span>|<span data-ttu-id="98f8b-135">请求者添加或删除资源的理由。</span><span class="sxs-lookup"><span data-stu-id="98f8b-135">The requestor's justification for adding or removing the resource.</span></span>|
|<span data-ttu-id="98f8b-136">requestState</span><span class="sxs-lookup"><span data-stu-id="98f8b-136">requestState</span></span>|<span data-ttu-id="98f8b-137">String</span><span class="sxs-lookup"><span data-stu-id="98f8b-137">String</span></span>| <span data-ttu-id="98f8b-138">服务能否将资源添加到目录的结果。</span><span class="sxs-lookup"><span data-stu-id="98f8b-138">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="98f8b-139">该值是 `Delivered` 添加或删除资源。</span><span class="sxs-lookup"><span data-stu-id="98f8b-139">The value is `Delivered` if the resource was added or removed.</span></span> <span data-ttu-id="98f8b-140">只读。</span><span class="sxs-lookup"><span data-stu-id="98f8b-140">Read-Only.</span></span>|
|<span data-ttu-id="98f8b-141">requestStatus</span><span class="sxs-lookup"><span data-stu-id="98f8b-141">requestStatus</span></span>|<span data-ttu-id="98f8b-142">String</span><span class="sxs-lookup"><span data-stu-id="98f8b-142">String</span></span>|<span data-ttu-id="98f8b-143">只读。</span><span class="sxs-lookup"><span data-stu-id="98f8b-143">Read-only.</span></span>|
|<span data-ttu-id="98f8b-144">requestType</span><span class="sxs-lookup"><span data-stu-id="98f8b-144">requestType</span></span>|<span data-ttu-id="98f8b-145">String</span><span class="sxs-lookup"><span data-stu-id="98f8b-145">String</span></span>|<span data-ttu-id="98f8b-146">用于 `AdminAdd` 添加资源（如果调用方是管理员或资源所有者） `AdminRemove` 或删除资源。</span><span class="sxs-lookup"><span data-stu-id="98f8b-146">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner, or `AdminRemove` to remove a resource.</span></span> |

## <a name="relationships"></a><span data-ttu-id="98f8b-147">关系</span><span class="sxs-lookup"><span data-stu-id="98f8b-147">Relationships</span></span>

| <span data-ttu-id="98f8b-148">关系</span><span class="sxs-lookup"><span data-stu-id="98f8b-148">Relationship</span></span> | <span data-ttu-id="98f8b-149">类型</span><span class="sxs-lookup"><span data-stu-id="98f8b-149">Type</span></span>        | <span data-ttu-id="98f8b-150">说明</span><span class="sxs-lookup"><span data-stu-id="98f8b-150">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="98f8b-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="98f8b-151">accessPackageResource</span></span>|[<span data-ttu-id="98f8b-152">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="98f8b-152">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="98f8b-153">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="98f8b-153">Nullable.</span></span>|
|<span data-ttu-id="98f8b-154">requestor</span><span class="sxs-lookup"><span data-stu-id="98f8b-154">requestor</span></span>|[<span data-ttu-id="98f8b-155">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="98f8b-155">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="98f8b-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="98f8b-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98f8b-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98f8b-158">JSON representation</span></span>

<span data-ttu-id="98f8b-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98f8b-159">The following is a JSON representation of the resource.</span></span>

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


