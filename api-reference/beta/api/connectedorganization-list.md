---
title: 列出 connectedOrganizations
description: 检索 connectedOrganization 对象的列表。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9475026b2bf4ea5c2f2ec4c0b539850c52938ec5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957665"
---
# <a name="list-connectedorganizations"></a><span data-ttu-id="a3ef4-103">列出 connectedOrganizations</span><span class="sxs-lookup"><span data-stu-id="a3ef4-103">List connectedOrganizations</span></span>

<span data-ttu-id="a3ef4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3ef4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3ef4-105">检索 [connectedOrganization](../resources/connectedorganization.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-105">Retrieve a list of [connectedOrganization](../resources/connectedorganization.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3ef4-106">权限</span><span class="sxs-lookup"><span data-stu-id="a3ef4-106">Permissions</span></span>

<span data-ttu-id="a3ef4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ef4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3ef4-109">Permission type</span></span>|<span data-ttu-id="a3ef4-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a3ef4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
| <span data-ttu-id="a3ef4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ef4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a3ef4-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="a3ef4-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="a3ef4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ef4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3ef4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-114">Not supported.</span></span> |
| <span data-ttu-id="a3ef4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3ef4-115">Application</span></span>                            | <span data-ttu-id="a3ef4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3ef4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3ef4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/connectedOrganizations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a3ef4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a3ef4-118">Optional query parameters</span></span>
<span data-ttu-id="a3ef4-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a3ef4-120">例如，若要仅检索具有特定显示名称的已连接组织，请添加 `$filter=displayName eq 'Name'` 。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-120">For example, to retrieve only the connected organizations with a specific display name, add `$filter=displayName eq 'Name'`.</span></span> <span data-ttu-id="a3ef4-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3ef4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3ef4-122">Request headers</span></span>
|<span data-ttu-id="a3ef4-123">名称</span><span class="sxs-lookup"><span data-stu-id="a3ef4-123">Name</span></span>|<span data-ttu-id="a3ef4-124">说明</span><span class="sxs-lookup"><span data-stu-id="a3ef4-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a3ef4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3ef4-125">Authorization</span></span>|<span data-ttu-id="a3ef4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3ef4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3ef4-128">Request body</span></span>
<span data-ttu-id="a3ef4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3ef4-130">响应</span><span class="sxs-lookup"><span data-stu-id="a3ef4-130">Response</span></span>

<span data-ttu-id="a3ef4-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [connectedOrganization](../resources/connectedorganization.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-131">If successful, this method returns a `200 OK` response code and a collection of [connectedOrganization](../resources/connectedorganization.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a3ef4-132">示例</span><span class="sxs-lookup"><span data-stu-id="a3ef4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a3ef4-133">请求</span><span class="sxs-lookup"><span data-stu-id="a3ef4-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a3ef4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a3ef4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectedorganizations"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/connectedOrganizations
```
# <a name="c"></a>[<span data-ttu-id="a3ef4-135">C#</span><span class="sxs-lookup"><span data-stu-id="a3ef4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectedorganizations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a3ef4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a3ef4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectedorganizations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a3ef4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a3ef4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectedorganizations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a3ef4-138">Java</span><span class="sxs-lookup"><span data-stu-id="a3ef4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectedorganizations-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a3ef4-139">响应</span><span class="sxs-lookup"><span data-stu-id="a3ef4-139">Response</span></span>
<span data-ttu-id="a3ef4-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a3ef4-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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


