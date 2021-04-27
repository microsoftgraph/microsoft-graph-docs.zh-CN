---
title: 获取 entitlementManagementSettings
description: 检索 entitlementManagementSettings 对象的属性。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 398a0f75fd4cbf606cbc5c54c509ade4191fb9f2
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042623"
---
# <a name="get-entitlementmanagementsettings"></a><span data-ttu-id="9ffb7-103">获取 entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="9ffb7-103">Get entitlementManagementSettings</span></span>

<span data-ttu-id="9ffb7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ffb7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ffb7-105">检索 [entitlementManagementSettings 对象](../resources/entitlementManagementSettings.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-105">Retrieve the properties of an [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ffb7-106">权限</span><span class="sxs-lookup"><span data-stu-id="9ffb7-106">Permissions</span></span>

<span data-ttu-id="9ffb7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ffb7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ffb7-109">Permission type</span></span>                        | <span data-ttu-id="9ffb7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ffb7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ffb7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ffb7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ffb7-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffb7-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9ffb7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ffb7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ffb7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-114">Not supported.</span></span> |
| <span data-ttu-id="9ffb7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ffb7-115">Application</span></span>                            | <span data-ttu-id="9ffb7-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ffb7-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ffb7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ffb7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ffb7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9ffb7-118">Optional query parameters</span></span>

<span data-ttu-id="9ffb7-119">此运营商不支持通过 OData 查询参数 来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-119">This method does not support the OData query parameters to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ffb7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ffb7-120">Request headers</span></span>

| <span data-ttu-id="9ffb7-121">名称</span><span class="sxs-lookup"><span data-stu-id="9ffb7-121">Name</span></span>      |<span data-ttu-id="9ffb7-122">说明</span><span class="sxs-lookup"><span data-stu-id="9ffb7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ffb7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ffb7-123">Authorization</span></span> | <span data-ttu-id="9ffb7-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ffb7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ffb7-126">Request body</span></span>

<span data-ttu-id="9ffb7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ffb7-128">响应</span><span class="sxs-lookup"><span data-stu-id="9ffb7-128">Response</span></span>

<span data-ttu-id="9ffb7-129">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [entitlementManagementSettings](../resources/entitlementManagementSettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-129">If successful, this method returns a `200 OK` response code and the requested [entitlementManagementSettings](../resources/entitlementManagementSettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ffb7-130">示例</span><span class="sxs-lookup"><span data-stu-id="9ffb7-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9ffb7-131">请求</span><span class="sxs-lookup"><span data-stu-id="9ffb7-131">Request</span></span>

<span data-ttu-id="9ffb7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="9ffb7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ffb7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_entitlementManagementSettings"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
```
# <a name="c"></a>[<span data-ttu-id="9ffb7-134">C#</span><span class="sxs-lookup"><span data-stu-id="9ffb7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ffb7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ffb7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ffb7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ffb7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ffb7-137">Java</span><span class="sxs-lookup"><span data-stu-id="9ffb7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="9ffb7-138">响应</span><span class="sxs-lookup"><span data-stu-id="9ffb7-138">Response</span></span>

<span data-ttu-id="9ffb7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-139">The following is an example of the response.</span></span>

> <span data-ttu-id="9ffb7-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ffb7-140">**Note:** The response object shown here might be shortened for readability.</span></span>

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


