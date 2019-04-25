---
title: 列出 trustFrameworkPolicies
description: 此操作列出了 Azure AD B2C 租户中的所有 trustFrameworkPolicy 对象。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 873fe9de84ec58ded43141668dd3681409032e56
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536710"
---
# <a name="list-trustframeworkpolicies"></a><span data-ttu-id="4e3d3-103">列出 trustFrameworkPolicies</span><span class="sxs-lookup"><span data-stu-id="4e3d3-103">List trustFrameworkPolicies</span></span>

> <span data-ttu-id="4e3d3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e3d3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e3d3-106">检索租户/目录中的[trustFrameworkPolicies](../resources/trustframeworkpolicy.md)列表。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-106">Retrieve a list of [trustFrameworkPolicies](../resources/trustframeworkpolicy.md) in the tenant/directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e3d3-107">权限</span><span class="sxs-lookup"><span data-stu-id="4e3d3-107">Permissions</span></span>

<span data-ttu-id="4e3d3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="4e3d3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e3d3-110">Permission type</span></span>      | <span data-ttu-id="4e3d3-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e3d3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e3d3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e3d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e3d3-113">TrustFramework、policy、read. All</span><span class="sxs-lookup"><span data-stu-id="4e3d3-113">Policy.Read.TrustFramework, Policy.Read.All</span></span>|
|<span data-ttu-id="4e3d3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e3d3-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4e3d3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-115">Not supported.</span></span>|
|<span data-ttu-id="4e3d3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e3d3-116">Application</span></span>|<span data-ttu-id="4e3d3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-117">Not supported.</span></span>|

<span data-ttu-id="4e3d3-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="4e3d3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e3d3-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /trustFramework/policies/
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4e3d3-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4e3d3-120">Optional query parameters</span></span>

<span data-ttu-id="4e3d3-121">此方法支持`$select`和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-121">This method supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e3d3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e3d3-122">Request headers</span></span>

|<span data-ttu-id="4e3d3-123">名称</span><span class="sxs-lookup"><span data-stu-id="4e3d3-123">Name</span></span>|<span data-ttu-id="4e3d3-124">说明</span><span class="sxs-lookup"><span data-stu-id="4e3d3-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4e3d3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e3d3-125">Authorization</span></span>|<span data-ttu-id="4e3d3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e3d3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e3d3-128">Request body</span></span>

<span data-ttu-id="4e3d3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e3d3-130">响应</span><span class="sxs-lookup"><span data-stu-id="4e3d3-130">Response</span></span>

<span data-ttu-id="4e3d3-131">如果成功, 此方法在响应`200 OK`正文的 JSON 表示形式中返回响应代码和[trustFrameworkPolicy](../resources/trustframeworkpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-131">If successful, this method returns a `200 OK` response code and a collection of [trustFrameworkPolicy](../resources/trustframeworkpolicy.md) objects in a JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e3d3-132">示例</span><span class="sxs-lookup"><span data-stu-id="4e3d3-132">Example</span></span>

<span data-ttu-id="4e3d3-133">下面的示例检索所有**trustFrameworkPolicies**。</span><span class="sxs-lookup"><span data-stu-id="4e3d3-133">The following example retrieves all **trustFrameworkPolicies**.</span></span>

##### <a name="request"></a><span data-ttu-id="4e3d3-134">请求</span><span class="sxs-lookup"><span data-stu-id="4e3d3-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get__trustFrameworks"
}-->
```http
GET https://graph.microsoft.com/beta/trustFramework/policies
```

##### <a name="response"></a><span data-ttu-id="4e3d3-135">响应</span><span class="sxs-lookup"><span data-stu-id="4e3d3-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFramework.policy",
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
  "tocPath": ""
}-->
