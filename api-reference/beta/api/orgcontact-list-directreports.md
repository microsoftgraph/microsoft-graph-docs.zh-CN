---
title: 'orgContact: List directReports'
description: 获取联系人的直接下属。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5d1e4ae94bb6b740293e450dbbf5889a89862bf4
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723733"
---
# <a name="orgcontact-list-directreports"></a><span data-ttu-id="59aee-103">orgContact: List directReports</span><span class="sxs-lookup"><span data-stu-id="59aee-103">orgContact: List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59aee-104">获取联系人的直接下属。</span><span class="sxs-lookup"><span data-stu-id="59aee-104">Get the contact's direct reports.</span></span>

## <a name="permissions"></a><span data-ttu-id="59aee-105">权限</span><span class="sxs-lookup"><span data-stu-id="59aee-105">Permissions</span></span>
<span data-ttu-id="59aee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59aee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59aee-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="59aee-108">Permission type</span></span>      | <span data-ttu-id="59aee-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59aee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59aee-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59aee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59aee-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59aee-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="59aee-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59aee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59aee-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="59aee-113">Not supported.</span></span>    |
|<span data-ttu-id="59aee-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="59aee-114">Application</span></span> | <span data-ttu-id="59aee-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59aee-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59aee-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59aee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59aee-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59aee-117">Optional query parameters</span></span>
<span data-ttu-id="59aee-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59aee-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59aee-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="59aee-119">Request headers</span></span>
| <span data-ttu-id="59aee-120">名称</span><span class="sxs-lookup"><span data-stu-id="59aee-120">Name</span></span>       | <span data-ttu-id="59aee-121">类型</span><span class="sxs-lookup"><span data-stu-id="59aee-121">Type</span></span> | <span data-ttu-id="59aee-122">说明</span><span class="sxs-lookup"><span data-stu-id="59aee-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59aee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59aee-123">Authorization</span></span>  | <span data-ttu-id="59aee-124">string</span><span class="sxs-lookup"><span data-stu-id="59aee-124">string</span></span>  | <span data-ttu-id="59aee-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59aee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59aee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="59aee-127">Request body</span></span>
<span data-ttu-id="59aee-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59aee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59aee-129">响应</span><span class="sxs-lookup"><span data-stu-id="59aee-129">Response</span></span>

<span data-ttu-id="59aee-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="59aee-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="59aee-131">示例</span><span class="sxs-lookup"><span data-stu-id="59aee-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59aee-132">请求</span><span class="sxs-lookup"><span data-stu-id="59aee-132">Request</span></span>
<span data-ttu-id="59aee-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59aee-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="59aee-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="59aee-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "contacts_get_directreports"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/directReports
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="59aee-135">C#</span><span class="sxs-lookup"><span data-stu-id="59aee-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/contacts-get-directreports-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="59aee-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59aee-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/contacts-get-directreports-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="59aee-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="59aee-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/contacts-get-directreports-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59aee-138">响应</span><span class="sxs-lookup"><span data-stu-id="59aee-138">Response</span></span>
<span data-ttu-id="59aee-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59aee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
