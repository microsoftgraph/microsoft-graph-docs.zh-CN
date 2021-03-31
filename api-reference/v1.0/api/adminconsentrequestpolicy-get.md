---
title: 获取 adminConsentRequestPolicy
description: 读取 adminConsentRequestPolicy 对象的属性和关系。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f9a6d19c1671265034ca5f2663ab55aa701eeda8
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469539"
---
# <a name="get-adminconsentrequestpolicy"></a><span data-ttu-id="06b81-103">获取 adminConsentRequestPolicy</span><span class="sxs-lookup"><span data-stu-id="06b81-103">Get adminConsentRequestPolicy</span></span>

<span data-ttu-id="06b81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06b81-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="06b81-105">读取 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06b81-105">Read the properties and relationships of an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="06b81-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="06b81-106">Permissions</span></span>

<span data-ttu-id="06b81-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06b81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06b81-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="06b81-109">Permission type</span></span>|<span data-ttu-id="06b81-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06b81-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06b81-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06b81-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06b81-112">Policy.Read.All、Policy.ReadWrite.ConsentRequest、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06b81-112">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="06b81-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06b81-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06b81-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="06b81-114">Not supported.</span></span>|
|<span data-ttu-id="06b81-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="06b81-115">Application</span></span>|<span data-ttu-id="06b81-116">Policy.Read.All、Policy.ReadWrite.ConsentRequest、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="06b81-116">Policy.Read.All, Policy.ReadWrite.ConsentRequest, Directory.Read.All, Directory.ReadWrite.All</span></span>|

<span data-ttu-id="06b81-117">代表用户进行呼叫时，用户需要属于以下目录角色之一。</span><span class="sxs-lookup"><span data-stu-id="06b81-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="06b81-118">若要了解有关目录角色的信息，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：</span><span class="sxs-lookup"><span data-stu-id="06b81-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="06b81-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="06b81-119">Global Administrator</span></span>
+ <span data-ttu-id="06b81-120">全局读取者</span><span class="sxs-lookup"><span data-stu-id="06b81-120">Global Reader</span></span>
+ <span data-ttu-id="06b81-121">云 应用程序管理员</span><span class="sxs-lookup"><span data-stu-id="06b81-121">Cloud Application Administrator</span></span>
+ <span data-ttu-id="06b81-122"> 应用程序管理员</span><span class="sxs-lookup"><span data-stu-id="06b81-122">Application Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="06b81-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06b81-123">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/adminConsentRequestPolicy
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06b81-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="06b81-124">Optional query parameters</span></span>

<span data-ttu-id="06b81-125">此方法支持  `$select`   OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="06b81-125">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="06b81-126">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="06b81-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="06b81-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="06b81-127">Request headers</span></span>

|<span data-ttu-id="06b81-128">名称</span><span class="sxs-lookup"><span data-stu-id="06b81-128">Name</span></span>|<span data-ttu-id="06b81-129">说明</span><span class="sxs-lookup"><span data-stu-id="06b81-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06b81-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="06b81-130">Authorization</span></span>|<span data-ttu-id="06b81-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06b81-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06b81-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="06b81-133">Request body</span></span>

<span data-ttu-id="06b81-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06b81-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06b81-135">响应</span><span class="sxs-lookup"><span data-stu-id="06b81-135">Response</span></span>

<span data-ttu-id="06b81-136">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="06b81-136">If successful, this method returns a `200 OK` response code and an [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="06b81-137">示例</span><span class="sxs-lookup"><span data-stu-id="06b81-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06b81-138">请求</span><span class="sxs-lookup"><span data-stu-id="06b81-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_adminconsentrequestpolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy
```

### <a name="response"></a><span data-ttu-id="06b81-139">响应</span><span class="sxs-lookup"><span data-stu-id="06b81-139">Response</span></span>

<span data-ttu-id="06b81-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="06b81-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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
