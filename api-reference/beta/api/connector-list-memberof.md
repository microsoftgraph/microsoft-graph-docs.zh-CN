---
title: 列出 memberOf
description: 检索连接器所属的 connectorgroup。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0127cbff360f0b4b08d43eccaabe26a5d4e31c6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957491"
---
# <a name="list-memberof"></a><span data-ttu-id="9a951-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="9a951-103">List memberOf</span></span>

<span data-ttu-id="9a951-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a951-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a951-105">检索[连接器](../resources/connector.md)所属的[connectorGroup](../resources/connectorgroup.md) 。</span><span class="sxs-lookup"><span data-stu-id="9a951-105">Retrieve the [connectorGroup](../resources/connectorgroup.md) the [connector](../resources/connector.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a951-106">权限</span><span class="sxs-lookup"><span data-stu-id="9a951-106">Permissions</span></span>
<span data-ttu-id="9a951-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a951-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a951-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a951-109">Permission type</span></span>      | <span data-ttu-id="9a951-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9a951-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a951-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a951-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9a951-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9a951-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9a951-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a951-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a951-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a951-114">Not supported.</span></span>    |
|<span data-ttu-id="9a951-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a951-115">Application</span></span> | <span data-ttu-id="9a951-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a951-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9a951-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a951-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a951-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9a951-118">Optional query parameters</span></span>
<span data-ttu-id="9a951-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9a951-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a951-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a951-120">Request headers</span></span>
| <span data-ttu-id="9a951-121">名称</span><span class="sxs-lookup"><span data-stu-id="9a951-121">Name</span></span>      |<span data-ttu-id="9a951-122">说明</span><span class="sxs-lookup"><span data-stu-id="9a951-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9a951-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a951-123">Authorization</span></span>  | <span data-ttu-id="9a951-124">负载.</span><span class="sxs-lookup"><span data-stu-id="9a951-124">Bearer.</span></span> <span data-ttu-id="9a951-125">必需</span><span class="sxs-lookup"><span data-stu-id="9a951-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a951-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a951-126">Request body</span></span>
<span data-ttu-id="9a951-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9a951-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a951-128">响应</span><span class="sxs-lookup"><span data-stu-id="9a951-128">Response</span></span>

<span data-ttu-id="9a951-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [connectorGroup](../resources/connectorgroup.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9a951-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a951-130">示例</span><span class="sxs-lookup"><span data-stu-id="9a951-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a951-131">请求</span><span class="sxs-lookup"><span data-stu-id="9a951-131">Request</span></span>
<span data-ttu-id="9a951-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9a951-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9a951-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a951-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="9a951-134">C#</span><span class="sxs-lookup"><span data-stu-id="9a951-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9a951-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a951-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9a951-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a951-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9a951-137">Java</span><span class="sxs-lookup"><span data-stu-id="9a951-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/connector-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9a951-138">响应</span><span class="sxs-lookup"><span data-stu-id="9a951-138">Response</span></span>
<span data-ttu-id="9a951-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9a951-139">The following is an example of the response.</span></span> <span data-ttu-id="9a951-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9a951-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9a951-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a951-141">All of the properties will be returned from an actual call.</span></span>
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
