---
title: 列出 trustFrameworkPolicies
description: 此操作列出了 Azure AD B2C 租户中的所有 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 90f54512221c22014228e7309467b808772e0a1d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362547"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="3864b-103">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="3864b-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="3864b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3864b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3864b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3864b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3864b-106">检索租户/目录中的[trustFrameworkPolicies](../resources/trustframeworkpolicy.md)列表。</span><span class="sxs-lookup"><span data-stu-id="3864b-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="3864b-107">权限</span><span class="sxs-lookup"><span data-stu-id="3864b-107">Permissions</span></span>

<span data-ttu-id="3864b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3864b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3864b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3864b-110">Permission type</span></span>      | <span data-ttu-id="3864b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3864b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3864b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3864b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3864b-113">TrustFramework、Policy、Read. All</span><span class="sxs-lookup"><span data-stu-id="3864b-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="3864b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3864b-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3864b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3864b-115">Not supported.</span></span>|
|<span data-ttu-id="3864b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3864b-116">Application</span></span>|<span data-ttu-id="3864b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3864b-117">Not supported.</span></span>|

<span data-ttu-id="3864b-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="3864b-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="3864b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3864b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3864b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3864b-120">Optional query parameters</span></span>

<span data-ttu-id="3864b-121">此方法支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3864b-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3864b-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3864b-122">Request headers</span></span>

|<span data-ttu-id="3864b-123">名称</span><span class="sxs-lookup"><span data-stu-id="3864b-123">Name</span></span>|<span data-ttu-id="3864b-124">说明</span><span class="sxs-lookup"><span data-stu-id="3864b-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3864b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3864b-125">Authorization</span></span>|<span data-ttu-id="3864b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3864b-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3864b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3864b-128">Request body</span></span>

<span data-ttu-id="3864b-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3864b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3864b-130">响应</span><span class="sxs-lookup"><span data-stu-id="3864b-130">Response</span></span>

<span data-ttu-id="3864b-131">如果成功, 此方法在响应`200 OK`正文的 JSON 表示形式中返回响应代码和[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="3864b-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3864b-132">示例</span><span class="sxs-lookup"><span data-stu-id="3864b-132">Example</span></span>

<span data-ttu-id="3864b-133">下面的示例检索所有**trustFrameworkPolicies**。</span><span class="sxs-lookup"><span data-stu-id="3864b-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="3864b-134">请求</span><span class="sxs-lookup"><span data-stu-id="3864b-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3864b-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3864b-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3864b-136">C#</span><span class="sxs-lookup"><span data-stu-id="3864b-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3864b-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3864b-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3864b-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="3864b-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3864b-139">Java</span><span class="sxs-lookup"><span data-stu-id="3864b-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-trustframeworks-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3864b-140">响应</span><span class="sxs-lookup"><span data-stu-id="3864b-140">Response</span></span>

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
