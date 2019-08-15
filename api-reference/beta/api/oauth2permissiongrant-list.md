---
title: List oauth2PermissionGrants
description: 检索 oauth2PermissionGrant 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: c10d57342ad68e27b1856e9daf169908165c94bc
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414677"
---
# <a name="list-oauth2permissiongrants"></a><span data-ttu-id="3059d-103">List oauth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="3059d-103">List oauth2PermissionGrants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3059d-104">检索 oauth2PermissionGrant 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="3059d-104">Retrieve a list of oauth2PermissionGrant objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="3059d-105">权限</span><span class="sxs-lookup"><span data-stu-id="3059d-105">Permissions</span></span>

<span data-ttu-id="3059d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3059d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3059d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3059d-108">Permission type</span></span>      | <span data-ttu-id="3059d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3059d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3059d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3059d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3059d-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3059d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3059d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3059d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3059d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3059d-113">Not supported.</span></span>    |
|<span data-ttu-id="3059d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3059d-114">Application</span></span> | <span data-ttu-id="3059d-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3059d-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3059d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3059d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oauth2PermissionGrants
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3059d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3059d-117">Optional query parameters</span></span>
<span data-ttu-id="3059d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3059d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3059d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3059d-119">Request headers</span></span>
| <span data-ttu-id="3059d-120">名称</span><span class="sxs-lookup"><span data-stu-id="3059d-120">Name</span></span> | <span data-ttu-id="3059d-121">说明</span><span class="sxs-lookup"><span data-stu-id="3059d-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="3059d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3059d-122">Authorization</span></span>  | <span data-ttu-id="3059d-123">string</span><span class="sxs-lookup"><span data-stu-id="3059d-123">string</span></span>  | <span data-ttu-id="3059d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3059d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3059d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3059d-126">Request body</span></span>
<span data-ttu-id="3059d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3059d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3059d-128">响应</span><span class="sxs-lookup"><span data-stu-id="3059d-128">Response</span></span>

<span data-ttu-id="3059d-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3059d-129">If successful, this method returns a `200 OK` response code and collection of [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3059d-130">示例</span><span class="sxs-lookup"><span data-stu-id="3059d-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3059d-131">请求</span><span class="sxs-lookup"><span data-stu-id="3059d-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3059d-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3059d-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_oauth2permissiongrants"
}-->
```http
GET https://graph.microsoft.com/beta/oauth2PermissionGrants
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3059d-133">C#</span><span class="sxs-lookup"><span data-stu-id="3059d-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-oauth2permissiongrants-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3059d-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3059d-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-oauth2permissiongrants-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3059d-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="3059d-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-oauth2permissiongrants-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3059d-136">响应</span><span class="sxs-lookup"><span data-stu-id="3059d-136">Response</span></span>

<span data-ttu-id="3059d-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3059d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 259

{
  "value": [
    {
      "clientId": "clientId-value",
      "consentType": "consentType-value",
      "expiryTime": "datetime-value",
      "id": "id-value",
      "principalId": "principalId-value",
      "resourceId": "resourceId-value",
      "scope": "scope-value",
      "startTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List oauth2PermissionGrants",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
