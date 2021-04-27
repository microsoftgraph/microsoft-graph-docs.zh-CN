---
title: 列出 memberOf
description: 检索连接器是该连接器的一个成员的连接器组。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 4a069e0e501d1916b310daa390a2b2af0de5318f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047214"
---
# <a name="list-memberof"></a><span data-ttu-id="9bcb6-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="9bcb6-103">List memberOf</span></span>

<span data-ttu-id="9bcb6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bcb6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bcb6-105">检索[连接器是](../resources/connectorgroup.md)[该连接器](../resources/connector.md)的成员组。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-105">Retrieve the [connectorGroup](../resources/connectorgroup.md) the [connector](../resources/connector.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="9bcb6-106">权限</span><span class="sxs-lookup"><span data-stu-id="9bcb6-106">Permissions</span></span>
<span data-ttu-id="9bcb6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9bcb6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9bcb6-109">Permission type</span></span>      | <span data-ttu-id="9bcb6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9bcb6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9bcb6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9bcb6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9bcb6-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9bcb6-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9bcb6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9bcb6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9bcb6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-114">Not supported.</span></span>    |
|<span data-ttu-id="9bcb6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9bcb6-115">Application</span></span> | <span data-ttu-id="9bcb6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9bcb6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9bcb6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9bcb6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9bcb6-118">Optional query parameters</span></span>
<span data-ttu-id="9bcb6-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9bcb6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9bcb6-120">Request headers</span></span>
| <span data-ttu-id="9bcb6-121">名称</span><span class="sxs-lookup"><span data-stu-id="9bcb6-121">Name</span></span>      |<span data-ttu-id="9bcb6-122">说明</span><span class="sxs-lookup"><span data-stu-id="9bcb6-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9bcb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bcb6-123">Authorization</span></span>  | <span data-ttu-id="9bcb6-124">Bearer。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-124">Bearer.</span></span> <span data-ttu-id="9bcb6-125">必需</span><span class="sxs-lookup"><span data-stu-id="9bcb6-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bcb6-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9bcb6-126">Request body</span></span>
<span data-ttu-id="9bcb6-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9bcb6-128">响应</span><span class="sxs-lookup"><span data-stu-id="9bcb6-128">Response</span></span>

<span data-ttu-id="9bcb6-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [connectorGroup](../resources/connectorgroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9bcb6-130">示例</span><span class="sxs-lookup"><span data-stu-id="9bcb6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9bcb6-131">请求</span><span class="sxs-lookup"><span data-stu-id="9bcb6-131">Request</span></span>
<span data-ttu-id="9bcb6-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9bcb6-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9bcb6-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="9bcb6-134">C#</span><span class="sxs-lookup"><span data-stu-id="9bcb6-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9bcb6-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9bcb6-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9bcb6-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9bcb6-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9bcb6-137">Java</span><span class="sxs-lookup"><span data-stu-id="9bcb6-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/connector-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9bcb6-138">响应</span><span class="sxs-lookup"><span data-stu-id="9bcb6-138">Response</span></span>
<span data-ttu-id="9bcb6-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-139">The following is an example of the response.</span></span> <span data-ttu-id="9bcb6-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9bcb6-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": false,
      "region": "region-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

