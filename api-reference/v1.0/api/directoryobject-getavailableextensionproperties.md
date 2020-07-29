---
title: directoryObject： getAvailableExtensionProperties
description: 获取已在目录中注册的目录扩展属性的所有或筛选列表。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3dfc4d3c8e6d2f379d717649c945aaa48e978916
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509503"
---
# <a name="directoryobject-getavailableextensionproperties"></a><span data-ttu-id="86a2d-103">directoryObject： getAvailableExtensionProperties</span><span class="sxs-lookup"><span data-stu-id="86a2d-103">directoryObject: getAvailableExtensionProperties</span></span>
<span data-ttu-id="86a2d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86a2d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86a2d-105">返回已在目录中注册的目录扩展属性的所有或已筛选列表。</span><span class="sxs-lookup"><span data-stu-id="86a2d-105">Return all or a filtered list of the directory extension properties that have been registered in a directory.</span></span> <span data-ttu-id="86a2d-106">以下实体支持扩展属性：**用户**、**组**、**组织**、**设备**、**应用程序**和**servicePrincipal**。</span><span class="sxs-lookup"><span data-stu-id="86a2d-106">The following entities support extension properties: **user**, **group**, **organization**, **device**, **application**, and **servicePrincipal**.</span></span>

## <a name="permissions"></a><span data-ttu-id="86a2d-107">权限</span><span class="sxs-lookup"><span data-stu-id="86a2d-107">Permissions</span></span>
<span data-ttu-id="86a2d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86a2d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a2d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="86a2d-110">Permission type</span></span>|<span data-ttu-id="86a2d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="86a2d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86a2d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86a2d-112">Delegated (work or school account)</span></span>| <span data-ttu-id="86a2d-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a2d-113">Directory.Read.All</span></span> |
|<span data-ttu-id="86a2d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86a2d-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="86a2d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="86a2d-115">Not supported.</span></span> |
|<span data-ttu-id="86a2d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="86a2d-116">Application</span></span>| <span data-ttu-id="86a2d-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a2d-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86a2d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86a2d-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /directoryObjects/getAvailableExtensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="86a2d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="86a2d-119">Request headers</span></span>
|<span data-ttu-id="86a2d-120">名称</span><span class="sxs-lookup"><span data-stu-id="86a2d-120">Name</span></span>|<span data-ttu-id="86a2d-121">说明</span><span class="sxs-lookup"><span data-stu-id="86a2d-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="86a2d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86a2d-122">Authorization</span></span>|<span data-ttu-id="86a2d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86a2d-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="86a2d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="86a2d-125">Content-Type</span></span>|<span data-ttu-id="86a2d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="86a2d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="86a2d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="86a2d-128">Request body</span></span>
<span data-ttu-id="86a2d-129">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86a2d-129">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="86a2d-130">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="86a2d-130">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="86a2d-131">参数</span><span class="sxs-lookup"><span data-stu-id="86a2d-131">Parameter</span></span>|<span data-ttu-id="86a2d-132">类型</span><span class="sxs-lookup"><span data-stu-id="86a2d-132">Type</span></span>|<span data-ttu-id="86a2d-133">说明</span><span class="sxs-lookup"><span data-stu-id="86a2d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86a2d-134">isSyncedFromOnPremises</span><span class="sxs-lookup"><span data-stu-id="86a2d-134">isSyncedFromOnPremises</span></span>|<span data-ttu-id="86a2d-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="86a2d-135">Boolean</span></span>|<span data-ttu-id="86a2d-136">`true`若要指定仅应返回从本地目录同步的扩展属性，则为  ; 否则为  。`false`若要指定仅应返回不是从本地目录同步的扩展属性。</span><span class="sxs-lookup"><span data-stu-id="86a2d-136">`true` to specify that only extension properties that are synced from the on-premises directory should be returned; `false` to specify that only extension properties that are not synced from the on-premises directory should be returned.</span></span> <span data-ttu-id="86a2d-137">如果省略该参数，则返回所有扩展属性（同步和未同步）。</span><span class="sxs-lookup"><span data-stu-id="86a2d-137">If the parameter is omitted, all extension properties (both synced and non-synced) are returned.</span></span>|


## <a name="response"></a><span data-ttu-id="86a2d-138">响应</span><span class="sxs-lookup"><span data-stu-id="86a2d-138">Response</span></span>

<span data-ttu-id="86a2d-139">如果成功，此操作会 `200 OK` 在响应正文中返回响应代码和[extensionProperty](../resources/extensionproperty.md)集合。</span><span class="sxs-lookup"><span data-stu-id="86a2d-139">If successful, this action returns a `200 OK` response code and an [extensionProperty](../resources/extensionproperty.md) collection in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86a2d-140">示例</span><span class="sxs-lookup"><span data-stu-id="86a2d-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="86a2d-141">请求</span><span class="sxs-lookup"><span data-stu-id="86a2d-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="86a2d-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="86a2d-142">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="86a2d-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="86a2d-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getavailableextensionproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="86a2d-144">响应</span><span class="sxs-lookup"><span data-stu-id="86a2d-144">Response</span></span>
> <span data-ttu-id="86a2d-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="86a2d-145">**Note:** The response object shown here might be shortened for readability.</span></span>

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

