---
title: orgContact：获取管理器
description: 获取联系人的经理
localization_priority: Normal
author: dkershaw10
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 3b1bf0939a7fe5e33b31ad9d2200e55da8464a67
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957763"
---
# <a name="orgcontact-get-manager"></a><span data-ttu-id="40467-103">orgContact：获取管理器</span><span class="sxs-lookup"><span data-stu-id="40467-103">orgContact: Get manager</span></span>

<span data-ttu-id="40467-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40467-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40467-105">获取联系人的经理</span><span class="sxs-lookup"><span data-stu-id="40467-105">Get the contact's manager</span></span>

## <a name="permissions"></a><span data-ttu-id="40467-106">权限</span><span class="sxs-lookup"><span data-stu-id="40467-106">Permissions</span></span>
<span data-ttu-id="40467-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40467-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="40467-109">Permission type</span></span>      | <span data-ttu-id="40467-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40467-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="40467-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40467-111">Delegated (work or school account)</span></span> | <span data-ttu-id="40467-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="40467-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="40467-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40467-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40467-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="40467-114">Not supported.</span></span>    |
|<span data-ttu-id="40467-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="40467-115">Application</span></span> | <span data-ttu-id="40467-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40467-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="40467-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40467-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /contacts/{id}/manager
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40467-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="40467-118">Optional query parameters</span></span>
<span data-ttu-id="40467-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="40467-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40467-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40467-120">Request headers</span></span>
| <span data-ttu-id="40467-121">名称</span><span class="sxs-lookup"><span data-stu-id="40467-121">Name</span></span>       | <span data-ttu-id="40467-122">类型</span><span class="sxs-lookup"><span data-stu-id="40467-122">Type</span></span> | <span data-ttu-id="40467-123">说明</span><span class="sxs-lookup"><span data-stu-id="40467-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="40467-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="40467-124">Authorization</span></span>  | <span data-ttu-id="40467-125">string</span><span class="sxs-lookup"><span data-stu-id="40467-125">string</span></span>  | <span data-ttu-id="40467-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="40467-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40467-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="40467-128">Request body</span></span>
<span data-ttu-id="40467-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="40467-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40467-130">响应</span><span class="sxs-lookup"><span data-stu-id="40467-130">Response</span></span>

<span data-ttu-id="40467-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="40467-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="40467-132">示例</span><span class="sxs-lookup"><span data-stu-id="40467-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="40467-133">请求</span><span class="sxs-lookup"><span data-stu-id="40467-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40467-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="40467-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manager_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/contacts/{id}/manager
```
# <a name="c"></a>[<span data-ttu-id="40467-135">C#</span><span class="sxs-lookup"><span data-stu-id="40467-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manager-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40467-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40467-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manager-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40467-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40467-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manager-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40467-138">Java</span><span class="sxs-lookup"><span data-stu-id="40467-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manager-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="40467-139">响应</span><span class="sxs-lookup"><span data-stu-id="40467-139">Response</span></span>

<span data-ttu-id="40467-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40467-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
