---
title: 创建 accessPackage
description: 创建新的 accessPackage。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1a415978968b4fa03133de156702ead1c473f1a1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439770"
---
# <a name="create-accesspackage"></a><span data-ttu-id="f10a9-103">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="f10a9-103">Create accessPackage</span></span>

<span data-ttu-id="f10a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f10a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f10a9-105">创建新的 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f10a9-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f10a9-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f10a9-106">Permissions</span></span>

<span data-ttu-id="f10a9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f10a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f10a9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f10a9-109">Permission type</span></span>                        | <span data-ttu-id="f10a9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f10a9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f10a9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f10a9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f10a9-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10a9-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f10a9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f10a9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f10a9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f10a9-114">Not supported.</span></span> |
| <span data-ttu-id="f10a9-115">Application</span><span class="sxs-lookup"><span data-stu-id="f10a9-115">Application</span></span>                            | <span data-ttu-id="f10a9-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10a9-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f10a9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f10a9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="f10a9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f10a9-118">Request headers</span></span>

| <span data-ttu-id="f10a9-119">名称</span><span class="sxs-lookup"><span data-stu-id="f10a9-119">Name</span></span>          | <span data-ttu-id="f10a9-120">说明</span><span class="sxs-lookup"><span data-stu-id="f10a9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f10a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f10a9-121">Authorization</span></span> | <span data-ttu-id="f10a9-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="f10a9-122">Bearer \{token\}.</span></span> <span data-ttu-id="f10a9-123">必需。</span><span class="sxs-lookup"><span data-stu-id="f10a9-123">Required.</span></span> |
| <span data-ttu-id="f10a9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f10a9-124">Content-Type</span></span>  | <span data-ttu-id="f10a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f10a9-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f10a9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f10a9-126">Request body</span></span>

<span data-ttu-id="f10a9-127">在请求正文中，提供 [accessPackage](../resources/accesspackage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f10a9-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f10a9-128">响应</span><span class="sxs-lookup"><span data-stu-id="f10a9-128">Response</span></span>

<span data-ttu-id="f10a9-129">如果成功，此方法在响应正文中返回 201 创建的响应代码和新 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f10a9-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f10a9-130">示例</span><span class="sxs-lookup"><span data-stu-id="f10a9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f10a9-131">请求</span><span class="sxs-lookup"><span data-stu-id="f10a9-131">Request</span></span>

<span data-ttu-id="f10a9-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f10a9-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f10a9-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f10a9-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackage_from_accesspackages"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages
Content-type: application/json

{
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives"
}
```
# <a name="c"></a>[<span data-ttu-id="f10a9-134">C#</span><span class="sxs-lookup"><span data-stu-id="f10a9-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f10a9-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f10a9-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f10a9-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f10a9-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f10a9-137">Java</span><span class="sxs-lookup"><span data-stu-id="f10a9-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f10a9-138">响应</span><span class="sxs-lookup"><span data-stu-id="f10a9-138">Response</span></span>

<span data-ttu-id="f10a9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f10a9-139">The following is an example of the response.</span></span>

> <span data-ttu-id="f10a9-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f10a9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "56ff43fd-6b05-48df-9634-956a777fce6d",
  "catalogId": "aa2f6514-3232-46e7-a08a-2411ad8d7128",
  "displayName": "sales reps",
  "description": "outside sales representatives",
  "isHidden": false,
  "isRoleScopesVisible": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


