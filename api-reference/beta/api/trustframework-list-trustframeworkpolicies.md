---
title: 列出 trustFrameworkPolicies
description: 此操作列出了 Azure AD B2C 租户中的所有 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f10cb19e78a1607cc6d535e97e593e604b743703
ms.sourcegitcommit: 126b15ac37fb199c7b1001f91e70d8463a18c280
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/16/2019
ms.locfileid: "34083262"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="aadd0-103">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="aadd0-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="aadd0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aadd0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aadd0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aadd0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aadd0-106">检索租户/目录中的[trustFrameworkPolicies](../resources/trustframeworkpolicy.md)列表。</span><span class="sxs-lookup"><span data-stu-id="aadd0-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="aadd0-107">权限</span><span class="sxs-lookup"><span data-stu-id="aadd0-107">Permissions</span></span>

<span data-ttu-id="aadd0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aadd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aadd0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aadd0-110">Permission type</span></span>      | <span data-ttu-id="aadd0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aadd0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aadd0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aadd0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aadd0-113">TrustFramework、Policy、Read。 All</span><span class="sxs-lookup"><span data-stu-id="aadd0-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="aadd0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aadd0-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="aadd0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aadd0-115">Not supported.</span></span>|
|<span data-ttu-id="aadd0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aadd0-116">Application</span></span>|<span data-ttu-id="aadd0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aadd0-117">Not supported.</span></span>|

<span data-ttu-id="aadd0-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="aadd0-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="aadd0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aadd0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aadd0-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aadd0-120">Optional query parameters</span></span>

<span data-ttu-id="aadd0-121">此方法支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="aadd0-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aadd0-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="aadd0-122">Request headers</span></span>

|<span data-ttu-id="aadd0-123">名称</span><span class="sxs-lookup"><span data-stu-id="aadd0-123">Name</span></span>|<span data-ttu-id="aadd0-124">说明</span><span class="sxs-lookup"><span data-stu-id="aadd0-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="aadd0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="aadd0-125">Authorization</span></span>|<span data-ttu-id="aadd0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aadd0-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="aadd0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="aadd0-128">Request body</span></span>

<span data-ttu-id="aadd0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aadd0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aadd0-130">响应</span><span class="sxs-lookup"><span data-stu-id="aadd0-130">Response</span></span>

<span data-ttu-id="aadd0-131">如果成功, 此方法在响应`200 OK`正文的 JSON 表示形式中返回响应代码和[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="aadd0-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aadd0-132">示例</span><span class="sxs-lookup"><span data-stu-id="aadd0-132">Example</span></span>

<span data-ttu-id="aadd0-133">下面的示例检索所有**trustFrameworkPolicies**。</span><span class="sxs-lookup"><span data-stu-id="aadd0-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="aadd0-134">请求</span><span class="sxs-lookup"><span data-stu-id="aadd0-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```

##### <a name="response"></a><span data-ttu-id="aadd0-135">响应</span><span class="sxs-lookup"><span data-stu-id="aadd0-135">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="aadd0-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="aadd0-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aadd0-137">C#</span><span class="sxs-lookup"><span data-stu-id="aadd0-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aadd0-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="aadd0-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_trustFrameworks-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/trustframework-list-trustframeworkpolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
