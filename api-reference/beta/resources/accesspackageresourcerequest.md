---
title: accessPackageResourceRequest 资源类型
description: 访问包资源请求是向目录添加资源的请求，以便可以在一个或多个目录的访问包中使用该资源的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c109c2c28a9c4c9248adfbad4c94c9c50268f28f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871782"
---
# <a name="accesspackageresourcerequest-resource-type"></a><span data-ttu-id="7447a-103">accessPackageResourceRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="7447a-103">accessPackageResourceRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7447a-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源请求是向目录添加资源的请求，以便可以在一个或多个目录的访问包中使用该资源的角色。</span><span class="sxs-lookup"><span data-stu-id="7447a-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package resource request is a request to a add a resource to a catalog so that the roles of the resource can be used in one or more of the catalog's access packages.</span></span>

## <a name="methods"></a><span data-ttu-id="7447a-105">方法</span><span class="sxs-lookup"><span data-stu-id="7447a-105">Methods</span></span>

| <span data-ttu-id="7447a-106">方法</span><span class="sxs-lookup"><span data-stu-id="7447a-106">Method</span></span>       | <span data-ttu-id="7447a-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="7447a-107">Return Type</span></span> | <span data-ttu-id="7447a-108">说明</span><span class="sxs-lookup"><span data-stu-id="7447a-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7447a-109">列出 accessPackageResourceRequests</span><span class="sxs-lookup"><span data-stu-id="7447a-109">List accessPackageResourceRequests</span></span>](../api/accesspackageresourcerequest-list.md) | <span data-ttu-id="7447a-110">[accessPackageResourceRequest](accesspackageresourcerequest.md)集合</span><span class="sxs-lookup"><span data-stu-id="7447a-110">[accessPackageResourceRequest](accesspackageresourcerequest.md) collection</span></span> | <span data-ttu-id="7447a-111">检索**accessPackageResourceRequest**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7447a-111">Retrieve a list of **accessPackageResourceRequest** objects.</span></span> |
| [<span data-ttu-id="7447a-112">创建 accessPackageResourceRequest</span><span class="sxs-lookup"><span data-stu-id="7447a-112">Create accessPackageResourceRequest</span></span>](../api/accesspackageresourcerequest-post.md) | [<span data-ttu-id="7447a-113">accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="7447a-113">accessPackageCatalog</span></span>](accesspackageresourcerequest.md) | <span data-ttu-id="7447a-114">创建新的**accessPackageResourceRequest**对象。</span><span class="sxs-lookup"><span data-stu-id="7447a-114">Create a new **accessPackageResourceRequest** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7447a-115">属性</span><span class="sxs-lookup"><span data-stu-id="7447a-115">Properties</span></span>

| <span data-ttu-id="7447a-116">属性</span><span class="sxs-lookup"><span data-stu-id="7447a-116">Property</span></span>     | <span data-ttu-id="7447a-117">类型</span><span class="sxs-lookup"><span data-stu-id="7447a-117">Type</span></span>        | <span data-ttu-id="7447a-118">说明</span><span class="sxs-lookup"><span data-stu-id="7447a-118">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7447a-119">catalogId</span><span class="sxs-lookup"><span data-stu-id="7447a-119">catalogId</span></span>|<span data-ttu-id="7447a-120">String</span><span class="sxs-lookup"><span data-stu-id="7447a-120">String</span></span>|<span data-ttu-id="7447a-121">访问包目录的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="7447a-121">The unique ID of the access package catalog.</span></span>|
|<span data-ttu-id="7447a-122">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7447a-122">expirationDateTime</span></span>|<span data-ttu-id="7447a-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7447a-123">DateTimeOffset</span></span>|<span data-ttu-id="7447a-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7447a-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7447a-126">id</span><span class="sxs-lookup"><span data-stu-id="7447a-126">id</span></span>|<span data-ttu-id="7447a-127">String</span><span class="sxs-lookup"><span data-stu-id="7447a-127">String</span></span>| <span data-ttu-id="7447a-128">只读。</span><span class="sxs-lookup"><span data-stu-id="7447a-128">Read-only.</span></span>|
|<span data-ttu-id="7447a-129">isValidationOnly</span><span class="sxs-lookup"><span data-stu-id="7447a-129">isValidationOnly</span></span>|<span data-ttu-id="7447a-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="7447a-130">Boolean</span></span>|<span data-ttu-id="7447a-131">如果设置，则不添加资源。</span><span class="sxs-lookup"><span data-stu-id="7447a-131">If set, does not add the resource.</span></span>|
|<span data-ttu-id="7447a-132">合理化</span><span class="sxs-lookup"><span data-stu-id="7447a-132">justification</span></span>|<span data-ttu-id="7447a-133">String</span><span class="sxs-lookup"><span data-stu-id="7447a-133">String</span></span>|<span data-ttu-id="7447a-134">请求者的添加资源的理由。</span><span class="sxs-lookup"><span data-stu-id="7447a-134">The requestor's justification for adding the resource.</span></span>|
|<span data-ttu-id="7447a-135">requestState</span><span class="sxs-lookup"><span data-stu-id="7447a-135">requestState</span></span>|<span data-ttu-id="7447a-136">String</span><span class="sxs-lookup"><span data-stu-id="7447a-136">String</span></span>| <span data-ttu-id="7447a-137">服务是否能够将资源添加到目录的结果。</span><span class="sxs-lookup"><span data-stu-id="7447a-137">The outcome of whether the service was able to add the resource to the catalog.</span></span>  <span data-ttu-id="7447a-138">值为`Delivered`是否添加了资源。</span><span class="sxs-lookup"><span data-stu-id="7447a-138">The value is `Delivered` if the resource was added.</span></span> <span data-ttu-id="7447a-139">只读。</span><span class="sxs-lookup"><span data-stu-id="7447a-139">Read-Only.</span></span>|
|<span data-ttu-id="7447a-140">requestStatus</span><span class="sxs-lookup"><span data-stu-id="7447a-140">requestStatus</span></span>|<span data-ttu-id="7447a-141">String</span><span class="sxs-lookup"><span data-stu-id="7447a-141">String</span></span>|<span data-ttu-id="7447a-142">只读。</span><span class="sxs-lookup"><span data-stu-id="7447a-142">Read-only.</span></span>|
|<span data-ttu-id="7447a-143">requestType</span><span class="sxs-lookup"><span data-stu-id="7447a-143">requestType</span></span>|<span data-ttu-id="7447a-144">String</span><span class="sxs-lookup"><span data-stu-id="7447a-144">String</span></span>|<span data-ttu-id="7447a-145">如果`AdminAdd`呼叫者是管理员或资源所有者，请使用添加资源。</span><span class="sxs-lookup"><span data-stu-id="7447a-145">Use `AdminAdd` to add a resource, if the caller is an administrator or resource owner.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7447a-146">关系</span><span class="sxs-lookup"><span data-stu-id="7447a-146">Relationships</span></span>

| <span data-ttu-id="7447a-147">关系</span><span class="sxs-lookup"><span data-stu-id="7447a-147">Relationship</span></span> | <span data-ttu-id="7447a-148">类型</span><span class="sxs-lookup"><span data-stu-id="7447a-148">Type</span></span>        | <span data-ttu-id="7447a-149">说明</span><span class="sxs-lookup"><span data-stu-id="7447a-149">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7447a-150">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="7447a-150">accessPackageResource</span></span>|[<span data-ttu-id="7447a-151">accessPackageResource</span><span class="sxs-lookup"><span data-stu-id="7447a-151">accessPackageResource</span></span>](accesspackageresource.md)| <span data-ttu-id="7447a-152">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="7447a-152">Nullable.</span></span>|
|<span data-ttu-id="7447a-153">请求程序</span><span class="sxs-lookup"><span data-stu-id="7447a-153">requestor</span></span>|[<span data-ttu-id="7447a-154">accessPackageSubject</span><span class="sxs-lookup"><span data-stu-id="7447a-154">accessPackageSubject</span></span>](accesspackagesubject.md)| <span data-ttu-id="7447a-p103">只读。可为空。</span><span class="sxs-lookup"><span data-stu-id="7447a-p103">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7447a-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7447a-157">JSON representation</span></span>

<span data-ttu-id="7447a-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7447a-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRequest",
  "baseType": "",
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
