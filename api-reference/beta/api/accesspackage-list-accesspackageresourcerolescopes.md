---
title: 列出 accessPackageResourceRoleScopes
description: 检索 accesspackageresourcerolescope 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee39c846fc40a89d28490c4ee5782a9f75b68f18
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994185"
---
# <a name="list-accesspackageresourcerolescopes"></a><span data-ttu-id="caa30-103">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="caa30-103">List accessPackageResourceRoleScopes</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="caa30-104">检索包含[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)对象列表的 access 程序包。</span><span class="sxs-lookup"><span data-stu-id="caa30-104">Retrieve an access package with a list of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.</span></span>  <span data-ttu-id="caa30-105">每个对象链接到[accessPackageResourceRole](../resources/accesspackageresourcerole.md)和[accessPackageResourceScope](../resources/accesspackageresourcescope.md)。</span><span class="sxs-lookup"><span data-stu-id="caa30-105">Each object links to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="caa30-106">权限</span><span class="sxs-lookup"><span data-stu-id="caa30-106">Permissions</span></span>

<span data-ttu-id="caa30-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="caa30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="caa30-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="caa30-109">Permission type</span></span>                        | <span data-ttu-id="caa30-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="caa30-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="caa30-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="caa30-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="caa30-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="caa30-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="caa30-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="caa30-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="caa30-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="caa30-114">Not supported.</span></span> |
| <span data-ttu-id="caa30-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="caa30-115">Application</span></span>                            | <span data-ttu-id="caa30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="caa30-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="caa30-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="caa30-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="caa30-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="caa30-118">Optional query parameters</span></span>

<span data-ttu-id="caa30-119">此方法使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="caa30-119">This method uses OData query parameters to customize the response.</span></span> <span data-ttu-id="caa30-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="caa30-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="caa30-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="caa30-121">Request headers</span></span>

| <span data-ttu-id="caa30-122">名称</span><span class="sxs-lookup"><span data-stu-id="caa30-122">Name</span></span>      |<span data-ttu-id="caa30-123">说明</span><span class="sxs-lookup"><span data-stu-id="caa30-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="caa30-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="caa30-124">Authorization</span></span> | <span data-ttu-id="caa30-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="caa30-125">Bearer \{token\}.</span></span> <span data-ttu-id="caa30-126">必填。</span><span class="sxs-lookup"><span data-stu-id="caa30-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="caa30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="caa30-127">Request body</span></span>

<span data-ttu-id="caa30-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="caa30-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="caa30-129">响应</span><span class="sxs-lookup"><span data-stu-id="caa30-129">Response</span></span>

<span data-ttu-id="caa30-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和包含[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)对象集合的[accessPackage](../resources/accesspackage.md) 。</span><span class="sxs-lookup"><span data-stu-id="caa30-130">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) containing a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="caa30-131">示例</span><span class="sxs-lookup"><span data-stu-id="caa30-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="caa30-132">请求</span><span class="sxs-lookup"><span data-stu-id="caa30-132">Request</span></span>

<span data-ttu-id="caa30-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="caa30-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="caa30-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="caa30-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescopes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="caa30-135">C#</span><span class="sxs-lookup"><span data-stu-id="caa30-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerolescopes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="caa30-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="caa30-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerolescopes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="caa30-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="caa30-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerolescopes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="caa30-138">响应</span><span class="sxs-lookup"><span data-stu-id="caa30-138">Response</span></span>

<span data-ttu-id="caa30-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="caa30-139">The following is an example of the response.</span></span>

> <span data-ttu-id="caa30-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="caa30-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
