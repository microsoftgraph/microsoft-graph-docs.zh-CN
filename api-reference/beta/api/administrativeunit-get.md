---
title: 获取 administrativeUnit
description: 检索 administrativeUnit 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a583e7d826e1fb57a11c0a11fc899360ea64252d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855783"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="bebed-103">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="bebed-103">Get administrativeUnit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bebed-104">检索[administrativeUnit](../resources/administrativeunit.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bebed-104">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="bebed-105">由于**administrativeUnit**资源支持[扩展](/graph/extensibility-overview), 因此您还可以使用此`GET`操作获取**administrativeUnit**实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="bebed-105">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="bebed-106">权限</span><span class="sxs-lookup"><span data-stu-id="bebed-106">Permissions</span></span>
<span data-ttu-id="bebed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bebed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bebed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bebed-109">Permission type</span></span>      | <span data-ttu-id="bebed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bebed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bebed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bebed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bebed-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bebed-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bebed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bebed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bebed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bebed-114">Not supported.</span></span>    |
|<span data-ttu-id="bebed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bebed-115">Application</span></span> | <span data-ttu-id="bebed-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bebed-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bebed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bebed-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bebed-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bebed-118">Optional query parameters</span></span>
<span data-ttu-id="bebed-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bebed-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bebed-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bebed-120">Request headers</span></span>
| <span data-ttu-id="bebed-121">名称</span><span class="sxs-lookup"><span data-stu-id="bebed-121">Name</span></span>      |<span data-ttu-id="bebed-122">说明</span><span class="sxs-lookup"><span data-stu-id="bebed-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bebed-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bebed-123">Authorization</span></span>  | <span data-ttu-id="bebed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bebed-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bebed-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bebed-126">Request body</span></span>
<span data-ttu-id="bebed-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bebed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bebed-128">响应</span><span class="sxs-lookup"><span data-stu-id="bebed-128">Response</span></span>

<span data-ttu-id="bebed-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[administrativeUnit](../resources/administrativeunit.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bebed-129">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bebed-130">示例</span><span class="sxs-lookup"><span data-stu-id="bebed-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bebed-131">请求</span><span class="sxs-lookup"><span data-stu-id="bebed-131">Request</span></span>
<span data-ttu-id="bebed-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bebed-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bebed-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bebed-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bebed-134">C#</span><span class="sxs-lookup"><span data-stu-id="bebed-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bebed-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="bebed-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bebed-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="bebed-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bebed-137">Java</span><span class="sxs-lookup"><span data-stu-id="bebed-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bebed-138">响应</span><span class="sxs-lookup"><span data-stu-id="bebed-138">Response</span></span>
<span data-ttu-id="bebed-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bebed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="bebed-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bebed-142">See also</span></span>

- [<span data-ttu-id="bebed-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="bebed-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="bebed-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="bebed-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
