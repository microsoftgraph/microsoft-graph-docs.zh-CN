---
title: 获取 administrativeUnit
description: 检索 administrativeUnit 对象的属性和关系。
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3429caeb6cc8aafeeb2201445be0e7a74d416010
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992000"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="ae5fd-103">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ae5fd-103">Get administrativeUnit</span></span>

<span data-ttu-id="ae5fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae5fd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae5fd-105">检索 [administrativeUnit 对象的属性和](../resources/administrativeunit.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="ae5fd-106">由于 **administrativeUnit** 资源 [支持扩展](/graph/extensibility-overview)，因此您还可以使用 操作获取 administrativeUnit 实例中的自定义属性 `GET` 和 **扩展** 数据。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-106">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae5fd-107">权限</span><span class="sxs-lookup"><span data-stu-id="ae5fd-107">Permissions</span></span>
<span data-ttu-id="ae5fd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ae5fd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ae5fd-110">Permission type</span></span>      | <span data-ttu-id="ae5fd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ae5fd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae5fd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ae5fd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ae5fd-113">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ae5fd-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ae5fd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ae5fd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae5fd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-115">Not supported.</span></span>    |
|<span data-ttu-id="ae5fd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ae5fd-116">Application</span></span> | <span data-ttu-id="ae5fd-117">AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae5fd-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae5fd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ae5fd-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ae5fd-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ae5fd-119">Optional query parameters</span></span>
<span data-ttu-id="ae5fd-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae5fd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ae5fd-121">Request headers</span></span>
| <span data-ttu-id="ae5fd-122">名称</span><span class="sxs-lookup"><span data-stu-id="ae5fd-122">Name</span></span>      |<span data-ttu-id="ae5fd-123">说明</span><span class="sxs-lookup"><span data-stu-id="ae5fd-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ae5fd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae5fd-124">Authorization</span></span>  | <span data-ttu-id="ae5fd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae5fd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ae5fd-127">Request body</span></span>
<span data-ttu-id="ae5fd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae5fd-129">响应</span><span class="sxs-lookup"><span data-stu-id="ae5fd-129">Response</span></span>

<span data-ttu-id="ae5fd-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-130">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ae5fd-131">示例</span><span class="sxs-lookup"><span data-stu-id="ae5fd-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ae5fd-132">请求</span><span class="sxs-lookup"><span data-stu-id="ae5fd-132">Request</span></span>
<span data-ttu-id="ae5fd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae5fd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae5fd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="ae5fd-135">C#</span><span class="sxs-lookup"><span data-stu-id="ae5fd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ae5fd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae5fd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae5fd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae5fd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ae5fd-138">Java</span><span class="sxs-lookup"><span data-stu-id="ae5fd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ae5fd-139">响应</span><span class="sxs-lookup"><span data-stu-id="ae5fd-139">Response</span></span>
<span data-ttu-id="ae5fd-p103">这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ae5fd-p103">Here is an example of the response. Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 134

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value",
  "id": "id-value"
}
```

## <a name="see-also"></a><span data-ttu-id="ae5fd-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ae5fd-142">See also</span></span>

- [<span data-ttu-id="ae5fd-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="ae5fd-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ae5fd-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="ae5fd-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
