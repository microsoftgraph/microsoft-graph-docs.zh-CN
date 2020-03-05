---
title: 获取 oAuth2Permissiongrant
description: 检索 oAuth2Permissiongrant 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: e81d81182d40940c900c4855aa7eebb018aea54d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456661"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="8bb75-103">获取 oAuth2Permissiongrant</span><span class="sxs-lookup"><span data-stu-id="8bb75-103">Get oAuth2Permissiongrant</span></span>

<span data-ttu-id="8bb75-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8bb75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bb75-105">检索 oAuth2Permissiongrant 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8bb75-105">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bb75-106">权限</span><span class="sxs-lookup"><span data-stu-id="8bb75-106">Permissions</span></span>
<span data-ttu-id="8bb75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bb75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8bb75-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bb75-109">Permission type</span></span>      | <span data-ttu-id="8bb75-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bb75-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bb75-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bb75-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8bb75-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8bb75-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8bb75-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bb75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bb75-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bb75-114">Not supported.</span></span>    |
|<span data-ttu-id="8bb75-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bb75-115">Application</span></span> | <span data-ttu-id="8bb75-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bb75-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bb75-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bb75-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8bb75-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8bb75-118">Optional query parameters</span></span>
<span data-ttu-id="8bb75-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8bb75-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bb75-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bb75-120">Request headers</span></span>
| <span data-ttu-id="8bb75-121">名称</span><span class="sxs-lookup"><span data-stu-id="8bb75-121">Name</span></span>       | <span data-ttu-id="8bb75-122">类型</span><span class="sxs-lookup"><span data-stu-id="8bb75-122">Type</span></span> | <span data-ttu-id="8bb75-123">说明</span><span class="sxs-lookup"><span data-stu-id="8bb75-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8bb75-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bb75-124">Authorization</span></span>  | <span data-ttu-id="8bb75-125">string</span><span class="sxs-lookup"><span data-stu-id="8bb75-125">string</span></span>  | <span data-ttu-id="8bb75-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bb75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bb75-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bb75-128">Request body</span></span>
<span data-ttu-id="8bb75-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8bb75-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bb75-130">响应</span><span class="sxs-lookup"><span data-stu-id="8bb75-130">Response</span></span>

<span data-ttu-id="8bb75-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[oAuth2Permissiongrant](../resources/oauth2permissiongrant.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8bb75-131">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8bb75-132">示例</span><span class="sxs-lookup"><span data-stu-id="8bb75-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8bb75-133">请求</span><span class="sxs-lookup"><span data-stu-id="8bb75-133">Request</span></span>
<span data-ttu-id="8bb75-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8bb75-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8bb75-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="8bb75-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
# <a name="c"></a>[<span data-ttu-id="8bb75-136">C#</span><span class="sxs-lookup"><span data-stu-id="8bb75-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8bb75-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8bb75-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8bb75-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8bb75-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8bb75-139">响应</span><span class="sxs-lookup"><span data-stu-id="8bb75-139">Response</span></span>
<span data-ttu-id="8bb75-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8bb75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
