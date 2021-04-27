---
title: 列出 accessPackageResourceRoleScopes
description: 检索 accesspackageresourcerolescope 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d2376d9eb4aaf0bd8ab58b0dd5cbbb131e36a01c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038633"
---
# <a name="list-accesspackageresourcerolescopes"></a><span data-ttu-id="3577a-103">列出 accessPackageResourceRoleScopes</span><span class="sxs-lookup"><span data-stu-id="3577a-103">List accessPackageResourceRoleScopes</span></span>

<span data-ttu-id="3577a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3577a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3577a-105">检索包含 [accessPackageResourceRoleScope 对象列表的访问](../resources/accesspackageresourcerolescope.md) 包。</span><span class="sxs-lookup"><span data-stu-id="3577a-105">Retrieve an access package with a list of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects.</span></span>  <span data-ttu-id="3577a-106">每个对象链接到 [一个 accessPackageResourceRole](../resources/accesspackageresourcerole.md) 和 [一个 accessPackageResourceScope](../resources/accesspackageresourcescope.md)。</span><span class="sxs-lookup"><span data-stu-id="3577a-106">Each object links to an [accessPackageResourceRole](../resources/accesspackageresourcerole.md) and an [accessPackageResourceScope](../resources/accesspackageresourcescope.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3577a-107">权限</span><span class="sxs-lookup"><span data-stu-id="3577a-107">Permissions</span></span>

<span data-ttu-id="3577a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3577a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3577a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3577a-110">Permission type</span></span>                        | <span data-ttu-id="3577a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3577a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3577a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3577a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3577a-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3577a-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3577a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3577a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3577a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3577a-115">Not supported.</span></span> |
| <span data-ttu-id="3577a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3577a-116">Application</span></span>                            | <span data-ttu-id="3577a-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3577a-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3577a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3577a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3577a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3577a-119">Optional query parameters</span></span>

<span data-ttu-id="3577a-120">此方法使用 OData 查询参数自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3577a-120">This method uses OData query parameters to customize the response.</span></span> <span data-ttu-id="3577a-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3577a-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3577a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="3577a-122">Request headers</span></span>

| <span data-ttu-id="3577a-123">名称</span><span class="sxs-lookup"><span data-stu-id="3577a-123">Name</span></span>      |<span data-ttu-id="3577a-124">说明</span><span class="sxs-lookup"><span data-stu-id="3577a-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3577a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="3577a-125">Authorization</span></span> | <span data-ttu-id="3577a-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="3577a-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3577a-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="3577a-128">Request body</span></span>

<span data-ttu-id="3577a-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3577a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3577a-130">响应</span><span class="sxs-lookup"><span data-stu-id="3577a-130">Response</span></span>

<span data-ttu-id="3577a-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` 包含[accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md)对象集合的[accessPackage。](../resources/accesspackage.md)</span><span class="sxs-lookup"><span data-stu-id="3577a-131">If successful, this method returns a `200 OK` response code and an [accessPackage](../resources/accesspackage.md) containing a collection of [accessPackageResourceRoleScope](../resources/accesspackageresourcerolescope.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3577a-132">示例</span><span class="sxs-lookup"><span data-stu-id="3577a-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3577a-133">请求</span><span class="sxs-lookup"><span data-stu-id="3577a-133">Request</span></span>

<span data-ttu-id="3577a-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3577a-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3577a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="3577a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcerolescopes"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}?$expand=accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)
```
# <a name="c"></a>[<span data-ttu-id="3577a-136">C#</span><span class="sxs-lookup"><span data-stu-id="3577a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresourcerolescopes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3577a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3577a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresourcerolescopes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3577a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3577a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresourcerolescopes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3577a-139">Java</span><span class="sxs-lookup"><span data-stu-id="3577a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresourcerolescopes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3577a-140">响应</span><span class="sxs-lookup"><span data-stu-id="3577a-140">Response</span></span>

<span data-ttu-id="3577a-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3577a-141">The following is an example of the response.</span></span>

> <span data-ttu-id="3577a-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3577a-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


