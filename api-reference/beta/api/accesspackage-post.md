---
title: 创建 accessPackage
description: 创建新的 accessPackage。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a70de297dcd22588914d8613635687f07aaf40b0
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994114"
---
# <a name="create-accesspackage"></a><span data-ttu-id="6399f-103">创建 accessPackage</span><span class="sxs-lookup"><span data-stu-id="6399f-103">Create accessPackage</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6399f-104">创建新的[accessPackage](../resources/accesspackage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6399f-104">Create a new [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6399f-105">权限</span><span class="sxs-lookup"><span data-stu-id="6399f-105">Permissions</span></span>

<span data-ttu-id="6399f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6399f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6399f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6399f-108">Permission type</span></span>                        | <span data-ttu-id="6399f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6399f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6399f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6399f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6399f-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6399f-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6399f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6399f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6399f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6399f-113">Not supported.</span></span> |
| <span data-ttu-id="6399f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="6399f-114">Application</span></span>                            | <span data-ttu-id="6399f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6399f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6399f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6399f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackages
```

## <a name="request-headers"></a><span data-ttu-id="6399f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="6399f-117">Request headers</span></span>

| <span data-ttu-id="6399f-118">名称</span><span class="sxs-lookup"><span data-stu-id="6399f-118">Name</span></span>          | <span data-ttu-id="6399f-119">说明</span><span class="sxs-lookup"><span data-stu-id="6399f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6399f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6399f-120">Authorization</span></span> | <span data-ttu-id="6399f-121">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="6399f-121">Bearer \{token\}.</span></span> <span data-ttu-id="6399f-122">必填。</span><span class="sxs-lookup"><span data-stu-id="6399f-122">Required.</span></span> |
| <span data-ttu-id="6399f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6399f-123">Content-Type</span></span>  | <span data-ttu-id="6399f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6399f-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6399f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6399f-125">Request body</span></span>

<span data-ttu-id="6399f-126">在请求正文中，提供[accessPackage](../resources/accesspackage.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6399f-126">In the request body, supply a JSON representation of [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6399f-127">响应</span><span class="sxs-lookup"><span data-stu-id="6399f-127">Response</span></span>

<span data-ttu-id="6399f-128">如果成功，此方法在响应正文中返回一个201创建的响应代码和一个新的[accessPackage](../resources/accesspackage.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6399f-128">If successful, this method returns a 201 Created response code and a new [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6399f-129">示例</span><span class="sxs-lookup"><span data-stu-id="6399f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6399f-130">请求</span><span class="sxs-lookup"><span data-stu-id="6399f-130">Request</span></span>

<span data-ttu-id="6399f-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6399f-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6399f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6399f-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6399f-133">C#</span><span class="sxs-lookup"><span data-stu-id="6399f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackage-from-accesspackages-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6399f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6399f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackage-from-accesspackages-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6399f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6399f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackage-from-accesspackages-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6399f-136">响应</span><span class="sxs-lookup"><span data-stu-id="6399f-136">Response</span></span>

<span data-ttu-id="6399f-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6399f-137">The following is an example of the response.</span></span>

> <span data-ttu-id="6399f-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6399f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
