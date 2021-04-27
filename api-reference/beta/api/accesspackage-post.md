---
title: 创建 accessPackage
description: 创建新的 accessPackage。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e6f6a80316bbdf12792bb47078be7f4e3ca9b48c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048643"
---
# <a name="create-accesspackage"></a><span data-ttu-id="4f80d-103">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="4f80d-103">Create accessPackage</span></span>

<span data-ttu-id="4f80d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f80d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f80d-105">创建新的 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f80d-105">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f80d-106">权限</span><span class="sxs-lookup"><span data-stu-id="4f80d-106">Permissions</span></span>

<span data-ttu-id="4f80d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f80d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f80d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f80d-109">Permission type</span></span>                        | <span data-ttu-id="4f80d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4f80d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4f80d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f80d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f80d-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f80d-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="4f80d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f80d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f80d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f80d-114">Not supported.</span></span> |
| <span data-ttu-id="4f80d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4f80d-115">Application</span></span>                            | <span data-ttu-id="4f80d-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f80d-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4f80d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f80d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="4f80d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f80d-118">Request headers</span></span>

| <span data-ttu-id="4f80d-119">名称</span><span class="sxs-lookup"><span data-stu-id="4f80d-119">Name</span></span>          | <span data-ttu-id="4f80d-120">说明</span><span class="sxs-lookup"><span data-stu-id="4f80d-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4f80d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f80d-121">Authorization</span></span> | <span data-ttu-id="4f80d-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="4f80d-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="4f80d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4f80d-124">Content-Type</span></span>  | <span data-ttu-id="4f80d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f80d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4f80d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f80d-126">Request body</span></span>

<span data-ttu-id="4f80d-127">在请求正文中，提供 [accessPackage](../resources/accesspackage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f80d-127">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4f80d-128">响应</span><span class="sxs-lookup"><span data-stu-id="4f80d-128">Response</span></span>

<span data-ttu-id="4f80d-129">如果成功，此方法在响应正文中返回 201 Created 响应代码和新 [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4f80d-129">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4f80d-130">示例</span><span class="sxs-lookup"><span data-stu-id="4f80d-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4f80d-131">请求</span><span class="sxs-lookup"><span data-stu-id="4f80d-131">Request</span></span>

<span data-ttu-id="4f80d-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4f80d-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4f80d-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4f80d-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4f80d-134">C#</span><span class="sxs-lookup"><span data-stu-id="4f80d-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4f80d-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4f80d-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4f80d-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4f80d-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4f80d-137">Java</span><span class="sxs-lookup"><span data-stu-id="4f80d-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accesspackage-from-accesspackages-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4f80d-138">响应</span><span class="sxs-lookup"><span data-stu-id="4f80d-138">Response</span></span>

<span data-ttu-id="4f80d-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4f80d-139">The following is an example of the response.</span></span>

> <span data-ttu-id="4f80d-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4f80d-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


