---
title: 列出应用程序
description: 检索该组织中应用程序的列表。
author: davidmu1
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e62ae878610fb1bcfd638c7d853bb2cb5195879
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318717"
---
# <a name="list-applications"></a><span data-ttu-id="59acb-103">列出应用程序</span><span class="sxs-lookup"><span data-stu-id="59acb-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59acb-104">检索该组织中应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="59acb-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="59acb-105">权限</span><span class="sxs-lookup"><span data-stu-id="59acb-105">Permissions</span></span>
<span data-ttu-id="59acb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59acb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="59acb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="59acb-108">Permission type</span></span>      | <span data-ttu-id="59acb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59acb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59acb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59acb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59acb-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59acb-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="59acb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59acb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59acb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="59acb-113">Not supported.</span></span>    |
|<span data-ttu-id="59acb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="59acb-114">Application</span></span> | <span data-ttu-id="59acb-115">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="59acb-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59acb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59acb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59acb-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59acb-117">Optional query parameters</span></span>
<span data-ttu-id="59acb-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59acb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59acb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59acb-119">Request headers</span></span>
| <span data-ttu-id="59acb-120">名称</span><span class="sxs-lookup"><span data-stu-id="59acb-120">Name</span></span>       | <span data-ttu-id="59acb-121">类型</span><span class="sxs-lookup"><span data-stu-id="59acb-121">Type</span></span> | <span data-ttu-id="59acb-122">说明</span><span class="sxs-lookup"><span data-stu-id="59acb-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59acb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59acb-123">Authorization</span></span>  | <span data-ttu-id="59acb-124">string</span><span class="sxs-lookup"><span data-stu-id="59acb-124">string</span></span>  | <span data-ttu-id="59acb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59acb-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="59acb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59acb-127">Request body</span></span>
<span data-ttu-id="59acb-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59acb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59acb-129">响应</span><span class="sxs-lookup"><span data-stu-id="59acb-129">Response</span></span>

<span data-ttu-id="59acb-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="59acb-130">If successful, this method returns a `200 OK` response code and a collection of [application](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59acb-131">示例</span><span class="sxs-lookup"><span data-stu-id="59acb-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59acb-132">请求</span><span class="sxs-lookup"><span data-stu-id="59acb-132">Request</span></span>
<span data-ttu-id="59acb-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59acb-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59acb-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="59acb-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59acb-135">C#</span><span class="sxs-lookup"><span data-stu-id="59acb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59acb-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59acb-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59acb-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59acb-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="59acb-138">Java</span><span class="sxs-lookup"><span data-stu-id="59acb-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59acb-139">响应</span><span class="sxs-lookup"><span data-stu-id="59acb-139">Response</span></span>
<span data-ttu-id="59acb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59acb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
