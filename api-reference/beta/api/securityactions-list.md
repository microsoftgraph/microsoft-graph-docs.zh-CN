---
title: 列出 securityActions
description: 检索 securityAction 对象的列表。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 02538a80ed8264b4e61bbeff57034d71a9cc011b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364136"
---
# <a name="list-securityactions"></a><span data-ttu-id="7caab-103">列出 securityActions</span><span class="sxs-lookup"><span data-stu-id="7caab-103">List securityActions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7caab-104">检索[securityAction](../resources/securityaction.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7caab-104">Retrieve a list of [securityAction](../resources/securityaction.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7caab-105">权限</span><span class="sxs-lookup"><span data-stu-id="7caab-105">Permissions</span></span>

<span data-ttu-id="7caab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7caab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7caab-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7caab-108">Permission type</span></span>                        | <span data-ttu-id="7caab-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7caab-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7caab-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7caab-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7caab-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="7caab-111">Not supported.</span></span> |
| <span data-ttu-id="7caab-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7caab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7caab-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7caab-113">Not supported.</span></span> |
| <span data-ttu-id="7caab-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7caab-114">Application</span></span>                            | <span data-ttu-id="7caab-115">SecurityActions、SecurityActions 和所有</span><span class="sxs-lookup"><span data-stu-id="7caab-115">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7caab-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7caab-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7caab-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7caab-117">Optional query parameters</span></span>

<span data-ttu-id="7caab-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7caab-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7caab-119">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7caab-119">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7caab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7caab-120">Request headers</span></span>

| <span data-ttu-id="7caab-121">名称</span><span class="sxs-lookup"><span data-stu-id="7caab-121">Name</span></span>      |<span data-ttu-id="7caab-122">说明</span><span class="sxs-lookup"><span data-stu-id="7caab-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7caab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7caab-123">Authorization</span></span> | <span data-ttu-id="7caab-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="7caab-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="7caab-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7caab-125">Request body</span></span>

<span data-ttu-id="7caab-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7caab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7caab-127">响应</span><span class="sxs-lookup"><span data-stu-id="7caab-127">Response</span></span>

<span data-ttu-id="7caab-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[securityAction](../resources/securityaction.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7caab-128">If successful, this method returns a `200 OK` response code and a collection of [securityAction](../resources/securityaction.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7caab-129">示例</span><span class="sxs-lookup"><span data-stu-id="7caab-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7caab-130">请求</span><span class="sxs-lookup"><span data-stu-id="7caab-130">Request</span></span>

<span data-ttu-id="7caab-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7caab-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7caab-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7caab-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityactions"
}-->

```http
GET https://graph.microsoft.com/beta/security/securityActions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7caab-133">C#</span><span class="sxs-lookup"><span data-stu-id="7caab-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityactions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7caab-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7caab-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityactions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7caab-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="7caab-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityactions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7caab-136">Java</span><span class="sxs-lookup"><span data-stu-id="7caab-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-securityactions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7caab-137">响应</span><span class="sxs-lookup"><span data-stu-id="7caab-137">Response</span></span>

<span data-ttu-id="7caab-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7caab-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="7caab-139">为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7caab-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7caab-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7caab-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "actionReason": "actionReason-value",
      "appId": "appId-value",
      "azureTenantId": "azureTenantId-value",
      "clientContext": "clientContext-value",
      "completedDateTime": "datetime-value",
      "createdDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List securityActions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
