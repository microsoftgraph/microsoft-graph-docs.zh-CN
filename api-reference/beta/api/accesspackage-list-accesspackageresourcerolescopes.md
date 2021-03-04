---
title: 列出 accessPackageResourceRoleScopes
description: 检索 accesspackageresourcerolescope 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 82a70b30c7669cecc209b5a129dbfaeba5a89f8b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439819"
---
# <a name="list-accesspackageresourcerolescopes"></a><span data-ttu-id="251e8-103">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="251e8-103">List accessPackageResourceRoleScopes</span></span>

<span data-ttu-id="251e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="251e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="251e8-105">检索包含 [accessPackageResourceRoleScope 对象列表的访问](../resources/accesspackageresourcerolescope.md) 包。</span><span class="sxs-lookup"><span data-stu-id="251e8-105">Retrieve an access package with a list of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.</span></span>  <span data-ttu-id="251e8-106">每个对象链接到 [一个 accessPackageResourceRole](../resources/accesspackageresourcerole.md) 和 [一个 accessPackageResourceScope](../resources/accesspackageresourcescope.md)。</span><span class="sxs-lookup"><span data-stu-id="251e8-106">Each object links to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="251e8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="251e8-107">Permissions</span></span>

<span data-ttu-id="251e8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="251e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="251e8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="251e8-110">Permission type</span></span>                        | <span data-ttu-id="251e8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="251e8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="251e8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="251e8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="251e8-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="251e8-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="251e8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="251e8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="251e8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="251e8-115">Not supported.</span></span> |
| <span data-ttu-id="251e8-116">Application</span><span class="sxs-lookup"><span data-stu-id="251e8-116">Application</span></span>                            | <span data-ttu-id="251e8-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="251e8-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="251e8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="251e8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="251e8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="251e8-119">Optional query parameters</span></span>

<span data-ttu-id="251e8-120">此方法使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="251e8-120">This method uses OData query parameters to customize the response.</span></span> <span data-ttu-id="251e8-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="251e8-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="251e8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="251e8-122">Request headers</span></span>

| <span data-ttu-id="251e8-123">名称</span><span class="sxs-lookup"><span data-stu-id="251e8-123">Name</span></span>      |<span data-ttu-id="251e8-124">说明</span><span class="sxs-lookup"><span data-stu-id="251e8-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="251e8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="251e8-125">Authorization</span></span> | <span data-ttu-id="251e8-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="251e8-126">Bearer \{token\}.</span></span> <span data-ttu-id="251e8-127">必需。</span><span class="sxs-lookup"><span data-stu-id="251e8-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="251e8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="251e8-128">Request body</span></span>

<span data-ttu-id="251e8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="251e8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="251e8-130">响应</span><span class="sxs-lookup"><span data-stu-id="251e8-130">Response</span></span>

<span data-ttu-id="251e8-131">如果成功，此方法在响应正文中返回包含 `200 OK` [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)对象集合的响应代码和[accessPackage。](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="251e8-131">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) containing a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="251e8-132">示例</span><span class="sxs-lookup"><span data-stu-id="251e8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="251e8-133">请求</span><span class="sxs-lookup"><span data-stu-id="251e8-133">Request</span></span>

<span data-ttu-id="251e8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="251e8-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="251e8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="251e8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescopes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```
# <a name="c"></a>[<span data-ttu-id="251e8-136">C#</span><span class="sxs-lookup"><span data-stu-id="251e8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerolescopes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="251e8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="251e8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerolescopes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="251e8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="251e8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerolescopes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="251e8-139">Java</span><span class="sxs-lookup"><span data-stu-id="251e8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourcerolescopes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="251e8-140">响应</span><span class="sxs-lookup"><span data-stu-id="251e8-140">Response</span></span>

<span data-ttu-id="251e8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="251e8-141">The following is an example of the response.</span></span>

> <span data-ttu-id="251e8-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="251e8-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "id": "933a4822-aed1-445b-9623-62116cd07a39",
    "catalogId": "32efb28c-9a7a-446c-986b-ca6528c6669d",
    "displayName": "Test Package 9-9",
    "description": "Test Package 9-9",
    "isHidden": false,
    "accessPackageResourceRoleScopes": [
        {
            "id": "70113acf-4dcb-453f-b517-2394598d974e_22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
            "createdBy": "alice@contoso.com",
            "createdDateTime": "2019-09-09T19:54:14.853Z",
            "modifiedBy": "alice@contoso.com",
            "modifiedDateTime": "2019-09-09T19:54:14.853Z",
            "accessPackageResourceRole": {
                "id": "70113acf-4dcb-453f-b517-2394598d974e",
                "displayName": "Owner",
                "originSystem": "origin-type",
                "originId": "Owner_7b56ede0-9b58-40bd-b11e-b3d18fc32698"
            },
            "accessPackageResourceScope": {
                "id": "22bfd707-ab6f-404f-b0b5-a5e6f5d0ba36",
                "displayName": "Root",
                "description": "Root Scope",
                "originId": "7b56ede0-9b58-40bd-b11e-b3d18fc32698",
                "originSystem": "origin-type",
                "isRootScope": true
            }
        }
    ]
}

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResourceRoleScopes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


