---
title: 更新 accessPackageCatalog
description: 更新 accessPackageCatalog 对象的属性。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 213d771186f770b1c4ef791ec0d239d09d0afdfe
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806403"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="f8adf-103">更新 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="f8adf-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="f8adf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8adf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8adf-105">更新现有 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象以更改其一个或多个属性，如显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="f8adf-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="f8adf-106">权限</span><span class="sxs-lookup"><span data-stu-id="f8adf-106">Permissions</span></span>
<span data-ttu-id="f8adf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f8adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f8adf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8adf-109">Permission type</span></span>|<span data-ttu-id="f8adf-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8adf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8adf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8adf-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8adf-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8adf-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="f8adf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8adf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8adf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8adf-114">Not supported.</span></span> |
|<span data-ttu-id="f8adf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8adf-115">Application</span></span>                            | <span data-ttu-id="f8adf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8adf-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8adf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8adf-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="f8adf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8adf-118">Request headers</span></span>
|<span data-ttu-id="f8adf-119">名称</span><span class="sxs-lookup"><span data-stu-id="f8adf-119">Name</span></span>|<span data-ttu-id="f8adf-120">说明</span><span class="sxs-lookup"><span data-stu-id="f8adf-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f8adf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8adf-121">Authorization</span></span>|<span data-ttu-id="f8adf-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f8adf-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f8adf-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8adf-124">Content-Type</span></span>|<span data-ttu-id="f8adf-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f8adf-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8adf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8adf-127">Request body</span></span>
<span data-ttu-id="f8adf-128">在请求正文中，提供 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8adf-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="f8adf-129">下表显示了在更新 [accessPackageCatalog](../resources/accesspackagecatalog.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8adf-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="f8adf-130">属性</span><span class="sxs-lookup"><span data-stu-id="f8adf-130">Property</span></span>|<span data-ttu-id="f8adf-131">类型</span><span class="sxs-lookup"><span data-stu-id="f8adf-131">Type</span></span>|<span data-ttu-id="f8adf-132">说明</span><span class="sxs-lookup"><span data-stu-id="f8adf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8adf-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f8adf-133">displayName</span></span>|<span data-ttu-id="f8adf-134">String</span><span class="sxs-lookup"><span data-stu-id="f8adf-134">String</span></span>|<span data-ttu-id="f8adf-135">访问包目录名称。</span><span class="sxs-lookup"><span data-stu-id="f8adf-135">The access package catalog name.</span></span>|
|<span data-ttu-id="f8adf-136">description</span><span class="sxs-lookup"><span data-stu-id="f8adf-136">description</span></span>|<span data-ttu-id="f8adf-137">String</span><span class="sxs-lookup"><span data-stu-id="f8adf-137">String</span></span>|<span data-ttu-id="f8adf-138">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="f8adf-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="f8adf-139">响应</span><span class="sxs-lookup"><span data-stu-id="f8adf-139">Response</span></span>
<span data-ttu-id="f8adf-140">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f8adf-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="f8adf-141">示例</span><span class="sxs-lookup"><span data-stu-id="f8adf-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f8adf-142">请求</span><span class="sxs-lookup"><span data-stu-id="f8adf-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f8adf-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="f8adf-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accesspackagecatalog"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
Content-Type: application/json
Content-length: 39

{
  "displayName":"Catalog One"
}
```
# <a name="c"></a>[<span data-ttu-id="f8adf-144">C#</span><span class="sxs-lookup"><span data-stu-id="f8adf-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accesspackagecatalog-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f8adf-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f8adf-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accesspackagecatalog-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f8adf-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f8adf-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accesspackagecatalog-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f8adf-147">响应</span><span class="sxs-lookup"><span data-stu-id="f8adf-147">Response</span></span>

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
  "description": "Update accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
