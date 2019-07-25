---
title: 获取应用程序
description: 检索应用程序对象的属性和关系。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8faa031b06a06fdf0ccd65d36f10925e98a7baf6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855279"
---
# <a name="get-application"></a><span data-ttu-id="6a430-103">获取应用程序</span><span class="sxs-lookup"><span data-stu-id="6a430-103">Get application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a430-104">检索应用程序对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6a430-104">Retrieve the properties and relationships of application object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a430-105">权限</span><span class="sxs-lookup"><span data-stu-id="6a430-105">Permissions</span></span>
<span data-ttu-id="6a430-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a430-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a430-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a430-108">Permission type</span></span>      | <span data-ttu-id="6a430-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a430-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a430-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a430-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6a430-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a430-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a430-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a430-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a430-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a430-113">Not supported.</span></span>    |
|<span data-ttu-id="6a430-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a430-114">Application</span></span> | <span data-ttu-id="6a430-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6a430-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a430-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a430-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a430-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6a430-117">Optional query parameters</span></span>
<span data-ttu-id="6a430-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6a430-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a430-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a430-119">Request headers</span></span>
| <span data-ttu-id="6a430-120">名称</span><span class="sxs-lookup"><span data-stu-id="6a430-120">Name</span></span>       | <span data-ttu-id="6a430-121">类型</span><span class="sxs-lookup"><span data-stu-id="6a430-121">Type</span></span> | <span data-ttu-id="6a430-122">说明</span><span class="sxs-lookup"><span data-stu-id="6a430-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6a430-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a430-123">Authorization</span></span>  | <span data-ttu-id="6a430-124">string</span><span class="sxs-lookup"><span data-stu-id="6a430-124">string</span></span>  | <span data-ttu-id="6a430-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a430-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a430-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a430-127">Request body</span></span>
<span data-ttu-id="6a430-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a430-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a430-129">响应</span><span class="sxs-lookup"><span data-stu-id="6a430-129">Response</span></span>

<span data-ttu-id="6a430-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a430-130">If successful, this method returns a `200 OK` response code and [application](../resources/application.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6a430-131">示例</span><span class="sxs-lookup"><span data-stu-id="6a430-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a430-132">请求</span><span class="sxs-lookup"><span data-stu-id="6a430-132">Request</span></span>
<span data-ttu-id="6a430-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a430-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a430-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a430-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a430-135">C#</span><span class="sxs-lookup"><span data-stu-id="6a430-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a430-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a430-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a430-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6a430-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6a430-138">Java</span><span class="sxs-lookup"><span data-stu-id="6a430-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6a430-139">响应</span><span class="sxs-lookup"><span data-stu-id="6a430-139">Response</span></span>
<span data-ttu-id="6a430-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a430-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
  "api": {
    "acceptedAccessTokenVersion": 1,
    "publishedPermissionScopes": [
      {
        "adminConsentDescription": "adminConsentDescription-value",
        "adminConsentDisplayName": "adminConsentDisplayName-value",
        "id": "id-value",
        "isEnabled": true,
        "type": "type-value",
        "userConsentDescription": "userConsentDescription-value",
        "userConsentDisplayName": "userConsentDisplayName-value",
        "value": "value-value"
      }
    ]
  },
  "allowPublicClient": true,
  "applicationAliases": [
    "applicationAliases-value"
  ],
  "createdDateTime": "datetime-value",
  "installedClients": {
    "redirectUrls": [
      "redirectUrls-value"
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
