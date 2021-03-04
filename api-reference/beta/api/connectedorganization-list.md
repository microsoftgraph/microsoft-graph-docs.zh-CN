---
title: 列出 connectedOrganizations
description: 检索 connectedOrganization 对象的列表。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0d74b4624833ca8c6a9feecf824f6e4346ca952c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437441"
---
# <a name="list-connectedorganizations"></a><span data-ttu-id="f8525-103">列出 connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="f8525-103">List connectedOrganizations</span></span>

<span data-ttu-id="f8525-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8525-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8525-105">检索 [connectedOrganization 对象](../resources/connectedorganization.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="f8525-105">Retrieve a list of [connectedOrganization](../resources/connectedorganization.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8525-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f8525-106">Permissions</span></span>

<span data-ttu-id="f8525-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f8525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8525-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8525-109">Permission type</span></span>|<span data-ttu-id="f8525-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f8525-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="f8525-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8525-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8525-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8525-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f8525-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8525-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8525-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8525-114">Not supported.</span></span> |
| <span data-ttu-id="f8525-115">Application</span><span class="sxs-lookup"><span data-stu-id="f8525-115">Application</span></span>                            | <span data-ttu-id="f8525-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8525-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8525-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8525-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8525-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f8525-118">Optional query parameters</span></span>
<span data-ttu-id="f8525-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f8525-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f8525-120">例如，若要仅检索具有特定组织连接显示名称，请添加 `$filter=displayName eq 'Name'` 。</span><span class="sxs-lookup"><span data-stu-id="f8525-120">For example, to retrieve only the connected organizations with a specific display name, add `$filter=displayName eq 'Name'`.</span></span> <span data-ttu-id="f8525-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f8525-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8525-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8525-122">Request headers</span></span>
|<span data-ttu-id="f8525-123">名称</span><span class="sxs-lookup"><span data-stu-id="f8525-123">Name</span></span>|<span data-ttu-id="f8525-124">说明</span><span class="sxs-lookup"><span data-stu-id="f8525-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8525-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8525-125">Authorization</span></span>|<span data-ttu-id="f8525-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8525-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8525-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8525-128">Request body</span></span>
<span data-ttu-id="f8525-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f8525-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8525-130">响应</span><span class="sxs-lookup"><span data-stu-id="f8525-130">Response</span></span>

<span data-ttu-id="f8525-131">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [connectedOrganization](../resources/connectedorganization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f8525-131">If successful, this method returns a `200 OK` response code and a collection of [connectedOrganization](../resources/connectedorganization.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f8525-132">示例</span><span class="sxs-lookup"><span data-stu-id="f8525-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8525-133">请求</span><span class="sxs-lookup"><span data-stu-id="f8525-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f8525-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8525-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganizations"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations
```
# <a name="c"></a>[<span data-ttu-id="f8525-135">C#</span><span class="sxs-lookup"><span data-stu-id="f8525-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8525-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8525-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8525-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8525-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f8525-138">Java</span><span class="sxs-lookup"><span data-stu-id="f8525-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f8525-139">响应</span><span class="sxs-lookup"><span data-stu-id="f8525-139">Response</span></span>
<span data-ttu-id="f8525-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f8525-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.connectedOrganization)"
}
-->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "cd3709c6-be6a-4725-bd07-50f90ccca93f",
      "displayName": "Wingtip Toys",
      "description": "Wingtip Toys",
      "createdBy": "admin@contoso.com",
      "createdDateTime": "2020-05-13T15:18:04.81Z",
      "modifiedBy": "admin@contoso.com",
      "modifiedDateTime": "2020-05-13T15:18:04.81Z",
      "identitySources": [
        {
          "@odata.type": "#microsoft.graph.azureActiveDirectoryTenant",
          "tenantId": "bf85dc9d-cb43-44a4-80c4-469e8c58249e",
          "displayName": "Wingtip Toys Co"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List connectedOrganizations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


