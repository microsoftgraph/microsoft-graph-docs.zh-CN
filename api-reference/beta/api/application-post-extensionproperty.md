---
title: 创建 extensionProperty
description: 创建新的 extensionProperty。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd4a28300d18db4ef9bf7dded1b739d0870ffa49
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47996813"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="6c1bd-103">创建 extensionProperty</span><span class="sxs-lookup"><span data-stu-id="6c1bd-103">Create extensionProperty</span></span>

<span data-ttu-id="6c1bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c1bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c1bd-105">创建新的 [extensionProperty](../resources/extensionproperty.md) 定义。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-105">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="6c1bd-106">您可以使用此操作将自定义属性值添加到 extensionProperty 中定义的目标对象类型，使用目标对象的标准创建和更新请求。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-106">You can use this operation to add a custom property value to the targeted object type defined in the extensionProperty, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c1bd-107">权限</span><span class="sxs-lookup"><span data-stu-id="6c1bd-107">Permissions</span></span>

<span data-ttu-id="6c1bd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c1bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c1bd-110">Permission type</span></span>      | <span data-ttu-id="6c1bd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c1bd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c1bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c1bd-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6c1bd-113">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="6c1bd-113">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c1bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c1bd-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c1bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-115">Not supported.</span></span>    |
|<span data-ttu-id="6c1bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c1bd-116">Application</span></span> | <span data-ttu-id="6c1bd-117">Application.readwrite.ownedby、所有的 readwrite、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c1bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c1bd-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="6c1bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c1bd-119">Request headers</span></span>
| <span data-ttu-id="6c1bd-120">名称</span><span class="sxs-lookup"><span data-stu-id="6c1bd-120">Name</span></span>       | <span data-ttu-id="6c1bd-121">说明</span><span class="sxs-lookup"><span data-stu-id="6c1bd-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="6c1bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c1bd-122">Authorization</span></span>  | <span data-ttu-id="6c1bd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c1bd-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c1bd-125">Content-Type</span></span> | <span data-ttu-id="6c1bd-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6c1bd-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c1bd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c1bd-128">Request body</span></span>

<span data-ttu-id="6c1bd-129">在请求正文中，提供具有以下属性的 [extensionProperty](../resources/extensionproperty.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-129">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="6c1bd-130">属性</span><span class="sxs-lookup"><span data-stu-id="6c1bd-130">Property</span></span>     | <span data-ttu-id="6c1bd-131">类型</span><span class="sxs-lookup"><span data-stu-id="6c1bd-131">Type</span></span>        | <span data-ttu-id="6c1bd-132">说明</span><span class="sxs-lookup"><span data-stu-id="6c1bd-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c1bd-133">DataType</span><span class="sxs-lookup"><span data-stu-id="6c1bd-133">dataType</span></span>|<span data-ttu-id="6c1bd-134">String</span><span class="sxs-lookup"><span data-stu-id="6c1bd-134">String</span></span>| <span data-ttu-id="6c1bd-135">指定 extension 属性可以包含的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-135">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="6c1bd-136">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-136">Following values are supported.</span></span> <span data-ttu-id="6c1bd-137">不可为空。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-137">Not nullable.</span></span> <ul><li><span data-ttu-id="6c1bd-138">`Binary` -最多为256字节</span><span class="sxs-lookup"><span data-stu-id="6c1bd-138">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="6c1bd-139">`DateTime` -必须以 ISO 8601 格式指定。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-139">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="6c1bd-140">存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-140">Will be stored in UTC.</span></span></li><li><span data-ttu-id="6c1bd-141">`Integer` -32-位值。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-141">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="6c1bd-142">`LargeInteger` -64-位值。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-142">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="6c1bd-143">`String` -最多为-256 个字符</span><span class="sxs-lookup"><span data-stu-id="6c1bd-143">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="6c1bd-144">name</span><span class="sxs-lookup"><span data-stu-id="6c1bd-144">name</span></span>|<span data-ttu-id="6c1bd-145">String</span><span class="sxs-lookup"><span data-stu-id="6c1bd-145">String</span></span>| <span data-ttu-id="6c1bd-146">扩展属性的名称。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-146">Name of the extension property.</span></span> <span data-ttu-id="6c1bd-147">不可为空。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-147">Not nullable.</span></span> |
|<span data-ttu-id="6c1bd-148">targetObjects</span><span class="sxs-lookup"><span data-stu-id="6c1bd-148">targetObjects</span></span>|<span data-ttu-id="6c1bd-149">String collection</span><span class="sxs-lookup"><span data-stu-id="6c1bd-149">String collection</span></span>| <span data-ttu-id="6c1bd-150">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-150">Following values are supported.</span></span> <span data-ttu-id="6c1bd-151">不可为空。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-151">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="6c1bd-152">响应</span><span class="sxs-lookup"><span data-stu-id="6c1bd-152">Response</span></span>

<span data-ttu-id="6c1bd-153">如果成功，此方法 `201, Created` 在响应正文中返回响应代码和新的 [extensionProperty](../resources/extensionproperty.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-153">If successful, this method returns `201, Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c1bd-154">示例</span><span class="sxs-lookup"><span data-stu-id="6c1bd-154">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c1bd-155">请求</span><span class="sxs-lookup"><span data-stu-id="6c1bd-155">Request</span></span>

<span data-ttu-id="6c1bd-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c1bd-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c1bd-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="6c1bd-158">C#</span><span class="sxs-lookup"><span data-stu-id="6c1bd-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-extensionproperty-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c1bd-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c1bd-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-extensionproperty-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c1bd-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c1bd-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-extensionproperty-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c1bd-161">响应</span><span class="sxs-lookup"><span data-stu-id="6c1bd-161">Response</span></span>

<span data-ttu-id="6c1bd-162">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [extensionProperty](../resources/extensionProperty.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c1bd-162">If successful, this method returns a `201 Created` response code and an [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.extensionProperty"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "a2c459db-f5dc-4328-ae9b-118e88d04d19",
    "deletedDateTime": null,
    "appDisplayName": "Display name",
    "name": "extension_b3efaf8f68a44275abcff28ef86b2ee3_extensionName",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "targetObjects": [
        "Application"
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create extensionProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


