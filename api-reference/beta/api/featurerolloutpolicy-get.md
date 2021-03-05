---
title: 获取 featureRolloutPolicy
description: 检索 featurerolloutpolicy 对象的属性和关系。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d7f73b5c584f5862d272807876d6cd0d76ecc0ea
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471220"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="22cd7-103">获取 featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="22cd7-103">Get featureRolloutPolicy</span></span>

<span data-ttu-id="22cd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22cd7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22cd7-105">检索 [featureRolloutPolicy 对象的属性和](../resources/featurerolloutpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="22cd7-105">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="22cd7-106">权限</span><span class="sxs-lookup"><span data-stu-id="22cd7-106">Permissions</span></span>

<span data-ttu-id="22cd7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="22cd7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="22cd7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="22cd7-109">Permission type</span></span>                        | <span data-ttu-id="22cd7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="22cd7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="22cd7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="22cd7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="22cd7-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22cd7-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="22cd7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="22cd7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22cd7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="22cd7-114">Not supported.</span></span> |
| <span data-ttu-id="22cd7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="22cd7-115">Application</span></span>                            | <span data-ttu-id="22cd7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="22cd7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22cd7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="22cd7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="22cd7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="22cd7-118">Optional query parameters</span></span>

<span data-ttu-id="22cd7-119">此方法支持 `$select` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="22cd7-119">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="22cd7-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="22cd7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="22cd7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="22cd7-121">Request headers</span></span>

| <span data-ttu-id="22cd7-122">名称</span><span class="sxs-lookup"><span data-stu-id="22cd7-122">Name</span></span>      |<span data-ttu-id="22cd7-123">说明</span><span class="sxs-lookup"><span data-stu-id="22cd7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="22cd7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22cd7-124">Authorization</span></span> | <span data-ttu-id="22cd7-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="22cd7-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="22cd7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="22cd7-126">Request body</span></span>

<span data-ttu-id="22cd7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="22cd7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22cd7-128">响应</span><span class="sxs-lookup"><span data-stu-id="22cd7-128">Response</span></span>

<span data-ttu-id="22cd7-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` 请求 [的 featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="22cd7-129">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="22cd7-130">示例</span><span class="sxs-lookup"><span data-stu-id="22cd7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="22cd7-131">请求</span><span class="sxs-lookup"><span data-stu-id="22cd7-131">Request</span></span>

<span data-ttu-id="22cd7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="22cd7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22cd7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="22cd7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="22cd7-134">C#</span><span class="sxs-lookup"><span data-stu-id="22cd7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22cd7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22cd7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22cd7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22cd7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22cd7-137">Java</span><span class="sxs-lookup"><span data-stu-id="22cd7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22cd7-138">响应</span><span class="sxs-lookup"><span data-stu-id="22cd7-138">Response</span></span>

<span data-ttu-id="22cd7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22cd7-139">The following is an example of the response.</span></span>

> <span data-ttu-id="22cd7-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="22cd7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="request"></a><span data-ttu-id="22cd7-142">请求</span><span class="sxs-lookup"><span data-stu-id="22cd7-142">Request</span></span>

<span data-ttu-id="22cd7-143">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="22cd7-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="22cd7-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="22cd7-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="c"></a>[<span data-ttu-id="22cd7-145">C#</span><span class="sxs-lookup"><span data-stu-id="22cd7-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="22cd7-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="22cd7-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="22cd7-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="22cd7-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="22cd7-148">Java</span><span class="sxs-lookup"><span data-stu-id="22cd7-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-featurerolloutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="22cd7-149">响应</span><span class="sxs-lookup"><span data-stu-id="22cd7-149">Response</span></span>

<span data-ttu-id="22cd7-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="22cd7-150">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="22cd7-151">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="22cd7-151">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="22cd7-152">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="22cd7-152">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


