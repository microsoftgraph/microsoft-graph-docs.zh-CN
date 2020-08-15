---
title: 更新 accessPackageCatalog
description: 更新 accessPackageCatalog 对象的属性。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3145fcd5fda95bb9c76763bf804ef3a4f4cce7d7
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757410"
---
# <a name="update-accesspackagecatalog"></a><span data-ttu-id="09407-103">更新 accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="09407-103">Update accessPackageCatalog</span></span>

<span data-ttu-id="09407-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09407-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09407-105">更新现有 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象以更改其一个或多个属性，如显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="09407-105">Update an existing [accessPackageCatalog](../resources/accesspackagecatalog.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="09407-106">权限</span><span class="sxs-lookup"><span data-stu-id="09407-106">Permissions</span></span>
<span data-ttu-id="09407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="09407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="09407-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09407-109">Permission type</span></span>|<span data-ttu-id="09407-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="09407-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09407-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09407-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="09407-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09407-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="09407-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09407-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09407-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="09407-114">Not supported.</span></span> |
|<span data-ttu-id="09407-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09407-115">Application</span></span>                            | <span data-ttu-id="09407-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09407-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09407-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09407-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}
```
## <a name="request-headers"></a><span data-ttu-id="09407-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09407-118">Request headers</span></span>
|<span data-ttu-id="09407-119">名称</span><span class="sxs-lookup"><span data-stu-id="09407-119">Name</span></span>|<span data-ttu-id="09407-120">说明</span><span class="sxs-lookup"><span data-stu-id="09407-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="09407-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09407-121">Authorization</span></span>|<span data-ttu-id="09407-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="09407-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="09407-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09407-124">Content-Type</span></span>|<span data-ttu-id="09407-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="09407-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="09407-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="09407-127">Request body</span></span>
<span data-ttu-id="09407-128">在请求正文中，提供 [accessPackageCatalog](../resources/accesspackagecatalog.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09407-128">In the request body, supply a JSON representation of the [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

<span data-ttu-id="09407-129">下表显示了在更新 [accessPackageCatalog](../resources/accesspackagecatalog.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="09407-129">The following table shows the properties that are required when you update the [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

|<span data-ttu-id="09407-130">属性</span><span class="sxs-lookup"><span data-stu-id="09407-130">Property</span></span>|<span data-ttu-id="09407-131">类型</span><span class="sxs-lookup"><span data-stu-id="09407-131">Type</span></span>|<span data-ttu-id="09407-132">说明</span><span class="sxs-lookup"><span data-stu-id="09407-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09407-133">displayName</span><span class="sxs-lookup"><span data-stu-id="09407-133">displayName</span></span>|<span data-ttu-id="09407-134">字符串</span><span class="sxs-lookup"><span data-stu-id="09407-134">String</span></span>|<span data-ttu-id="09407-135">访问包目录名称。</span><span class="sxs-lookup"><span data-stu-id="09407-135">The access package catalog name.</span></span>|
|<span data-ttu-id="09407-136">说明</span><span class="sxs-lookup"><span data-stu-id="09407-136">description</span></span>|<span data-ttu-id="09407-137">字符串</span><span class="sxs-lookup"><span data-stu-id="09407-137">String</span></span>|<span data-ttu-id="09407-138">访问包目录的说明。</span><span class="sxs-lookup"><span data-stu-id="09407-138">The description of the access package catalog.</span></span>|

## <a name="response"></a><span data-ttu-id="09407-139">响应</span><span class="sxs-lookup"><span data-stu-id="09407-139">Response</span></span>
<span data-ttu-id="09407-140">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="09407-140">If successful, this method returns a `204 No Content` response code.</span></span>



## <a name="examples"></a><span data-ttu-id="09407-141">示例</span><span class="sxs-lookup"><span data-stu-id="09407-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09407-142">请求</span><span class="sxs-lookup"><span data-stu-id="09407-142">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="09407-143">响应</span><span class="sxs-lookup"><span data-stu-id="09407-143">Response</span></span>

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
