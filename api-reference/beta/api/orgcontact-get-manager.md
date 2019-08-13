---
title: 'orgContact: 获取管理器'
description: 获取联系人的经理
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 229ca8638a12f2291499347b9231960ee2482b00
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342458"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="41b35-103">orgContact: 获取管理器</span><span class="sxs-lookup"><span data-stu-id="41b35-103">orgContact: Get manager</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41b35-104">获取联系人的经理</span><span class="sxs-lookup"><span data-stu-id="41b35-104">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="41b35-105">权限</span><span class="sxs-lookup"><span data-stu-id="41b35-105">Permissions</span></span>
<span data-ttu-id="41b35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41b35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41b35-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="41b35-108">Permission type</span></span>      | <span data-ttu-id="41b35-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41b35-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41b35-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41b35-110">Delegated (work or school account)</span></span> | <span data-ttu-id="41b35-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41b35-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41b35-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41b35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41b35-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="41b35-113">Not supported.</span></span>    |
|<span data-ttu-id="41b35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="41b35-114">Application</span></span> | <span data-ttu-id="41b35-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41b35-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41b35-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41b35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41b35-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41b35-117">Optional query parameters</span></span>
<span data-ttu-id="41b35-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41b35-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41b35-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="41b35-119">Request headers</span></span>
| <span data-ttu-id="41b35-120">名称</span><span class="sxs-lookup"><span data-stu-id="41b35-120">Name</span></span>       | <span data-ttu-id="41b35-121">类型</span><span class="sxs-lookup"><span data-stu-id="41b35-121">Type</span></span> | <span data-ttu-id="41b35-122">说明</span><span class="sxs-lookup"><span data-stu-id="41b35-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="41b35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="41b35-123">Authorization</span></span>  | <span data-ttu-id="41b35-124">string</span><span class="sxs-lookup"><span data-stu-id="41b35-124">string</span></span>  | <span data-ttu-id="41b35-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41b35-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41b35-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="41b35-127">Request body</span></span>
<span data-ttu-id="41b35-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41b35-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41b35-129">响应</span><span class="sxs-lookup"><span data-stu-id="41b35-129">Response</span></span>

<span data-ttu-id="41b35-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="41b35-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41b35-131">示例</span><span class="sxs-lookup"><span data-stu-id="41b35-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="41b35-132">请求</span><span class="sxs-lookup"><span data-stu-id="41b35-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="41b35-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="41b35-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager"
}-->

```http
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="41b35-134">C#</span><span class="sxs-lookup"><span data-stu-id="41b35-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="41b35-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41b35-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="41b35-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="41b35-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="41b35-137">Java</span><span class="sxs-lookup"><span data-stu-id="41b35-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="41b35-138">响应</span><span class="sxs-lookup"><span data-stu-id="41b35-138">Response</span></span>

<span data-ttu-id="41b35-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41b35-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 455

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "24fcbca3-c3e2-48bf-9ffc-c7f81b81483d",
    "businessPhones": [
        "+1 205 555 0108"
    ],
    "displayName": "Diego Siciliani",
    "givenName": "Diego",
    "jobTitle": "CVP Finance",
    "mail": "DiegoS@contoso.com",
    "mobilePhone": null,
    "officeLocation": "14/1108",
    "preferredLanguage": "en-US",
    "surname": "Siciliani",
    "userPrincipalName": "DiegoS@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get manager",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
