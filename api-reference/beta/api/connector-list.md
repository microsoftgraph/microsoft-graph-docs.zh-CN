---
title: List connectors
description: 检索连接器对象的列表。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ae953bea60b81c2d74dbb1f4df61046f5152aa7f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047201"
---
# <a name="list-connectors"></a><span data-ttu-id="b3139-103">List connectors</span><span class="sxs-lookup"><span data-stu-id="b3139-103">List connectors</span></span>

<span data-ttu-id="b3139-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3139-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3139-105">检索连接器 [对象](../resources/connector.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="b3139-105">Retrieve a list of [connector](../resources/connector.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3139-106">权限</span><span class="sxs-lookup"><span data-stu-id="b3139-106">Permissions</span></span>
<span data-ttu-id="b3139-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3139-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3139-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3139-109">Permission type</span></span>      | <span data-ttu-id="b3139-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3139-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3139-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3139-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b3139-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b3139-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b3139-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3139-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3139-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3139-114">Not supported.</span></span>    |
|<span data-ttu-id="b3139-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3139-115">Application</span></span> | <span data-ttu-id="b3139-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3139-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3139-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3139-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b3139-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b3139-118">Optional query parameters</span></span>
<span data-ttu-id="b3139-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b3139-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b3139-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3139-120">Request headers</span></span>
| <span data-ttu-id="b3139-121">名称</span><span class="sxs-lookup"><span data-stu-id="b3139-121">Name</span></span>      |<span data-ttu-id="b3139-122">说明</span><span class="sxs-lookup"><span data-stu-id="b3139-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b3139-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3139-123">Authorization</span></span>  | <span data-ttu-id="b3139-124">Bearer。</span><span class="sxs-lookup"><span data-stu-id="b3139-124">Bearer.</span></span> <span data-ttu-id="b3139-125">必需</span><span class="sxs-lookup"><span data-stu-id="b3139-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3139-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3139-126">Request body</span></span>
<span data-ttu-id="b3139-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3139-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3139-128">响应</span><span class="sxs-lookup"><span data-stu-id="b3139-128">Response</span></span>

<span data-ttu-id="b3139-129">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/connector.md) 代码和 connector 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b3139-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3139-130">示例</span><span class="sxs-lookup"><span data-stu-id="b3139-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b3139-131">请求</span><span class="sxs-lookup"><span data-stu-id="b3139-131">Request</span></span>
<span data-ttu-id="b3139-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b3139-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b3139-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="b3139-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors
```
# <a name="c"></a>[<span data-ttu-id="b3139-134">C#</span><span class="sxs-lookup"><span data-stu-id="b3139-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b3139-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b3139-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b3139-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b3139-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b3139-137">Java</span><span class="sxs-lookup"><span data-stu-id="b3139-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b3139-138">响应</span><span class="sxs-lookup"><span data-stu-id="b3139-138">Response</span></span>
<span data-ttu-id="b3139-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b3139-139">The following is an example of the response.</span></span> <span data-ttu-id="b3139-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b3139-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

