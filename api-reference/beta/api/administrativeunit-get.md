---
title: 获取 administrativeUnit
description: 检索 administrativeUnit 对象的属性和关系。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d84abad95f0165d89adc0ea5cc8bae6e5c140eb7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997296"
---
# <a name="get-administrativeunit"></a><span data-ttu-id="ca03f-103">获取 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="ca03f-103">Get administrativeUnit</span></span>

<span data-ttu-id="ca03f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca03f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca03f-105">检索 [administrativeUnit](../resources/administrativeunit.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ca03f-105">Retrieve the properties and relationships of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="ca03f-106">由于 **administrativeUnit** 资源支持 [扩展](/graph/extensibility-overview)，因此您还可以使用此 `GET` 操作获取 **administrativeUnit** 实例中的自定义属性和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="ca03f-106">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in an **administrativeUnit** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca03f-107">权限</span><span class="sxs-lookup"><span data-stu-id="ca03f-107">Permissions</span></span>
<span data-ttu-id="ca03f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca03f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ca03f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca03f-110">Permission type</span></span>      | <span data-ttu-id="ca03f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca03f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca03f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca03f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca03f-113">AdministrativeUnit、AdministrativeUnit、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="ca03f-113">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca03f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca03f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca03f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca03f-115">Not supported.</span></span>    |
|<span data-ttu-id="ca03f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca03f-116">Application</span></span> | <span data-ttu-id="ca03f-117">AdministrativeUnit、AdministrativeUnit、all、all、all、All 和所有的</span><span class="sxs-lookup"><span data-stu-id="ca03f-117">AdministrativeUnit.Read.All, Directory.Read.All, AdministrativeUnit.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca03f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca03f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca03f-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ca03f-119">Optional query parameters</span></span>
<span data-ttu-id="ca03f-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ca03f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca03f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca03f-121">Request headers</span></span>
| <span data-ttu-id="ca03f-122">名称</span><span class="sxs-lookup"><span data-stu-id="ca03f-122">Name</span></span>      |<span data-ttu-id="ca03f-123">说明</span><span class="sxs-lookup"><span data-stu-id="ca03f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca03f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca03f-124">Authorization</span></span>  | <span data-ttu-id="ca03f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca03f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca03f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca03f-127">Request body</span></span>
<span data-ttu-id="ca03f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca03f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca03f-129">响应</span><span class="sxs-lookup"><span data-stu-id="ca03f-129">Response</span></span>

<span data-ttu-id="ca03f-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ca03f-130">If successful, this method returns a `200 OK` response code and [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca03f-131">示例</span><span class="sxs-lookup"><span data-stu-id="ca03f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca03f-132">请求</span><span class="sxs-lookup"><span data-stu-id="ca03f-132">Request</span></span>
<span data-ttu-id="ca03f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca03f-133">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ca03f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="ca03f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}
```
# <a name="c"></a>[<span data-ttu-id="ca03f-135">C#</span><span class="sxs-lookup"><span data-stu-id="ca03f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ca03f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ca03f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ca03f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ca03f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ca03f-138">响应</span><span class="sxs-lookup"><span data-stu-id="ca03f-138">Response</span></span>
<span data-ttu-id="ca03f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca03f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ca03f-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ca03f-142">See also</span></span>

- [<span data-ttu-id="ca03f-143">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="ca03f-143">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ca03f-144">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="ca03f-144">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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


