---
title: 获取 continuousAccessEvaluationPolicy
description: 读取 continuousAccessEvaluationPolicy 对象的属性。
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8dcafa080167facb1a692af8634fb6d1f4f345b5
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872651"
---
# <a name="get-continuousaccessevaluationpolicy"></a><span data-ttu-id="368f0-103">获取 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="368f0-103">Get continuousAccessEvaluationPolicy</span></span>
<span data-ttu-id="368f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="368f0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="368f0-105">读取 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="368f0-105">Read the properties and relationships of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="368f0-106">权限</span><span class="sxs-lookup"><span data-stu-id="368f0-106">Permissions</span></span>
<span data-ttu-id="368f0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="368f0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="368f0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="368f0-109">Permission type</span></span>|<span data-ttu-id="368f0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="368f0-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="368f0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="368f0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="368f0-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="368f0-112">Policy.Read.All</span></span> |
|<span data-ttu-id="368f0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="368f0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="368f0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="368f0-114">Not supported.</span></span> |
|<span data-ttu-id="368f0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="368f0-115">Application</span></span>                            | <span data-ttu-id="368f0-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="368f0-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="368f0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="368f0-117">HTTP request</span></span>

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="368f0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="368f0-118">Optional query parameters</span></span>
<span data-ttu-id="368f0-119">此方法支持"$select"OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="368f0-119">This method supports the '$select' OData query parameter to help customize the response.</span></span> <span data-ttu-id="368f0-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="368f0-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="368f0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="368f0-121">Request headers</span></span>
|<span data-ttu-id="368f0-122">名称</span><span class="sxs-lookup"><span data-stu-id="368f0-122">Name</span></span>|<span data-ttu-id="368f0-123">说明</span><span class="sxs-lookup"><span data-stu-id="368f0-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="368f0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="368f0-124">Authorization</span></span>|<span data-ttu-id="368f0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="368f0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="368f0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="368f0-127">Request body</span></span>
<span data-ttu-id="368f0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="368f0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="368f0-129">响应</span><span class="sxs-lookup"><span data-stu-id="368f0-129">Response</span></span>

<span data-ttu-id="368f0-130">如果成功，此方法在响应正文中返回响应代码和连续 `200 OK` [AccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="368f0-130">If successful, this method returns a `200 OK` response code and a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="368f0-131">示例</span><span class="sxs-lookup"><span data-stu-id="368f0-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="368f0-132">请求</span><span class="sxs-lookup"><span data-stu-id="368f0-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="368f0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="368f0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```
# <a name="c"></a>[<span data-ttu-id="368f0-134">C#</span><span class="sxs-lookup"><span data-stu-id="368f0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-continuousaccessevaluationpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="368f0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="368f0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-continuousaccessevaluationpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="368f0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="368f0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-continuousaccessevaluationpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="368f0-137">Java</span><span class="sxs-lookup"><span data-stu-id="368f0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-continuousaccessevaluationpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="368f0-138">响应</span><span class="sxs-lookup"><span data-stu-id="368f0-138">Response</span></span>

<span data-ttu-id="368f0-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="368f0-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
