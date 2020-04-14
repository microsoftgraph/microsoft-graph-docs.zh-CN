---
title: 列出 orgContacts
description: 检索此组织的组织联系人列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 87669fb0665a11d1f3bc6f1bf923cd55e1ee3af3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474728"
---
# <a name="list-orgcontacts"></a><span data-ttu-id="d6349-103">列出 orgContacts</span><span class="sxs-lookup"><span data-stu-id="d6349-103">List orgContacts</span></span>

<span data-ttu-id="d6349-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6349-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6349-105">获取此组织的组织联系人列表。</span><span class="sxs-lookup"><span data-stu-id="d6349-105">Get the list of organizational contacts for this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="d6349-106">权限</span><span class="sxs-lookup"><span data-stu-id="d6349-106">Permissions</span></span>
<span data-ttu-id="d6349-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6349-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6349-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6349-109">Permission type</span></span>      | <span data-ttu-id="d6349-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d6349-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d6349-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6349-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d6349-112">OrgContact、Directory.accessasuser.all、所有的目录、所有、和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="d6349-112">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d6349-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6349-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d6349-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6349-114">Not supported.</span></span>    |
|<span data-ttu-id="d6349-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6349-115">Application</span></span> | <span data-ttu-id="d6349-116">OrgContact、所有目录、全部读取、所有读写。</span><span class="sxs-lookup"><span data-stu-id="d6349-116">OrgContact.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d6349-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6349-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d6349-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d6349-118">Optional query parameters</span></span>
<span data-ttu-id="d6349-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d6349-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d6349-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6349-120">Request headers</span></span>
| <span data-ttu-id="d6349-121">名称</span><span class="sxs-lookup"><span data-stu-id="d6349-121">Name</span></span>       | <span data-ttu-id="d6349-122">类型</span><span class="sxs-lookup"><span data-stu-id="d6349-122">Type</span></span> | <span data-ttu-id="d6349-123">说明</span><span class="sxs-lookup"><span data-stu-id="d6349-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d6349-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6349-124">Authorization</span></span>  | <span data-ttu-id="d6349-125">string</span><span class="sxs-lookup"><span data-stu-id="d6349-125">string</span></span>  | <span data-ttu-id="d6349-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d6349-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d6349-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6349-128">Request body</span></span>
<span data-ttu-id="d6349-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d6349-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6349-130">响应</span><span class="sxs-lookup"><span data-stu-id="d6349-130">Response</span></span>

<span data-ttu-id="d6349-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[orgContact](../resources/orgcontact.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d6349-131">If successful, this method returns a `200 OK` response code and a collection of [orgContact](../resources/orgcontact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d6349-132">示例</span><span class="sxs-lookup"><span data-stu-id="d6349-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d6349-133">请求</span><span class="sxs-lookup"><span data-stu-id="d6349-133">Request</span></span>
<span data-ttu-id="d6349-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6349-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d6349-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d6349-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_orgcontact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts
```
# <a name="c"></a>[<span data-ttu-id="d6349-136">C#</span><span class="sxs-lookup"><span data-stu-id="d6349-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-orgcontact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d6349-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d6349-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-orgcontact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d6349-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d6349-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-orgcontact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d6349-139">响应</span><span class="sxs-lookup"><span data-stu-id="d6349-139">Response</span></span>
<span data-ttu-id="d6349-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6349-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
