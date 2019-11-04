---
title: 创建 extensionProperty
description: 创建新的 extensionProperty。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bb6ac47f3b33bb963181e71d7f5d7c83e2bf13b0
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939689"
---
# <a name="create-extensionproperty"></a><span data-ttu-id="e9048-103">创建 extensionProperty</span><span class="sxs-lookup"><span data-stu-id="e9048-103">Create extensionProperty</span></span>

<span data-ttu-id="e9048-104">创建新的[extensionProperty](../resources/extensionproperty.md)定义。</span><span class="sxs-lookup"><span data-stu-id="e9048-104">Create a new [extensionProperty](../resources/extensionproperty.md) definition.</span></span> <span data-ttu-id="e9048-105">您可以使用此操作将自定义属性值添加到**extensionProperty**中定义的目标对象类型，使用目标对象的标准创建和更新请求。</span><span class="sxs-lookup"><span data-stu-id="e9048-105">You can use this operation to add a custom property value to the targeted object type defined in the **extensionProperty**, using standard creation and update requests to the target object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9048-106">权限</span><span class="sxs-lookup"><span data-stu-id="e9048-106">Permissions</span></span>

<span data-ttu-id="e9048-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e9048-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9048-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9048-109">Permission type</span></span>      | <span data-ttu-id="e9048-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e9048-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9048-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9048-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e9048-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e9048-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e9048-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9048-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9048-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9048-114">Not supported.</span></span>    |
|<span data-ttu-id="e9048-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9048-115">Application</span></span> | <span data-ttu-id="e9048-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e9048-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e9048-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9048-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/extensionProperties
```

## <a name="request-headers"></a><span data-ttu-id="e9048-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9048-118">Request headers</span></span>
| <span data-ttu-id="e9048-119">名称</span><span class="sxs-lookup"><span data-stu-id="e9048-119">Name</span></span>       | <span data-ttu-id="e9048-120">说明</span><span class="sxs-lookup"><span data-stu-id="e9048-120">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="e9048-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9048-121">Authorization</span></span>  | <span data-ttu-id="e9048-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e9048-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e9048-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="e9048-124">Content-type</span></span> | <span data-ttu-id="e9048-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e9048-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e9048-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9048-127">Request body</span></span>

<span data-ttu-id="e9048-128">在请求正文中，提供具有以下属性的[extensionProperty](../resources/extensionproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e9048-128">In the request body, provide an [extensionProperty](../resources/extensionproperty.md) object with the following properties.</span></span>


| <span data-ttu-id="e9048-129">属性</span><span class="sxs-lookup"><span data-stu-id="e9048-129">Property</span></span>     | <span data-ttu-id="e9048-130">类型</span><span class="sxs-lookup"><span data-stu-id="e9048-130">Type</span></span>        | <span data-ttu-id="e9048-131">描述</span><span class="sxs-lookup"><span data-stu-id="e9048-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e9048-132">DataType</span><span class="sxs-lookup"><span data-stu-id="e9048-132">dataType</span></span>|<span data-ttu-id="e9048-133">String</span><span class="sxs-lookup"><span data-stu-id="e9048-133">String</span></span>| <span data-ttu-id="e9048-134">指定 extension 属性可以包含的值的数据类型。</span><span class="sxs-lookup"><span data-stu-id="e9048-134">Specifies the data type of the value the extension property can hold.</span></span> <span data-ttu-id="e9048-135">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="e9048-135">Following values are supported.</span></span> <span data-ttu-id="e9048-136">不可为空。</span><span class="sxs-lookup"><span data-stu-id="e9048-136">Not nullable.</span></span> <ul><li><span data-ttu-id="e9048-137">`Binary`-最多为256字节</span><span class="sxs-lookup"><span data-stu-id="e9048-137">`Binary` - 256 bytes maximum</span></span></li><li>`Boolean`</li><li><span data-ttu-id="e9048-138">`DateTime`-必须以 ISO 8601 格式指定。</span><span class="sxs-lookup"><span data-stu-id="e9048-138">`DateTime` - Must be specified in ISO 8601 format.</span></span> <span data-ttu-id="e9048-139">存储为 UTC 格式。</span><span class="sxs-lookup"><span data-stu-id="e9048-139">Will be stored in UTC.</span></span></li><li><span data-ttu-id="e9048-140">`Integer`-32-位值。</span><span class="sxs-lookup"><span data-stu-id="e9048-140">`Integer` - 32-bit value.</span></span></li><li><span data-ttu-id="e9048-141">`LargeInteger`-64-位值。</span><span class="sxs-lookup"><span data-stu-id="e9048-141">`LargeInteger` - 64-bit value.</span></span></li><li><span data-ttu-id="e9048-142">`String`-最多为-256 个字符</span><span class="sxs-lookup"><span data-stu-id="e9048-142">`String` - 256 characters maximum</span></span></li></ul>|
|<span data-ttu-id="e9048-143">name</span><span class="sxs-lookup"><span data-stu-id="e9048-143">name</span></span>|<span data-ttu-id="e9048-144">String</span><span class="sxs-lookup"><span data-stu-id="e9048-144">String</span></span>| <span data-ttu-id="e9048-145">扩展属性的名称。</span><span class="sxs-lookup"><span data-stu-id="e9048-145">Name of the extension property.</span></span> <span data-ttu-id="e9048-146">不可为空。</span><span class="sxs-lookup"><span data-stu-id="e9048-146">Not nullable.</span></span> |
|<span data-ttu-id="e9048-147">targetObjects</span><span class="sxs-lookup"><span data-stu-id="e9048-147">targetObjects</span></span>|<span data-ttu-id="e9048-148">String collection</span><span class="sxs-lookup"><span data-stu-id="e9048-148">String collection</span></span>| <span data-ttu-id="e9048-149">支持以下值。</span><span class="sxs-lookup"><span data-stu-id="e9048-149">Following values are supported.</span></span> <span data-ttu-id="e9048-150">不可为空。</span><span class="sxs-lookup"><span data-stu-id="e9048-150">Not nullable.</span></span> <ul><li>`User`</li><li>`Group`</li><li>`Organization`</li><li>`Device`</li><li>`Application`</li></ul>|


## <a name="response"></a><span data-ttu-id="e9048-151">响应</span><span class="sxs-lookup"><span data-stu-id="e9048-151">Response</span></span>

<span data-ttu-id="e9048-152">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[extensionProperty](../resources/extensionproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e9048-152">If successful, this method returns a `201 Created` response code and a new [extensionProperty](../resources/extensionproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e9048-153">示例</span><span class="sxs-lookup"><span data-stu-id="e9048-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e9048-154">请求</span><span class="sxs-lookup"><span data-stu-id="e9048-154">Request</span></span>

<span data-ttu-id="e9048-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e9048-155">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_extensionproperty_from_application"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/extensionProperties
Content-type: application/json

{
    "name": "extensionName",
    "dataType": "string",
    "targetObjects": [
        "Application"
    ]
}
```

### <a name="response"></a><span data-ttu-id="e9048-156">响应</span><span class="sxs-lookup"><span data-stu-id="e9048-156">Response</span></span>

<span data-ttu-id="e9048-157">如果成功，此方法在`201 Created`响应正文中返回响应代码和[extensionProperty](../resources/extensionProperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e9048-157">If successful, this method returns `201 Created` response code and [extensionProperty](../resources/extensionProperty.md) object in the response body.</span></span>

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
