---
title: 获取 accessPackage
description: 检索 accessPackage 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6324c868a4c78f108a8eb8177b70504d9129d8d7
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345199"
---
# <a name="get-accesspackage"></a><span data-ttu-id="b75db-103">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="b75db-103">Get accessPackage</span></span>

<span data-ttu-id="b75db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b75db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b75db-105">检索[accessPackage](../resources/accesspackage.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b75db-105">Retrieve the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b75db-106">权限</span><span class="sxs-lookup"><span data-stu-id="b75db-106">Permissions</span></span>

<span data-ttu-id="b75db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b75db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b75db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b75db-109">Permission type</span></span>                        | <span data-ttu-id="b75db-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b75db-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b75db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b75db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b75db-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="b75db-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="b75db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b75db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b75db-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b75db-114">Not supported.</span></span> |
| <span data-ttu-id="b75db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b75db-115">Application</span></span>                            | <span data-ttu-id="b75db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b75db-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b75db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b75db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b75db-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b75db-118">Optional query parameters</span></span>

<span data-ttu-id="b75db-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b75db-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="b75db-120">例如，若要检索访问包策略，请添加 `$expand=accessPackageAssignmentPolicies` 。</span><span class="sxs-lookup"><span data-stu-id="b75db-120">For example, to retrieve the access package policies, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="b75db-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b75db-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b75db-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="b75db-122">Request headers</span></span>

| <span data-ttu-id="b75db-123">名称</span><span class="sxs-lookup"><span data-stu-id="b75db-123">Name</span></span>      |<span data-ttu-id="b75db-124">说明</span><span class="sxs-lookup"><span data-stu-id="b75db-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b75db-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b75db-125">Authorization</span></span> | <span data-ttu-id="b75db-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="b75db-126">Bearer \{token\}.</span></span> <span data-ttu-id="b75db-127">必填。</span><span class="sxs-lookup"><span data-stu-id="b75db-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b75db-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b75db-128">Request body</span></span>

<span data-ttu-id="b75db-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b75db-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b75db-130">响应</span><span class="sxs-lookup"><span data-stu-id="b75db-130">Response</span></span>

<span data-ttu-id="b75db-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[accessPackage](../resources/accesspackage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b75db-131">If successful, this method returns a `200 OK` response code and the requested [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b75db-132">示例</span><span class="sxs-lookup"><span data-stu-id="b75db-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b75db-133">请求</span><span class="sxs-lookup"><span data-stu-id="b75db-133">Request</span></span>

<span data-ttu-id="b75db-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b75db-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b75db-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b75db-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="b75db-136">C#</span><span class="sxs-lookup"><span data-stu-id="b75db-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b75db-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b75db-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b75db-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b75db-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b75db-139">响应</span><span class="sxs-lookup"><span data-stu-id="b75db-139">Response</span></span>

<span data-ttu-id="b75db-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b75db-140">The following is an example of the response.</span></span>

> <span data-ttu-id="b75db-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b75db-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
