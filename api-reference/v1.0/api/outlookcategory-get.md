---
title: 获取 Outlook category
description: 获取指定的 outlookCategory 对象的属性和关系。
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8be4bc35a2d72794d269323097c1a68fe07a82de
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039207"
---
# <a name="get-outlook-category"></a><span data-ttu-id="4aac7-103">获取 Outlook category</span><span class="sxs-lookup"><span data-stu-id="4aac7-103">Get Outlook category</span></span>

<span data-ttu-id="4aac7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4aac7-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="4aac7-105">获取指定的 [outlookCategory](../resources/outlookcategory.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4aac7-105">Get the properties and relationships of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4aac7-106">权限</span><span class="sxs-lookup"><span data-stu-id="4aac7-106">Permissions</span></span>
<span data-ttu-id="4aac7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4aac7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aac7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4aac7-109">Permission type</span></span>      | <span data-ttu-id="4aac7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4aac7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4aac7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4aac7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4aac7-112">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4aac7-112">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4aac7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4aac7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4aac7-114">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4aac7-114">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="4aac7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4aac7-115">Application</span></span> | <span data-ttu-id="4aac7-116">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="4aac7-116">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="4aac7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4aac7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories/{id}
GET /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4aac7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4aac7-118">Optional query parameters</span></span>
<span data-ttu-id="4aac7-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4aac7-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4aac7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4aac7-120">Request headers</span></span>
| <span data-ttu-id="4aac7-121">名称</span><span class="sxs-lookup"><span data-stu-id="4aac7-121">Name</span></span>      |<span data-ttu-id="4aac7-122">说明</span><span class="sxs-lookup"><span data-stu-id="4aac7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4aac7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aac7-123">Authorization</span></span>  | <span data-ttu-id="4aac7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4aac7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4aac7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4aac7-126">Request body</span></span>
<span data-ttu-id="4aac7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4aac7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4aac7-128">响应</span><span class="sxs-lookup"><span data-stu-id="4aac7-128">Response</span></span>

<span data-ttu-id="4aac7-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4aac7-129">If successful, this method returns a `200 OK` response code and [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4aac7-130">示例</span><span class="sxs-lookup"><span data-stu-id="4aac7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4aac7-131">请求</span><span class="sxs-lookup"><span data-stu-id="4aac7-131">Request</span></span>
<span data-ttu-id="4aac7-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4aac7-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4aac7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4aac7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["de912e4d-c790-4da9-949c-ccd933aaa0f7"],
  "name": "get_outlookcategory"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/outlook/masterCategories/de912e4d-c790-4da9-949c-ccd933aaa0f7
```
# <a name="c"></a>[<span data-ttu-id="4aac7-134">C#</span><span class="sxs-lookup"><span data-stu-id="4aac7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4aac7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4aac7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4aac7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4aac7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4aac7-137">Java</span><span class="sxs-lookup"><span data-stu-id="4aac7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4aac7-138">响应</span><span class="sxs-lookup"><span data-stu-id="4aac7-138">Response</span></span>
<span data-ttu-id="4aac7-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="4aac7-139">Here is an example of the response.</span></span> <span data-ttu-id="4aac7-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4aac7-140">Note: The response object shown here might be shortened for readability.</span></span>
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
