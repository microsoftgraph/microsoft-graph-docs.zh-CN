---
title: 获取协议
description: 检索协议对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 92b794270c0912f1320f8bb2b5dcf47d1f976f5e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942892"
---
# <a name="get-agreement"></a><span data-ttu-id="87172-103">获取协议</span><span class="sxs-lookup"><span data-stu-id="87172-103">Get agreement</span></span>

<span data-ttu-id="87172-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87172-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87172-105">检索协议对象的属性 [和](../resources/agreement.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="87172-105">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="87172-106">权限</span><span class="sxs-lookup"><span data-stu-id="87172-106">Permissions</span></span>
<span data-ttu-id="87172-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="87172-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87172-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="87172-109">Permission type</span></span>                        | <span data-ttu-id="87172-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="87172-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="87172-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="87172-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="87172-112">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="87172-112">Agreement.Read.All</span></span> |
|<span data-ttu-id="87172-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="87172-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87172-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="87172-114">Not supported.</span></span> |
|<span data-ttu-id="87172-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="87172-115">Application</span></span>                            | <span data-ttu-id="87172-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="87172-116">Not supported.</span></span> |

<span data-ttu-id="87172-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="87172-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="87172-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="87172-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="87172-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="87172-119">Global Administrator</span></span>
+ <span data-ttu-id="87172-120">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="87172-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="87172-121">安全管理员</span><span class="sxs-lookup"><span data-stu-id="87172-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="87172-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="87172-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/termsOfUse/agreements/{id}
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="87172-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="87172-123">Request headers</span></span>
| <span data-ttu-id="87172-124">名称</span><span class="sxs-lookup"><span data-stu-id="87172-124">Name</span></span>         | <span data-ttu-id="87172-125">类型</span><span class="sxs-lookup"><span data-stu-id="87172-125">Type</span></span>        | <span data-ttu-id="87172-126">说明</span><span class="sxs-lookup"><span data-stu-id="87172-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="87172-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="87172-127">Authorization</span></span> | <span data-ttu-id="87172-128">string</span><span class="sxs-lookup"><span data-stu-id="87172-128">string</span></span> | <span data-ttu-id="87172-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="87172-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="87172-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="87172-131">Request body</span></span>
<span data-ttu-id="87172-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="87172-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="87172-133">响应</span><span class="sxs-lookup"><span data-stu-id="87172-133">Response</span></span>
<span data-ttu-id="87172-134">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/agreement.md) 代码和 agreement 对象。</span><span class="sxs-lookup"><span data-stu-id="87172-134">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="87172-135">示例</span><span class="sxs-lookup"><span data-stu-id="87172-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="87172-136">请求</span><span class="sxs-lookup"><span data-stu-id="87172-136">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="87172-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="87172-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements/{id}?$expand=files
```
# <a name="c"></a>[<span data-ttu-id="87172-138">C#</span><span class="sxs-lookup"><span data-stu-id="87172-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-agreement-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87172-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87172-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-agreement-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87172-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87172-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-agreement-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87172-141">Java</span><span class="sxs-lookup"><span data-stu-id="87172-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-agreement-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="87172-142">响应</span><span class="sxs-lookup"><span data-stu-id="87172-142">Response</span></span>
><span data-ttu-id="87172-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="87172-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
