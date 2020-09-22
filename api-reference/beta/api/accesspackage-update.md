---
title: 更新 accessPackage
description: 更新 accessPackage 对象的属性。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 04497ffcaeb8a7c738d18aff9e6668712cab4ace
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983926"
---
# <a name="update-accesspackage"></a><span data-ttu-id="5d4a0-103">更新 accessPackage</span><span class="sxs-lookup"><span data-stu-id="5d4a0-103">Update accessPackage</span></span>

<span data-ttu-id="5d4a0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d4a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d4a0-105">更新现有 [accessPackage](../resources/accesspackage.md) 对象以更改其一个或多个属性，如显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-105">Update an existing [accessPackage](../resources/accesspackage.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d4a0-106">权限</span><span class="sxs-lookup"><span data-stu-id="5d4a0-106">Permissions</span></span>
<span data-ttu-id="5d4a0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="5d4a0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d4a0-109">Permission type</span></span>|<span data-ttu-id="5d4a0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5d4a0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d4a0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d4a0-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5d4a0-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d4a0-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="5d4a0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d4a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d4a0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-114">Not supported.</span></span> |
|<span data-ttu-id="5d4a0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d4a0-115">Application</span></span>                            | <span data-ttu-id="5d4a0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d4a0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d4a0-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a><span data-ttu-id="5d4a0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d4a0-118">Request headers</span></span>
|<span data-ttu-id="5d4a0-119">名称</span><span class="sxs-lookup"><span data-stu-id="5d4a0-119">Name</span></span>|<span data-ttu-id="5d4a0-120">说明</span><span class="sxs-lookup"><span data-stu-id="5d4a0-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5d4a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d4a0-121">Authorization</span></span>|<span data-ttu-id="5d4a0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5d4a0-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d4a0-124">Content-Type</span></span>|<span data-ttu-id="5d4a0-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5d4a0-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d4a0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d4a0-127">Request body</span></span>
<span data-ttu-id="5d4a0-128">在请求正文中，提供 [accessPackage](../resources/accesspackage.md) 对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-128">In the request body, supply a JSON representation of the parameters of an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="5d4a0-129">下表显示了在更新 [accessPackage](../resources/accesspackage.md)时可提供的属性。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-129">The following table shows the properties that can be supplied when you update an [accessPackage](../resources/accesspackage.md).</span></span>

|<span data-ttu-id="5d4a0-130">属性</span><span class="sxs-lookup"><span data-stu-id="5d4a0-130">Property</span></span>|<span data-ttu-id="5d4a0-131">类型</span><span class="sxs-lookup"><span data-stu-id="5d4a0-131">Type</span></span>|<span data-ttu-id="5d4a0-132">说明</span><span class="sxs-lookup"><span data-stu-id="5d4a0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d4a0-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5d4a0-133">displayName</span></span>|<span data-ttu-id="5d4a0-134">String</span><span class="sxs-lookup"><span data-stu-id="5d4a0-134">String</span></span>|<span data-ttu-id="5d4a0-135">访问包名称。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-135">The access package name.</span></span>|
|<span data-ttu-id="5d4a0-136">description</span><span class="sxs-lookup"><span data-stu-id="5d4a0-136">description</span></span>|<span data-ttu-id="5d4a0-137">String</span><span class="sxs-lookup"><span data-stu-id="5d4a0-137">String</span></span>|<span data-ttu-id="5d4a0-138">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-138">The description of the access package.</span></span>|

## <a name="response"></a><span data-ttu-id="5d4a0-139">响应</span><span class="sxs-lookup"><span data-stu-id="5d4a0-139">Response</span></span>
<span data-ttu-id="5d4a0-140">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5d4a0-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5d4a0-141">示例</span><span class="sxs-lookup"><span data-stu-id="5d4a0-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5d4a0-142">请求</span><span class="sxs-lookup"><span data-stu-id="5d4a0-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5d4a0-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="5d4a0-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
Content-Type: application/json
Content-length: 38

{
  "displayName":"Access Package New Name"
}
```
# <a name="c"></a>[<span data-ttu-id="5d4a0-144">C#</span><span class="sxs-lookup"><span data-stu-id="5d4a0-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5d4a0-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5d4a0-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5d4a0-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5d4a0-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5d4a0-147">响应</span><span class="sxs-lookup"><span data-stu-id="5d4a0-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


