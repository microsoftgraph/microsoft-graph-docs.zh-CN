---
title: 获取 entitlementManagementSettings
description: 检索 entitlementManagementSettings 对象的属性。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e84530e6354ba647ec522253e6dbef88afcded37
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955039"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="dcbaa-103">获取 entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="dcbaa-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="dcbaa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcbaa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcbaa-105">检索 [entitlementManagementSettings](../resources/entitlementManagementSettings.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcbaa-106">权限</span><span class="sxs-lookup"><span data-stu-id="dcbaa-106">Permissions</span></span>

<span data-ttu-id="dcbaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dcbaa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcbaa-109">Permission type</span></span>                        | <span data-ttu-id="dcbaa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcbaa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dcbaa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcbaa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dcbaa-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="dcbaa-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="dcbaa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcbaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcbaa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-114">Not supported.</span></span> |
| <span data-ttu-id="dcbaa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dcbaa-115">Application</span></span>                            | <span data-ttu-id="dcbaa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcbaa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcbaa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dcbaa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dcbaa-118">Optional query parameters</span></span>

<span data-ttu-id="dcbaa-119">此运营商不支持通过 OData 查询参数 来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dcbaa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcbaa-120">Request headers</span></span>

| <span data-ttu-id="dcbaa-121">名称</span><span class="sxs-lookup"><span data-stu-id="dcbaa-121">Name</span></span>      |<span data-ttu-id="dcbaa-122">说明</span><span class="sxs-lookup"><span data-stu-id="dcbaa-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dcbaa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcbaa-123">Authorization</span></span> | <span data-ttu-id="dcbaa-124">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-124">Bearer \{token\}.</span></span> <span data-ttu-id="dcbaa-125">必填。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcbaa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcbaa-126">Request body</span></span>

<span data-ttu-id="dcbaa-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcbaa-128">响应</span><span class="sxs-lookup"><span data-stu-id="dcbaa-128">Response</span></span>

<span data-ttu-id="dcbaa-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [entitlementManagementSettings](../resources/entitlementManagementSettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dcbaa-130">示例</span><span class="sxs-lookup"><span data-stu-id="dcbaa-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dcbaa-131">请求</span><span class="sxs-lookup"><span data-stu-id="dcbaa-131">Request</span></span>

<span data-ttu-id="dcbaa-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dcbaa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcbaa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```
# <a name="c"></a>[<span data-ttu-id="dcbaa-134">C#</span><span class="sxs-lookup"><span data-stu-id="dcbaa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcbaa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcbaa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcbaa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcbaa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcbaa-137">Java</span><span class="sxs-lookup"><span data-stu-id="dcbaa-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="dcbaa-138">响应</span><span class="sxs-lookup"><span data-stu-id="dcbaa-138">Response</span></span>

<span data-ttu-id="dcbaa-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-139">The following is an example of the response.</span></span>

> <span data-ttu-id="dcbaa-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dcbaa-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entitlementManagementSettings"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "externalUserLifecycleAction": "None",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


