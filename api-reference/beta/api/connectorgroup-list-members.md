---
title: 列出成员
description: 检索与 connectorGroup 关联的连接器对象列表。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 540a08d9b5b586c00de0553285d17f38d1ba994d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129574"
---
# <a name="list-members"></a><span data-ttu-id="595da-103">列出成员</span><span class="sxs-lookup"><span data-stu-id="595da-103">List members</span></span>

<span data-ttu-id="595da-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="595da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="595da-105">检索与 [connectorGroup](../resources/connector.md) 关联的 [连接器对象的列表](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="595da-105">Retrieve a list of [connector](../resources/connector.md) objects associated with a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="595da-106">权限</span><span class="sxs-lookup"><span data-stu-id="595da-106">Permissions</span></span>
<span data-ttu-id="595da-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="595da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="595da-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="595da-109">Permission type</span></span>      | <span data-ttu-id="595da-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="595da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="595da-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="595da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="595da-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="595da-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="595da-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="595da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="595da-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="595da-114">Not supported.</span></span>    |
|<span data-ttu-id="595da-115">Application</span><span class="sxs-lookup"><span data-stu-id="595da-115">Application</span></span> | <span data-ttu-id="595da-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="595da-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="595da-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="595da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="595da-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="595da-118">Optional query parameters</span></span>
<span data-ttu-id="595da-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="595da-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="595da-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="595da-120">Request headers</span></span>
| <span data-ttu-id="595da-121">名称</span><span class="sxs-lookup"><span data-stu-id="595da-121">Name</span></span>      |<span data-ttu-id="595da-122">说明</span><span class="sxs-lookup"><span data-stu-id="595da-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="595da-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="595da-123">Authorization</span></span>  | <span data-ttu-id="595da-124">Bearer。</span><span class="sxs-lookup"><span data-stu-id="595da-124">Bearer.</span></span> <span data-ttu-id="595da-125">必需</span><span class="sxs-lookup"><span data-stu-id="595da-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="595da-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="595da-126">Request body</span></span>
<span data-ttu-id="595da-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="595da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="595da-128">响应</span><span class="sxs-lookup"><span data-stu-id="595da-128">Response</span></span>

<span data-ttu-id="595da-129">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [连接器](../resources/connector.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="595da-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="595da-130">示例</span><span class="sxs-lookup"><span data-stu-id="595da-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="595da-131">请求</span><span class="sxs-lookup"><span data-stu-id="595da-131">Request</span></span>
<span data-ttu-id="595da-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="595da-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="595da-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="595da-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="595da-134">C#</span><span class="sxs-lookup"><span data-stu-id="595da-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="595da-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="595da-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="595da-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="595da-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="595da-137">Java</span><span class="sxs-lookup"><span data-stu-id="595da-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroup-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="595da-138">响应</span><span class="sxs-lookup"><span data-stu-id="595da-138">Response</span></span>
<span data-ttu-id="595da-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="595da-139">The following is an example of the response.</span></span> <span data-ttu-id="595da-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="595da-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="595da-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="595da-141">All of the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

