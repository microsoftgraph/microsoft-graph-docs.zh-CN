---
title: 列出 trustFrameworkPolicies
description: 此操作列出了 Azure AD B2C 租户中的所有 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 019b309a4c789cef3da5e8ac6f0ccc0aabbe13e3
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722102"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="ec315-103">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="ec315-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="ec315-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ec315-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec315-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ec315-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec315-106">检索租户/目录中的[trustFrameworkPolicies](../resources/trustframeworkpolicy.md)列表。</span><span class="sxs-lookup"><span data-stu-id="ec315-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec315-107">权限</span><span class="sxs-lookup"><span data-stu-id="ec315-107">Permissions</span></span>

<span data-ttu-id="ec315-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec315-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec315-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec315-110">Permission type</span></span>      | <span data-ttu-id="ec315-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ec315-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec315-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec315-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec315-113">TrustFramework、Policy、Read. All</span><span class="sxs-lookup"><span data-stu-id="ec315-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="ec315-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec315-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="ec315-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec315-115">Not supported.</span></span>|
|<span data-ttu-id="ec315-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec315-116">Application</span></span>|<span data-ttu-id="ec315-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec315-117">Not supported.</span></span>|

<span data-ttu-id="ec315-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="ec315-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="ec315-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec315-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ec315-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ec315-120">Optional query parameters</span></span>

<span data-ttu-id="ec315-121">此方法支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ec315-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec315-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec315-122">Request headers</span></span>

|<span data-ttu-id="ec315-123">名称</span><span class="sxs-lookup"><span data-stu-id="ec315-123">Name</span></span>|<span data-ttu-id="ec315-124">说明</span><span class="sxs-lookup"><span data-stu-id="ec315-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="ec315-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec315-125">Authorization</span></span>|<span data-ttu-id="ec315-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ec315-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec315-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec315-128">Request body</span></span>

<span data-ttu-id="ec315-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ec315-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec315-130">响应</span><span class="sxs-lookup"><span data-stu-id="ec315-130">Response</span></span>

<span data-ttu-id="ec315-131">如果成功, 此方法在响应`200 OK`正文的 JSON 表示形式中返回响应代码和[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ec315-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec315-132">示例</span><span class="sxs-lookup"><span data-stu-id="ec315-132">Example</span></span>

<span data-ttu-id="ec315-133">下面的示例检索所有**trustFrameworkPolicies**。</span><span class="sxs-lookup"><span data-stu-id="ec315-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="ec315-134">请求</span><span class="sxs-lookup"><span data-stu-id="ec315-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ec315-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ec315-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec315-136">C#</span><span class="sxs-lookup"><span data-stu-id="ec315-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec315-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ec315-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec315-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="ec315-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ec315-139">响应</span><span class="sxs-lookup"><span data-stu-id="ec315-139">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "B2C_1A_CustomPolicy2"
        },
        {
            "id": "B2C_1A_CustomPolicy3"
        },
        {
            "id": "B2C_1A_SocialAndLocalAccounts_Base"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
