---
title: 列出 servicePrincipal 的 delegatedPermissionClassifications 集合
description: 检索为 API 的服务主体公开的委派权限给定的分类列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: fdf42339adea9441ff0378fe26cce2063062eb82
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054446"
---
# <a name="list-delegatedpermissionclassifications-collection-of-serviceprincipal"></a><span data-ttu-id="f9278-103">列出 servicePrincipal 的 delegatedPermissionClassifications 集合</span><span class="sxs-lookup"><span data-stu-id="f9278-103">List delegatedPermissionClassifications collection of servicePrincipal</span></span>

<span data-ttu-id="f9278-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9278-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f9278-105">检索当前为 API 公开的委派权限配置的 [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="f9278-105">Retrieve the list of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) currently configured for the delegated permissions exposed by an API.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9278-106">权限</span><span class="sxs-lookup"><span data-stu-id="f9278-106">Permissions</span></span>

<span data-ttu-id="f9278-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9278-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9278-109">Permission type</span></span>      | <span data-ttu-id="f9278-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f9278-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9278-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9278-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f9278-112">Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9278-112">Application.Read.All, Directory.Read.All</span></span> |
|<span data-ttu-id="f9278-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9278-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9278-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9278-114">Not supported.</span></span>    |
|<span data-ttu-id="f9278-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9278-115">Application</span></span> | <span data-ttu-id="f9278-116">Application.Read.OwnedBy、Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9278-116">Application.Read.OwnedBy, Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f9278-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9278-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/delegatedPermissionClassifications
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f9278-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f9278-118">Optional query parameters</span></span>

<span data-ttu-id="f9278-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f9278-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f9278-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9278-120">Request headers</span></span>

| <span data-ttu-id="f9278-121">名称</span><span class="sxs-lookup"><span data-stu-id="f9278-121">Name</span></span>           | <span data-ttu-id="f9278-122">说明</span><span class="sxs-lookup"><span data-stu-id="f9278-122">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="f9278-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9278-123">Authorization</span></span>  | <span data-ttu-id="f9278-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f9278-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f9278-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9278-126">Request body</span></span>

<span data-ttu-id="f9278-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9278-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9278-128">响应</span><span class="sxs-lookup"><span data-stu-id="f9278-128">Response</span></span>

<span data-ttu-id="f9278-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f9278-129">If successful, this method returns a `200 OK` response code and a collection of [delegatedPermissionClassification](../resources/delegatedpermissionclassification.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9278-130">示例</span><span class="sxs-lookup"><span data-stu-id="f9278-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9278-131">请求</span><span class="sxs-lookup"><span data-stu-id="f9278-131">Request</span></span>

<span data-ttu-id="f9278-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f9278-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f9278-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f9278-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_get_delegatedpermissionclassification"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications
```
# <a name="c"></a>[<span data-ttu-id="f9278-134">C#</span><span class="sxs-lookup"><span data-stu-id="f9278-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-get-delegatedpermissionclassification-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f9278-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f9278-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-get-delegatedpermissionclassification-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f9278-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f9278-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-get-delegatedpermissionclassification-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f9278-137">Java</span><span class="sxs-lookup"><span data-stu-id="f9278-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-get-delegatedpermissionclassification-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f9278-138">响应</span><span class="sxs-lookup"><span data-stu-id="f9278-138">Response</span></span>

<span data-ttu-id="f9278-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f9278-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f9278-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f9278-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.delegatedPermissionClassification",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "id": "2G3-4TG6YU2J54hjnaRoPQE",
        "permissionId": "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
        "permissionName": "User.Read",
        "classification": "low"
    }
  ]
}
```
