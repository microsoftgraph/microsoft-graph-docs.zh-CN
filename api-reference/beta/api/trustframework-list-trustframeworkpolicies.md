---
title: 列出 trustFrameworkPolicies
description: 此操作列出了 Azure AD B2C 租户中的所有 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 61e110d00bb39074314f847cdfb530b9488a855f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452181"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="7905e-103">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="7905e-103">List trustFrameworkPolicies</span></span>

<span data-ttu-id="7905e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7905e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7905e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7905e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7905e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7905e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7905e-107">检索租户/目录中的[trustFrameworkPolicies](../resources/trustframeworkpolicy.md)列表。</span><span class="sxs-lookup"><span data-stu-id="7905e-107">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="7905e-108">权限</span><span class="sxs-lookup"><span data-stu-id="7905e-108">Permissions</span></span>

<span data-ttu-id="7905e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7905e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7905e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7905e-111">Permission type</span></span>      | <span data-ttu-id="7905e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7905e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7905e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7905e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7905e-114">Policy： Read. All，TrustFramework</span><span class="sxs-lookup"><span data-stu-id="7905e-114">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|
|<span data-ttu-id="7905e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7905e-115">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7905e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7905e-116">Not supported.</span></span>|
|<span data-ttu-id="7905e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7905e-117">Application</span></span>|<span data-ttu-id="7905e-118">Policy： Read. All，TrustFramework</span><span class="sxs-lookup"><span data-stu-id="7905e-118">Policy.Read.All, Policy.ReadWrite.TrustFramework</span></span>|

<span data-ttu-id="7905e-119">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="7905e-119">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="7905e-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7905e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7905e-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7905e-121">Optional query parameters</span></span>

<span data-ttu-id="7905e-122">此方法支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7905e-122">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7905e-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="7905e-123">Request headers</span></span>

|<span data-ttu-id="7905e-124">名称</span><span class="sxs-lookup"><span data-stu-id="7905e-124">Name</span></span>|<span data-ttu-id="7905e-125">说明</span><span class="sxs-lookup"><span data-stu-id="7905e-125">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="7905e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7905e-126">Authorization</span></span>|<span data-ttu-id="7905e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7905e-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7905e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7905e-129">Request body</span></span>

<span data-ttu-id="7905e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7905e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7905e-131">响应</span><span class="sxs-lookup"><span data-stu-id="7905e-131">Response</span></span>

<span data-ttu-id="7905e-132">如果成功，此方法在响应`200 OK`正文的 JSON 表示形式中返回响应代码和[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7905e-132">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7905e-133">示例</span><span class="sxs-lookup"><span data-stu-id="7905e-133">Example</span></span>

<span data-ttu-id="7905e-134">下面的示例检索所有**trustFrameworkPolicies**。</span><span class="sxs-lookup"><span data-stu-id="7905e-134">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="7905e-135">请求</span><span class="sxs-lookup"><span data-stu-id="7905e-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7905e-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="7905e-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_trustFrameworks"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/trustFramework/policies
```
# <a name="c"></a>[<span data-ttu-id="7905e-137">C#</span><span class="sxs-lookup"><span data-stu-id="7905e-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-trustframeworks-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7905e-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7905e-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-trustframeworks-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7905e-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7905e-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-trustframeworks-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7905e-140">响应</span><span class="sxs-lookup"><span data-stu-id="7905e-140">Response</span></span>

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
