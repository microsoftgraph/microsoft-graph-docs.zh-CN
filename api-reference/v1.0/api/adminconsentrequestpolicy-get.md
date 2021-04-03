---
title: 获取 adminConsentRequestPolicy
description: 读取 adminConsentRequestPolicy 对象的属性和关系。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: cfbd3cd98c17c9e261711932a0169c977b1d59ba
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508287"
---
# <a name="get-adminconsentrequestpolicy"></a><span data-ttu-id="9122c-103">获取 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="9122c-103">Get adminConsentRequestPolicy</span></span>

<span data-ttu-id="9122c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9122c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9122c-105">读取 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9122c-105">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9122c-106">权限</span><span class="sxs-lookup"><span data-stu-id="9122c-106">Permissions</span></span>

<span data-ttu-id="9122c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9122c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9122c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9122c-109">Permission type</span></span>|<span data-ttu-id="9122c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9122c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9122c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9122c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9122c-112">Policy.Read.All、Policy.ReadWrite.ConsentRequest、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9122c-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="9122c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9122c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9122c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9122c-114">Not supported.</span></span>|
|<span data-ttu-id="9122c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9122c-115">Application</span></span>|<span data-ttu-id="9122c-116">Policy.Read.All、Policy.ReadWrite.ConsentRequest、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9122c-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|

<span data-ttu-id="9122c-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="9122c-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="9122c-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="9122c-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="9122c-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="9122c-119">Global Administrator</span></span>
+ <span data-ttu-id="9122c-120">全局读取者</span><span class="sxs-lookup"><span data-stu-id="9122c-120">Global Reader</span></span>
+ <span data-ttu-id="9122c-121">云 应用程序管理员</span><span class="sxs-lookup"><span data-stu-id="9122c-121">Cloud Application Administrator</span></span>
+ <span data-ttu-id="9122c-122"> 应用程序管理员</span><span class="sxs-lookup"><span data-stu-id="9122c-122">Application Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9122c-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9122c-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9122c-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9122c-124">Optional query parameters</span></span>

<span data-ttu-id="9122c-125">此方法支持  `$select`   OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9122c-125">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="9122c-126">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9122c-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9122c-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="9122c-127">Request headers</span></span>

|<span data-ttu-id="9122c-128">名称</span><span class="sxs-lookup"><span data-stu-id="9122c-128">Name</span></span>|<span data-ttu-id="9122c-129">说明</span><span class="sxs-lookup"><span data-stu-id="9122c-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9122c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9122c-130">Authorization</span></span>|<span data-ttu-id="9122c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9122c-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9122c-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="9122c-133">Request body</span></span>

<span data-ttu-id="9122c-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9122c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9122c-135">响应</span><span class="sxs-lookup"><span data-stu-id="9122c-135">Response</span></span>

<span data-ttu-id="9122c-136">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9122c-136">If successful, this method returns a `200 OK` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9122c-137">示例</span><span class="sxs-lookup"><span data-stu-id="9122c-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9122c-138">请求</span><span class="sxs-lookup"><span data-stu-id="9122c-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9122c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="9122c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy
```
# <a name="c"></a>[<span data-ttu-id="9122c-140">C#</span><span class="sxs-lookup"><span data-stu-id="9122c-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9122c-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9122c-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9122c-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9122c-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9122c-143">Java</span><span class="sxs-lookup"><span data-stu-id="9122c-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9122c-144">响应</span><span class="sxs-lookup"><span data-stu-id="9122c-144">Response</span></span>

<span data-ttu-id="9122c-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9122c-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/adminConsentRequestPolicy/$entity",
  "isEnabled": true,
  "notifyReviewers": false,
  "remindersEnabled": false,
  "requestDurationInDays": 0,
  "version": 0,
  "reviewers": [
    {
      "query": "/users/906e0ee5-6372-4cc8-8248-fdf2846b48ed",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    },
    {
      "query": "/users/daddef1a-acb0-4f62-96d0-49df2495d657",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ]
}
```
