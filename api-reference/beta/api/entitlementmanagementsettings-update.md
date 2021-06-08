---
title: 更新 entitlementManagementSettings
description: 更新 entitlementManagementSettings 对象以更改其一个或多个属性。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f1b95cf9fdeb38d998fcd153d36611e5e0d43328
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787012"
---
# <a name="update-entitlementmanagementsettings"></a><span data-ttu-id="044c2-103">更新 entitlementManagementSettings</span><span class="sxs-lookup"><span data-stu-id="044c2-103">Update entitlementManagementSettings</span></span>

<span data-ttu-id="044c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="044c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="044c2-105">更新现有 [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) 对象以更改其一个或多个属性。</span><span class="sxs-lookup"><span data-stu-id="044c2-105">Update an existing [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object to change one or more of its properties.</span></span>


## <a name="permissions"></a><span data-ttu-id="044c2-106">权限</span><span class="sxs-lookup"><span data-stu-id="044c2-106">Permissions</span></span>
<span data-ttu-id="044c2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="044c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="044c2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="044c2-109">Permission type</span></span>                        | <span data-ttu-id="044c2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="044c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="044c2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="044c2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="044c2-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="044c2-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="044c2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="044c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="044c2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="044c2-114">Not supported.</span></span> |
|<span data-ttu-id="044c2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="044c2-115">Application</span></span>                            | <span data-ttu-id="044c2-116">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="044c2-116">EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="044c2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="044c2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a><span data-ttu-id="044c2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="044c2-118">Request headers</span></span>
| <span data-ttu-id="044c2-119">名称</span><span class="sxs-lookup"><span data-stu-id="044c2-119">Name</span></span>         | <span data-ttu-id="044c2-120">说明</span><span class="sxs-lookup"><span data-stu-id="044c2-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="044c2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="044c2-121">Authorization</span></span> | <span data-ttu-id="044c2-p102">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="044c2-p102">Bearer \{token\}. Required.</span></span> |
| <span data-ttu-id="044c2-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="044c2-124">Content-Type</span></span>  | <span data-ttu-id="044c2-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="044c2-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="044c2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="044c2-127">Request body</span></span>
<span data-ttu-id="044c2-128">在请求正文中，提供 [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) 对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="044c2-128">In the request body, supply a JSON representation of the parameters of an [entitlementManagementSettings](../resources/entitlementmanagementsettings.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="044c2-129">响应</span><span class="sxs-lookup"><span data-stu-id="044c2-129">Response</span></span>
<span data-ttu-id="044c2-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="044c2-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="044c2-131">示例</span><span class="sxs-lookup"><span data-stu-id="044c2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="044c2-132">请求</span><span class="sxs-lookup"><span data-stu-id="044c2-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="044c2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="044c2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_entitlementManagementSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
Content-type: application/json

{
  "externalUserLifecycleAction": "None"
}
```
# <a name="c"></a>[<span data-ttu-id="044c2-134">C#</span><span class="sxs-lookup"><span data-stu-id="044c2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="044c2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="044c2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="044c2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="044c2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="044c2-137">Java</span><span class="sxs-lookup"><span data-stu-id="044c2-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="044c2-138">响应</span><span class="sxs-lookup"><span data-stu-id="044c2-138">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


