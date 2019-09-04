---
title: 列出 Outlook 类别
description: 获取为用户定义的所有类别。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: ce98ce6c0b686855d3fc7950f95a8defce9c8534
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725876"
---
# <a name="list-outlook-categories"></a><span data-ttu-id="86e29-103">列出 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="86e29-103">List Outlook categories</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86e29-104">获取为用户定义的所有类别。</span><span class="sxs-lookup"><span data-stu-id="86e29-104">Get all the categories that have been defined for the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="86e29-105">权限</span><span class="sxs-lookup"><span data-stu-id="86e29-105">Permissions</span></span>
<span data-ttu-id="86e29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86e29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86e29-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="86e29-108">Permission type</span></span>      | <span data-ttu-id="86e29-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86e29-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86e29-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86e29-110">Delegated (work or school account)</span></span> | <span data-ttu-id="86e29-111">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="86e29-111">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="86e29-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86e29-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86e29-113">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="86e29-113">MailboxSettings.Read</span></span>    |
|<span data-ttu-id="86e29-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="86e29-114">Application</span></span> | <span data-ttu-id="86e29-115">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="86e29-115">MailboxSettings.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="86e29-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86e29-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/masterCategories
GET /users/{id|userPrincipalName}/outlook/masterCategories
```
## <a name="optional-query-parameters"></a><span data-ttu-id="86e29-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86e29-117">Optional query parameters</span></span>
<span data-ttu-id="86e29-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="86e29-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86e29-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="86e29-119">Request headers</span></span>
| <span data-ttu-id="86e29-120">名称</span><span class="sxs-lookup"><span data-stu-id="86e29-120">Name</span></span>      |<span data-ttu-id="86e29-121">说明</span><span class="sxs-lookup"><span data-stu-id="86e29-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="86e29-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86e29-122">Authorization</span></span>  | <span data-ttu-id="86e29-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86e29-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86e29-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="86e29-125">Request body</span></span>
<span data-ttu-id="86e29-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86e29-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86e29-127">响应</span><span class="sxs-lookup"><span data-stu-id="86e29-127">Response</span></span>

<span data-ttu-id="86e29-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [outlookCategory](../resources/outlookcategory.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="86e29-128">If successful, this method returns a `200 OK` response code and collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86e29-129">示例</span><span class="sxs-lookup"><span data-stu-id="86e29-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86e29-130">请求</span><span class="sxs-lookup"><span data-stu-id="86e29-130">Request</span></span>
<span data-ttu-id="86e29-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="86e29-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="86e29-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="86e29-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_mastercategories"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/masterCategories
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="86e29-133">C#</span><span class="sxs-lookup"><span data-stu-id="86e29-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-mastercategories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="86e29-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86e29-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-mastercategories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="86e29-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="86e29-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-mastercategories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="86e29-136">响应</span><span class="sxs-lookup"><span data-stu-id="86e29-136">Response</span></span>
<span data-ttu-id="86e29-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="86e29-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 727

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories",
  "value":[
    {
      "id":"5a9a6aa8-b65f-4357-b1f9-60c6bf6330d8",
      "displayName":"Red category",
      "color":"preset0"
    },
    {
      "id":"4b1c2495-54c9-4a5e-90a2-0ab0b31987d8",
      "displayName":"Orange category",
      "color":"preset1"
    },
    {
      "id":"de912e4d-c790-4da9-949c-ccd933aaa0f7",
      "displayName":"Yellow category",
      "color":"preset3"
    },
    {
      "id":"79c8d8f8-9db1-49ec-99ce-ae25793e7232",
      "displayName":"Green category",
      "color":"preset4"
    },
    {
      "id":"626e696c-6a10-48b8-89b9-12de3160cfb9",
      "displayName":"Blue category",
      "color":"preset7"
    },
    {
      "id":"453d06d0-447d-41f7-91cd-aa0f6b190b5b",
      "displayName":"Purple category",
      "color":"preset8"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
