---
title: 创建案例
description: 使用此 API 创建新案例。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 7fa7331b9a75c9c9d787ab12804540b1e5efe31a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52044723"
---
# <a name="create-case"></a><span data-ttu-id="8dadd-103">创建案例</span><span class="sxs-lookup"><span data-stu-id="8dadd-103">Create case</span></span>

<span data-ttu-id="8dadd-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="8dadd-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8dadd-105">创建新的 [case](../resources/ediscovery-case.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8dadd-105">Create a new [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dadd-106">权限</span><span class="sxs-lookup"><span data-stu-id="8dadd-106">Permissions</span></span>

<span data-ttu-id="8dadd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8dadd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8dadd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8dadd-109">Permission type</span></span>|<span data-ttu-id="8dadd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8dadd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8dadd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8dadd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8dadd-112">eDiscovery.Read.All、eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8dadd-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="8dadd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8dadd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8dadd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8dadd-114">Not supported.</span></span>|
|<span data-ttu-id="8dadd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8dadd-115">Application</span></span>|<span data-ttu-id="8dadd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8dadd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dadd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8dadd-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases
```

## <a name="request-headers"></a><span data-ttu-id="8dadd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8dadd-118">Request headers</span></span>

| <span data-ttu-id="8dadd-119">名称</span><span class="sxs-lookup"><span data-stu-id="8dadd-119">Name</span></span>          | <span data-ttu-id="8dadd-120">说明</span><span class="sxs-lookup"><span data-stu-id="8dadd-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8dadd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dadd-121">Authorization</span></span> | <span data-ttu-id="8dadd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8dadd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8dadd-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8dadd-124">Request body</span></span>

<span data-ttu-id="8dadd-125">在请求正文中，提供 case 对象的 JSON [表示](../resources/ediscovery-case.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="8dadd-125">In the request body, supply a JSON representation of a [case](../resources/ediscovery-case.md) object.</span></span> <span data-ttu-id="8dadd-126">下表列出了可以通过调用提交的属性。</span><span class="sxs-lookup"><span data-stu-id="8dadd-126">The following table lists properties that can be submitted with the call.</span></span>

| <span data-ttu-id="8dadd-127">属性</span><span class="sxs-lookup"><span data-stu-id="8dadd-127">Property</span></span>     | <span data-ttu-id="8dadd-128">类型</span><span class="sxs-lookup"><span data-stu-id="8dadd-128">Type</span></span>        | <span data-ttu-id="8dadd-129">说明</span><span class="sxs-lookup"><span data-stu-id="8dadd-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="8dadd-130">displayName</span><span class="sxs-lookup"><span data-stu-id="8dadd-130">displayName</span></span>  | <span data-ttu-id="8dadd-131">string</span><span class="sxs-lookup"><span data-stu-id="8dadd-131">string</span></span>      | <span data-ttu-id="8dadd-132">电子数据展示案例的名称。</span><span class="sxs-lookup"><span data-stu-id="8dadd-132">The name of the eDiscovery case.</span></span> |

## <a name="response"></a><span data-ttu-id="8dadd-133">响应</span><span class="sxs-lookup"><span data-stu-id="8dadd-133">Response</span></span>

<span data-ttu-id="8dadd-134">如果成功，此方法在响应正文中返回 响应代码和新的 `201 Created` [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8dadd-134">If successful, this method returns a `201 Created` response code and a new [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8dadd-135">示例</span><span class="sxs-lookup"><span data-stu-id="8dadd-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8dadd-136">请求</span><span class="sxs-lookup"><span data-stu-id="8dadd-136">Request</span></span>

<span data-ttu-id="8dadd-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8dadd-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8dadd-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="8dadd-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_case"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-type: application/json

{
    "displayName": "My Case 1",
}
```

# <a name="c"></a>[<span data-ttu-id="8dadd-139">C#</span><span class="sxs-lookup"><span data-stu-id="8dadd-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8dadd-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8dadd-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8dadd-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8dadd-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8dadd-142">Java</span><span class="sxs-lookup"><span data-stu-id="8dadd-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="8dadd-143">响应</span><span class="sxs-lookup"><span data-stu-id="8dadd-143">Response</span></span>

<span data-ttu-id="8dadd-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8dadd-144">The following is an example of the response.</span></span>

> <span data-ttu-id="8dadd-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8dadd-145">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
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
  "description": "Create case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
