---
title: Get connector
description: 检索连接器对象的属性。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 84d3d5d3b2ae8375304844e5d88315896722d110
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130092"
---
# <a name="get-connector"></a><span data-ttu-id="3699e-103">Get connector</span><span class="sxs-lookup"><span data-stu-id="3699e-103">Get connector</span></span>

<span data-ttu-id="3699e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3699e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3699e-105">检索连接器 [对象的属性和](../resources/connector.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3699e-105">Retrieve the properties and relationships of a [connector](../resources/connector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3699e-106">权限</span><span class="sxs-lookup"><span data-stu-id="3699e-106">Permissions</span></span>
<span data-ttu-id="3699e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3699e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3699e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3699e-109">Permission type</span></span>      | <span data-ttu-id="3699e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3699e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3699e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3699e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3699e-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3699e-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3699e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3699e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3699e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3699e-114">Not supported.</span></span>    |
|<span data-ttu-id="3699e-115">Application</span><span class="sxs-lookup"><span data-stu-id="3699e-115">Application</span></span> | <span data-ttu-id="3699e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3699e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3699e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3699e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3699e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3699e-118">Optional query parameters</span></span>
<span data-ttu-id="3699e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3699e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3699e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3699e-120">Request headers</span></span>
| <span data-ttu-id="3699e-121">名称</span><span class="sxs-lookup"><span data-stu-id="3699e-121">Name</span></span>      |<span data-ttu-id="3699e-122">说明</span><span class="sxs-lookup"><span data-stu-id="3699e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3699e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3699e-123">Authorization</span></span>  | <span data-ttu-id="3699e-124">Bearer。</span><span class="sxs-lookup"><span data-stu-id="3699e-124">Bearer.</span></span> <span data-ttu-id="3699e-125">必需</span><span class="sxs-lookup"><span data-stu-id="3699e-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3699e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3699e-126">Request body</span></span>
<span data-ttu-id="3699e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3699e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3699e-128">响应</span><span class="sxs-lookup"><span data-stu-id="3699e-128">Response</span></span>

<span data-ttu-id="3699e-129">如果成功，此方法在响应 `200 OK` 正文中返回响应[](../resources/connector.md)代码和连接器对象。</span><span class="sxs-lookup"><span data-stu-id="3699e-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3699e-130">示例</span><span class="sxs-lookup"><span data-stu-id="3699e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3699e-131">请求</span><span class="sxs-lookup"><span data-stu-id="3699e-131">Request</span></span>

<span data-ttu-id="3699e-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3699e-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3699e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3699e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="3699e-134">C#</span><span class="sxs-lookup"><span data-stu-id="3699e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3699e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3699e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3699e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3699e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3699e-137">Java</span><span class="sxs-lookup"><span data-stu-id="3699e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3699e-138">响应</span><span class="sxs-lookup"><span data-stu-id="3699e-138">Response</span></span>
<span data-ttu-id="3699e-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3699e-139">The following is an example of the response.</span></span> <span data-ttu-id="3699e-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3699e-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3699e-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3699e-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

