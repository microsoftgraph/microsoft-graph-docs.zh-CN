---
title: 创建 administrativeUnit
description: 使用此 API 创建新的 administrativeUnit。
author: DougKirschner
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c363c5a387cbc0824b558cebfc03732cdf8fccb3
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991918"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="c61f8-103">创建 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="c61f8-103">Create administrativeUnit</span></span>

<span data-ttu-id="c61f8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c61f8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c61f8-105">使用此 API 创建新的 [administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="c61f8-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c61f8-106">权限</span><span class="sxs-lookup"><span data-stu-id="c61f8-106">Permissions</span></span>
<span data-ttu-id="c61f8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c61f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c61f8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c61f8-109">Permission type</span></span>      | <span data-ttu-id="c61f8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c61f8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c61f8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c61f8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c61f8-112">AdministrativeUnit.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c61f8-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c61f8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c61f8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c61f8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c61f8-114">Not supported.</span></span>    |
|<span data-ttu-id="c61f8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c61f8-115">Application</span></span> | <span data-ttu-id="c61f8-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c61f8-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c61f8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c61f8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="c61f8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c61f8-118">Request headers</span></span>
| <span data-ttu-id="c61f8-119">名称</span><span class="sxs-lookup"><span data-stu-id="c61f8-119">Name</span></span>      |<span data-ttu-id="c61f8-120">说明</span><span class="sxs-lookup"><span data-stu-id="c61f8-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c61f8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c61f8-121">Authorization</span></span>  | <span data-ttu-id="c61f8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c61f8-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c61f8-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="c61f8-124">Content-type</span></span> | <span data-ttu-id="c61f8-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c61f8-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c61f8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c61f8-127">Request body</span></span>
<span data-ttu-id="c61f8-128">在请求正文中，提供 [administrativeUnit](../resources/administrativeunit.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c61f8-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="c61f8-129">由于 **administrativeUnit** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用 操作，并在创建时将包含自己的数据的自定义属性 `POST` 添加到管理单元。</span><span class="sxs-lookup"><span data-stu-id="c61f8-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="c61f8-130">响应</span><span class="sxs-lookup"><span data-stu-id="c61f8-130">Response</span></span>

<span data-ttu-id="c61f8-131">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c61f8-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c61f8-132">示例</span><span class="sxs-lookup"><span data-stu-id="c61f8-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c61f8-133">请求</span><span class="sxs-lookup"><span data-stu-id="c61f8-133">Request</span></span>

<span data-ttu-id="c61f8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c61f8-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c61f8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="c61f8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/beta/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```
# <a name="c"></a>[<span data-ttu-id="c61f8-136">C#</span><span class="sxs-lookup"><span data-stu-id="c61f8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c61f8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c61f8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c61f8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c61f8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c61f8-139">Java</span><span class="sxs-lookup"><span data-stu-id="c61f8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-administrativeunit-from-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c61f8-140">在请求正文中，提供 [administrativeUnit](../resources/administrativeunit.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c61f8-140">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="c61f8-141">响应</span><span class="sxs-lookup"><span data-stu-id="c61f8-141">Response</span></span>

<span data-ttu-id="c61f8-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c61f8-142">The following is an example of the response.</span></span> 
> <span data-ttu-id="c61f8-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c61f8-143">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 172

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#administrativeUnits/$entity",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f",
    "deletedDateTime": null,
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```

## <a name="see-also"></a><span data-ttu-id="c61f8-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c61f8-144">See also</span></span>

- [<span data-ttu-id="c61f8-145">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c61f8-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c61f8-146">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="c61f8-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


