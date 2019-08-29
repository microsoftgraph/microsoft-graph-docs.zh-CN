---
title: 获取 orgContact
description: 检索 orgcontact 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: afde0586d165d452576de5e984d91bf9a1e53e3f
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667531"
---
# <a name="get-orgcontact"></a><span data-ttu-id="e7181-103">获取 orgContact</span><span class="sxs-lookup"><span data-stu-id="e7181-103">Get orgContact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7181-104">获取组织联系人对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e7181-104">Get the properties and relationships of an organizational contact object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e7181-105">权限</span><span class="sxs-lookup"><span data-stu-id="e7181-105">Permissions</span></span>
<span data-ttu-id="e7181-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7181-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7181-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7181-108">Permission type</span></span>      | <span data-ttu-id="e7181-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7181-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e7181-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7181-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e7181-111">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="e7181-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e7181-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7181-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e7181-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7181-113">Not supported.</span></span>    |
|<span data-ttu-id="e7181-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7181-114">Application</span></span> | <span data-ttu-id="e7181-115">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="e7181-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e7181-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7181-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e7181-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e7181-117">Optional query parameters</span></span>
<span data-ttu-id="e7181-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e7181-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e7181-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7181-119">Request headers</span></span>
| <span data-ttu-id="e7181-120">名称</span><span class="sxs-lookup"><span data-stu-id="e7181-120">Name</span></span>       | <span data-ttu-id="e7181-121">类型</span><span class="sxs-lookup"><span data-stu-id="e7181-121">Type</span></span> | <span data-ttu-id="e7181-122">说明</span><span class="sxs-lookup"><span data-stu-id="e7181-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e7181-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7181-123">Authorization</span></span>  | <span data-ttu-id="e7181-124">string</span><span class="sxs-lookup"><span data-stu-id="e7181-124">string</span></span>  | <span data-ttu-id="e7181-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e7181-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e7181-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7181-127">Request body</span></span>
<span data-ttu-id="e7181-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e7181-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e7181-129">响应</span><span class="sxs-lookup"><span data-stu-id="e7181-129">Response</span></span>

<span data-ttu-id="e7181-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7181-130">If successful, this method returns a `200 OK` response code and [orgContact](../resources/orgcontact.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e7181-131">示例</span><span class="sxs-lookup"><span data-stu-id="e7181-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e7181-132">请求</span><span class="sxs-lookup"><span data-stu-id="e7181-132">Request</span></span>
<span data-ttu-id="e7181-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7181-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e7181-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e7181-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_orgcontact"
}-->
```http
GET https://graph.microsoft.com/beta/contacts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e7181-135">C#</span><span class="sxs-lookup"><span data-stu-id="e7181-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e7181-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e7181-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e7181-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="e7181-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e7181-138">响应</span><span class="sxs-lookup"><span data-stu-id="e7181-138">Response</span></span>
<span data-ttu-id="e7181-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7181-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "addresses":[
      {
        "city": "string",
        "countryOrRegion": "string",
        "officeLocation": "string",
        "postalCode": "string",
        "state": "string",
        "street": "string"
      }
  ],
  "companyName": "companyName-value",
  "department": "department-value",
  "displayName": "displayName-value",
  "phones":[
      {
        "type": "string",
        "number": "string"
      }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
