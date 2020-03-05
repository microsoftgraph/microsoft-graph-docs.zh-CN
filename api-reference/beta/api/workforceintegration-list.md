---
title: 列出 workforceIntegrations
description: 检索 workforceIntegration 对象的列表。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7854a2bded54d8480e9423fb8e7e6d6548455430
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451278"
---
# <a name="list-workforceintegrations"></a><span data-ttu-id="4da23-103">列出 workforceIntegrations</span><span class="sxs-lookup"><span data-stu-id="4da23-103">List workforceIntegrations</span></span>

<span data-ttu-id="4da23-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4da23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4da23-105">检索[workforceIntegration](../resources/workforceintegration.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="4da23-105">Retrieve a list of [workforceIntegration](../resources/workforceintegration.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="4da23-106">权限</span><span class="sxs-lookup"><span data-stu-id="4da23-106">Permissions</span></span>

<span data-ttu-id="4da23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4da23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4da23-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4da23-109">Permission type</span></span>                        | <span data-ttu-id="4da23-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4da23-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4da23-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4da23-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="4da23-112">WorkforceIntegration、WorkforceIntegration 和所有</span><span class="sxs-lookup"><span data-stu-id="4da23-112">WorkforceIntegration.Read.All, WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="4da23-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4da23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4da23-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4da23-114">Not supported.</span></span> |
| <span data-ttu-id="4da23-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4da23-115">Application</span></span>                            | <span data-ttu-id="4da23-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4da23-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4da23-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4da23-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teamwork/workforceIntegrations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4da23-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4da23-118">Optional query parameters</span></span>

<span data-ttu-id="4da23-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4da23-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="4da23-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="4da23-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="4da23-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4da23-121">Request headers</span></span>

| <span data-ttu-id="4da23-122">名称</span><span class="sxs-lookup"><span data-stu-id="4da23-122">Name</span></span>      |<span data-ttu-id="4da23-123">说明</span><span class="sxs-lookup"><span data-stu-id="4da23-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4da23-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4da23-124">Authorization</span></span> | <span data-ttu-id="4da23-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4da23-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4da23-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4da23-127">Request body</span></span>

<span data-ttu-id="4da23-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4da23-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4da23-129">响应</span><span class="sxs-lookup"><span data-stu-id="4da23-129">Response</span></span>

<span data-ttu-id="4da23-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[workforceIntegration](../resources/workforceintegration.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4da23-130">If successful, this method returns a `200 OK` response code and a collection of [workforceIntegration](../resources/workforceintegration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4da23-131">示例</span><span class="sxs-lookup"><span data-stu-id="4da23-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4da23-132">请求</span><span class="sxs-lookup"><span data-stu-id="4da23-132">Request</span></span>

<span data-ttu-id="4da23-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4da23-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4da23-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="4da23-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_workforceintegrations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations
```
# <a name="c"></a>[<span data-ttu-id="4da23-135">C#</span><span class="sxs-lookup"><span data-stu-id="4da23-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-workforceintegrations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4da23-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4da23-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-workforceintegrations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4da23-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4da23-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-workforceintegrations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4da23-138">响应</span><span class="sxs-lookup"><span data-stu-id="4da23-138">Response</span></span>

<span data-ttu-id="4da23-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4da23-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4da23-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4da23-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "displayName": "displayName-value",
      "apiVersion": 99,
      "encryption": {
        "protocol": "protocol-value",
        "secret": "secret-value"
      },
      "isActive": true,
      "url": "url-value",
      "supports": "supports-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List workforceIntegrations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
