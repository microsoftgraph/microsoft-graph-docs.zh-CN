---
title: 列出 administrativeUnits
description: 检索 administrativeUnit 对象的列表。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: db17faeb311ff1168bec42e84dfb6aeeb7684351
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438811"
---
# <a name="list-administrativeunits"></a><span data-ttu-id="ae77c-103">列出 administrativeUnits</span><span class="sxs-lookup"><span data-stu-id="ae77c-103">List administrativeUnits</span></span>

<span data-ttu-id="ae77c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae77c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae77c-105">检索 [administrativeUnit 对象](../resources/administrativeunit.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="ae77c-105">Retrieve a list of [administrativeUnit](../resources/administrativeunit.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="ae77c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ae77c-106">Permissions</span></span>
<span data-ttu-id="ae77c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae77c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae77c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae77c-109">Permission type</span></span>      | <span data-ttu-id="ae77c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae77c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae77c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae77c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ae77c-112">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae77c-112">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae77c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae77c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae77c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae77c-114">Not supported.</span></span>    |
|<span data-ttu-id="ae77c-115">Application</span><span class="sxs-lookup"><span data-stu-id="ae77c-115">Application</span></span> | <span data-ttu-id="ae77c-116">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae77c-116">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae77c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae77c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae77c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae77c-118">Optional query parameters</span></span>
<span data-ttu-id="ae77c-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae77c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae77c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae77c-120">Request headers</span></span>
| <span data-ttu-id="ae77c-121">名称</span><span class="sxs-lookup"><span data-stu-id="ae77c-121">Name</span></span>      |<span data-ttu-id="ae77c-122">说明</span><span class="sxs-lookup"><span data-stu-id="ae77c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae77c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae77c-123">Authorization</span></span>  | <span data-ttu-id="ae77c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae77c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae77c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae77c-126">Request body</span></span>
<span data-ttu-id="ae77c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae77c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae77c-128">响应</span><span class="sxs-lookup"><span data-stu-id="ae77c-128">Response</span></span>

<span data-ttu-id="ae77c-129">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 administrativeUnit](../resources/administrativeunit.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ae77c-129">If successful, this method returns a `200 OK` response code and collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae77c-130">示例</span><span class="sxs-lookup"><span data-stu-id="ae77c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae77c-131">请求</span><span class="sxs-lookup"><span data-stu-id="ae77c-131">Request</span></span>
<span data-ttu-id="ae77c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae77c-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae77c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae77c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunits"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits
```
# <a name="c"></a>[<span data-ttu-id="ae77c-134">C#</span><span class="sxs-lookup"><span data-stu-id="ae77c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae77c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae77c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae77c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae77c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae77c-137">Java</span><span class="sxs-lookup"><span data-stu-id="ae77c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ae77c-138">响应</span><span class="sxs-lookup"><span data-stu-id="ae77c-138">Response</span></span>
<span data-ttu-id="ae77c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ae77c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
  "value": [
    {
      "displayName": "displayName-value",
      "description": "description-value",
      "visibility": "visibility-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List administrativeUnits",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
