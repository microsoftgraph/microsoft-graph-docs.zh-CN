---
title: 更新 accessPackage
description: 更新 accessPackage 对象的属性。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 919a9f6a87463313d0193f3d8d43234654f3952f
ms.sourcegitcommit: da4f3d03e98ee5fa13f8c7a263d931e68a20a12c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2020
ms.locfileid: "46757414"
---
# <a name="update-accesspackage"></a><span data-ttu-id="1f1e9-103">更新 accessPackage</span><span class="sxs-lookup"><span data-stu-id="1f1e9-103">Update accessPackage</span></span>

<span data-ttu-id="1f1e9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f1e9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f1e9-105">更新现有 [accessPackage](../resources/accesspackage.md) 对象以更改其一个或多个属性，如显示名称或说明。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-105">Update an existing [accessPackage](../resources/accesspackage.md) object to change one or more of its properties, such as the display name or description.</span></span>

## <a name="permissions"></a><span data-ttu-id="1f1e9-106">权限</span><span class="sxs-lookup"><span data-stu-id="1f1e9-106">Permissions</span></span>
<span data-ttu-id="1f1e9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="1f1e9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f1e9-109">Permission type</span></span>|<span data-ttu-id="1f1e9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f1e9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f1e9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f1e9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1f1e9-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f1e9-112">EntitlementManagement.ReadWrite.All</span></span> |
|<span data-ttu-id="1f1e9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f1e9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f1e9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-114">Not supported.</span></span> |
|<span data-ttu-id="1f1e9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f1e9-115">Application</span></span>                            | <span data-ttu-id="1f1e9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f1e9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f1e9-117">HTTP request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```
## <a name="request-headers"></a><span data-ttu-id="1f1e9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f1e9-118">Request headers</span></span>
|<span data-ttu-id="1f1e9-119">名称</span><span class="sxs-lookup"><span data-stu-id="1f1e9-119">Name</span></span>|<span data-ttu-id="1f1e9-120">说明</span><span class="sxs-lookup"><span data-stu-id="1f1e9-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1f1e9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f1e9-121">Authorization</span></span>|<span data-ttu-id="1f1e9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1f1e9-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1f1e9-124">Content-Type</span></span>|<span data-ttu-id="1f1e9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1f1e9-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f1e9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f1e9-127">Request body</span></span>
<span data-ttu-id="1f1e9-128">在请求正文中，提供 [accessPackage](../resources/accesspackage.md) 对象的参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-128">In the request body, supply a JSON representation of the parameters of an [accessPackage](../resources/accesspackage.md) object.</span></span>

<span data-ttu-id="1f1e9-129">下表显示了在更新 [accessPackage](../resources/accesspackage.md)时可提供的属性。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-129">The following table shows the properties that can be supplied when you update an [accessPackage](../resources/accesspackage.md).</span></span>

|<span data-ttu-id="1f1e9-130">属性</span><span class="sxs-lookup"><span data-stu-id="1f1e9-130">Property</span></span>|<span data-ttu-id="1f1e9-131">类型</span><span class="sxs-lookup"><span data-stu-id="1f1e9-131">Type</span></span>|<span data-ttu-id="1f1e9-132">说明</span><span class="sxs-lookup"><span data-stu-id="1f1e9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f1e9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1f1e9-133">displayName</span></span>|<span data-ttu-id="1f1e9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="1f1e9-134">String</span></span>|<span data-ttu-id="1f1e9-135">访问包名称。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-135">The access package name.</span></span>|
|<span data-ttu-id="1f1e9-136">说明</span><span class="sxs-lookup"><span data-stu-id="1f1e9-136">description</span></span>|<span data-ttu-id="1f1e9-137">字符串</span><span class="sxs-lookup"><span data-stu-id="1f1e9-137">String</span></span>|<span data-ttu-id="1f1e9-138">访问包的说明。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-138">The description of the access package.</span></span>|

## <a name="response"></a><span data-ttu-id="1f1e9-139">响应</span><span class="sxs-lookup"><span data-stu-id="1f1e9-139">Response</span></span>
<span data-ttu-id="1f1e9-140">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="1f1e9-140">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1f1e9-141">示例</span><span class="sxs-lookup"><span data-stu-id="1f1e9-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1f1e9-142">请求</span><span class="sxs-lookup"><span data-stu-id="1f1e9-142">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="1f1e9-143">响应</span><span class="sxs-lookup"><span data-stu-id="1f1e9-143">Response</span></span>

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
