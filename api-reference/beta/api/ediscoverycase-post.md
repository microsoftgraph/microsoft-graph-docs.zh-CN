---
title: 创建 ediscoveryCase
description: 使用此 API 创建新的 ediscoveryCase。
localization_priority: Normal
author: mahage-msft
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 2e6502555263c9f42e2558cde88fd73d8398694f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966711"
---
# <a name="create-ediscoverycase"></a><span data-ttu-id="61685-103">创建 ediscoveryCase</span><span class="sxs-lookup"><span data-stu-id="61685-103">Create ediscoveryCase</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61685-104">创建新的 [ediscoveryCase](../resources/ediscoverycase.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61685-104">Create a new [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="61685-105">权限</span><span class="sxs-lookup"><span data-stu-id="61685-105">Permissions</span></span>

<span data-ttu-id="61685-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="61685-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="61685-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="61685-108">Permission type</span></span>                        | <span data-ttu-id="61685-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="61685-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="61685-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="61685-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="61685-111">User.Read</span><span class="sxs-lookup"><span data-stu-id="61685-111">User.Read</span></span>      |
| <span data-ttu-id="61685-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="61685-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="61685-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="61685-113">Not supported.</span></span> |
| <span data-ttu-id="61685-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="61685-114">Application</span></span>                            | <span data-ttu-id="61685-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="61685-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="61685-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="61685-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases
```

## <a name="request-headers"></a><span data-ttu-id="61685-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="61685-117">Request headers</span></span>

| <span data-ttu-id="61685-118">名称</span><span class="sxs-lookup"><span data-stu-id="61685-118">Name</span></span>          | <span data-ttu-id="61685-119">说明</span><span class="sxs-lookup"><span data-stu-id="61685-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="61685-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="61685-120">Authorization</span></span> | <span data-ttu-id="61685-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="61685-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="61685-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="61685-123">Request body</span></span>

<span data-ttu-id="61685-124">在请求正文中，提供 [ediscoveryCase](../resources/ediscoverycase.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61685-124">In the request body, supply a JSON representation of an [ediscoveryCase](../resources/ediscoverycase.md) object.</span></span> <span data-ttu-id="61685-125">下表列出了可以通过调用提交的属性。</span><span class="sxs-lookup"><span data-stu-id="61685-125">The following table lists properties that can be submitted with the call.</span></span>

| <span data-ttu-id="61685-126">属性</span><span class="sxs-lookup"><span data-stu-id="61685-126">Property</span></span>     | <span data-ttu-id="61685-127">类型</span><span class="sxs-lookup"><span data-stu-id="61685-127">Type</span></span>        | <span data-ttu-id="61685-128">说明</span><span class="sxs-lookup"><span data-stu-id="61685-128">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="61685-129">displayName</span><span class="sxs-lookup"><span data-stu-id="61685-129">displayName</span></span>  | <span data-ttu-id="61685-130">string</span><span class="sxs-lookup"><span data-stu-id="61685-130">string</span></span>      | <span data-ttu-id="61685-131">电子数据展示事例的名称。</span><span class="sxs-lookup"><span data-stu-id="61685-131">The name of the eDiscovery case.</span></span> |

## <a name="response"></a><span data-ttu-id="61685-132">响应</span><span class="sxs-lookup"><span data-stu-id="61685-132">Response</span></span>

<span data-ttu-id="61685-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和新的 [ediscoveryCase](../resources/ediscoverycase.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="61685-133">If successful, this method returns a `201 Created` response code and a new [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61685-134">示例</span><span class="sxs-lookup"><span data-stu-id="61685-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61685-135">请求</span><span class="sxs-lookup"><span data-stu-id="61685-135">Request</span></span>

<span data-ttu-id="61685-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="61685-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="61685-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="61685-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_ediscoverycase"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-type: application/json

{
    "displayName": "My Case 1",
}
```
# <a name="c"></a>[<span data-ttu-id="61685-138">C#</span><span class="sxs-lookup"><span data-stu-id="61685-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-ediscoverycase-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="61685-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="61685-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-ediscoverycase-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="61685-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="61685-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-ediscoverycase-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="61685-141">Java</span><span class="sxs-lookup"><span data-stu-id="61685-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-ediscoverycase-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="61685-142">响应</span><span class="sxs-lookup"><span data-stu-id="61685-142">Response</span></span>

<span data-ttu-id="61685-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="61685-143">The following is an example of the response.</span></span>

> <span data-ttu-id="61685-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="61685-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases/$entity",
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ediscoveryCase",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


