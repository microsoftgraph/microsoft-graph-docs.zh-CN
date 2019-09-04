---
title: 列出 orgContacts
description: 检索此组织的组织联系人列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8de141d16f02db3ebe420119d622232fd6a5a621
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723726"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="c1c5d-103">列出 orgContacts</span><span class="sxs-lookup"><span data-stu-id="c1c5d-103">List orgContacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1c5d-104">获取此组织的组织联系人列表。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-104">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1c5d-105">权限</span><span class="sxs-lookup"><span data-stu-id="c1c5d-105">Permissions</span></span>
<span data-ttu-id="c1c5d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c1c5d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1c5d-108">Permission type</span></span>      | <span data-ttu-id="c1c5d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1c5d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c1c5d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1c5d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c1c5d-111">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-111">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c1c5d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1c5d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c1c5d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-113">Not supported.</span></span>    |
|<span data-ttu-id="c1c5d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1c5d-114">Application</span></span> | <span data-ttu-id="c1c5d-115">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-115">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c1c5d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1c5d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c1c5d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c1c5d-117">Optional query parameters</span></span>
<span data-ttu-id="c1c5d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c1c5d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1c5d-119">Request headers</span></span>
| <span data-ttu-id="c1c5d-120">名称</span><span class="sxs-lookup"><span data-stu-id="c1c5d-120">Name</span></span>       | <span data-ttu-id="c1c5d-121">类型</span><span class="sxs-lookup"><span data-stu-id="c1c5d-121">Type</span></span> | <span data-ttu-id="c1c5d-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1c5d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c1c5d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1c5d-123">Authorization</span></span>  | <span data-ttu-id="c1c5d-124">string</span><span class="sxs-lookup"><span data-stu-id="c1c5d-124">string</span></span>  | <span data-ttu-id="c1c5d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c1c5d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1c5d-127">Request body</span></span>
<span data-ttu-id="c1c5d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c1c5d-129">响应</span><span class="sxs-lookup"><span data-stu-id="c1c5d-129">Response</span></span>

<span data-ttu-id="c1c5d-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-130">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c1c5d-131">示例</span><span class="sxs-lookup"><span data-stu-id="c1c5d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c1c5d-132">请求</span><span class="sxs-lookup"><span data-stu-id="c1c5d-132">Request</span></span>
<span data-ttu-id="c1c5d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c1c5d-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c1c5d-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c1c5d-135">C#</span><span class="sxs-lookup"><span data-stu-id="c1c5d-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c1c5d-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1c5d-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c1c5d-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="c1c5d-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c1c5d-138">响应</span><span class="sxs-lookup"><span data-stu-id="c1c5d-138">Response</span></span>
<span data-ttu-id="c1c5d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c1c5d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.orgcontact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 222

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List orgContact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
