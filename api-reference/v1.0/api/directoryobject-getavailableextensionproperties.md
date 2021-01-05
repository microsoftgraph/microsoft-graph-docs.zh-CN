---
title: directoryObject： getAvailableExtensionProperties
description: 获取已在目录中注册的目录扩展属性的所有或筛选列表。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6de4d6e0b98045d84fcaa02d9da9c71f337f8cb2
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754207"
---
# <a name="directoryobject-getavailableextensionproperties"></a><span data-ttu-id="6671e-103">directoryObject：getAvailableExtensionProperties</span><span class="sxs-lookup"><span data-stu-id="6671e-103">directoryObject: getAvailableExtensionProperties</span></span>
<span data-ttu-id="6671e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6671e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6671e-105">返回已在目录中注册的目录扩展属性的所有列表或筛选列表。</span><span class="sxs-lookup"><span data-stu-id="6671e-105">Return all or a filtered list of the directory extension properties that have been registered in a directory.</span></span> <span data-ttu-id="6671e-106">以下实体支持扩展属性：**用户**、**组**、**组织**、**设备\*\*\*\*、应用程序和** **servicePrincipal。**</span><span class="sxs-lookup"><span data-stu-id="6671e-106">The following entities support extension properties: **user**, **group**, **organization**, **device**, **application**, and **servicePrincipal**.</span></span>

## <a name="permissions"></a><span data-ttu-id="6671e-107">权限</span><span class="sxs-lookup"><span data-stu-id="6671e-107">Permissions</span></span>
<span data-ttu-id="6671e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6671e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6671e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6671e-110">Permission type</span></span>|<span data-ttu-id="6671e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6671e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6671e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6671e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="6671e-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6671e-113">Directory.Read.All</span></span> |
|<span data-ttu-id="6671e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6671e-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="6671e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6671e-115">Not supported.</span></span> |
|<span data-ttu-id="6671e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6671e-116">Application</span></span>| <span data-ttu-id="6671e-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6671e-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6671e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6671e-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directoryObjects/getAvailableExtensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="6671e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6671e-119">Request headers</span></span>
|<span data-ttu-id="6671e-120">名称</span><span class="sxs-lookup"><span data-stu-id="6671e-120">Name</span></span>|<span data-ttu-id="6671e-121">说明</span><span class="sxs-lookup"><span data-stu-id="6671e-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6671e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6671e-122">Authorization</span></span>|<span data-ttu-id="6671e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6671e-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6671e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6671e-125">Content-Type</span></span>|<span data-ttu-id="6671e-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6671e-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6671e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6671e-128">Request body</span></span>
<span data-ttu-id="6671e-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6671e-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6671e-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="6671e-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6671e-131">参数</span><span class="sxs-lookup"><span data-stu-id="6671e-131">Parameter</span></span>|<span data-ttu-id="6671e-132">类型</span><span class="sxs-lookup"><span data-stu-id="6671e-132">Type</span></span>|<span data-ttu-id="6671e-133">说明</span><span class="sxs-lookup"><span data-stu-id="6671e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6671e-134">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="6671e-134">isSyncedFromOnPremises</span></span>|<span data-ttu-id="6671e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="6671e-135">Boolean</span></span>|<span data-ttu-id="6671e-136">`true` 指定仅返回从本地目录同步的扩展属性;以指定仅返回未从本地目录同步的 `false` 扩展属性。</span><span class="sxs-lookup"><span data-stu-id="6671e-136">`true` to specify that only extension properties that are synced from the on-premises directory should be returned; `false` to specify that only extension properties that are not synced from the on-premises directory should be returned.</span></span> <span data-ttu-id="6671e-137">如果省略该参数，则返回 (同步和非同步) 属性。</span><span class="sxs-lookup"><span data-stu-id="6671e-137">If the parameter is omitted, all extension properties (both synced and non-synced) are returned.</span></span>|


## <a name="response"></a><span data-ttu-id="6671e-138">响应</span><span class="sxs-lookup"><span data-stu-id="6671e-138">Response</span></span>

<span data-ttu-id="6671e-139">如果成功，此操作在响应正文中返回响应 `200 OK` 代码和 [extensionProperty](../resources/extensionproperty.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="6671e-139">If successful, this action returns a `200 OK` response code and an [extensionProperty](../resources/extensionproperty.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6671e-140">示例</span><span class="sxs-lookup"><span data-stu-id="6671e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6671e-141">请求</span><span class="sxs-lookup"><span data-stu-id="6671e-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6671e-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6671e-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getavailableextensionproperties"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/directoryObjects/getAvailableExtensionProperties
Content-Type: application/json
Content-length: 43

{
  "isSyncedFromOnPremises": "Boolean"
}
```
# <a name="javascript"></a>[<span data-ttu-id="6671e-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6671e-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getavailableextensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6671e-144">C#</span><span class="sxs-lookup"><span data-stu-id="6671e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getavailableextensionproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6671e-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6671e-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getavailableextensionproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6671e-146">Java</span><span class="sxs-lookup"><span data-stu-id="6671e-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getavailableextensionproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6671e-147">响应</span><span class="sxs-lookup"><span data-stu-id="6671e-147">Response</span></span>
> <span data-ttu-id="6671e-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6671e-148">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.extensionProperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.extensionProperty",
      "id": "d6a8bfec-893d-46e4-88fd-7db5fcc0fa62",
      "deletedDateTime": null,
      "appDisplayName": "SampleApp",
      "name": "extension_4d405aa8baa04fb494d3e0571fd9fd71_skypeId",
      "dataType": "String",
      "isSyncedFromOnPremises": false,
      "targetObjects": [
        "User"
      ]
    }
  ]
}
```


