---
title: 获取 Outlook category
description: 获取指定的 outlookCategory 对象的属性和关系。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7bb91a91bee7b3562dd16c8236e0ce669c5174d9
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136491"
---
# <a name="get-outlook-category"></a><span data-ttu-id="c7584-103">获取 Outlook category</span><span class="sxs-lookup"><span data-stu-id="c7584-103">Get Outlook category</span></span>

<span data-ttu-id="c7584-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7584-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="c7584-105">获取指定的 [outlookCategory](../resources/outlookcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c7584-105">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7584-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c7584-106">Permissions</span></span>
<span data-ttu-id="c7584-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c7584-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7584-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c7584-109">Permission type</span></span>      | <span data-ttu-id="c7584-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c7584-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7584-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c7584-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c7584-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="c7584-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="c7584-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c7584-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7584-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="c7584-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="c7584-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c7584-115">Application</span></span> | <span data-ttu-id="c7584-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="c7584-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="c7584-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c7584-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c7584-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c7584-118">Optional query parameters</span></span>
<span data-ttu-id="c7584-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c7584-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7584-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c7584-120">Request headers</span></span>
| <span data-ttu-id="c7584-121">名称</span><span class="sxs-lookup"><span data-stu-id="c7584-121">Name</span></span>      |<span data-ttu-id="c7584-122">说明</span><span class="sxs-lookup"><span data-stu-id="c7584-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c7584-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7584-123">Authorization</span></span>  | <span data-ttu-id="c7584-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c7584-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7584-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c7584-126">Request body</span></span>
<span data-ttu-id="c7584-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c7584-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7584-128">响应</span><span class="sxs-lookup"><span data-stu-id="c7584-128">Response</span></span>

<span data-ttu-id="c7584-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c7584-129">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c7584-130">示例</span><span class="sxs-lookup"><span data-stu-id="c7584-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c7584-131">请求</span><span class="sxs-lookup"><span data-stu-id="c7584-131">Request</span></span>
<span data-ttu-id="c7584-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c7584-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c7584-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7584-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["de912e4d-c790-4da9-949c-ccd933aaa0f7"],
  "name": "get_outlookcategory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
# <a name="c"></a>[<span data-ttu-id="c7584-134">C#</span><span class="sxs-lookup"><span data-stu-id="c7584-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c7584-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7584-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c7584-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7584-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c7584-137">Java</span><span class="sxs-lookup"><span data-stu-id="c7584-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c7584-138">响应</span><span class="sxs-lookup"><span data-stu-id="c7584-138">Response</span></span>
<span data-ttu-id="c7584-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c7584-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 249

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
  "displayName":"Yellow category",
  "color":"preset3"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
