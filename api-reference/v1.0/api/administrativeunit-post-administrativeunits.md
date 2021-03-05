---
title: 创建 administrativeUnit
description: 使用此 API 创建新的 administrativeUnit。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c1e954dbbfc9a948e12c1ea99b3079e695531a27
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432989"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="1b5ec-103">创建 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="1b5ec-103">Create administrativeUnit</span></span>

<span data-ttu-id="1b5ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b5ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1b5ec-105">使用此 API 创建新的[administrativeUnit。](../resources/administrativeunit.md)</span><span class="sxs-lookup"><span data-stu-id="1b5ec-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1b5ec-106">权限</span><span class="sxs-lookup"><span data-stu-id="1b5ec-106">Permissions</span></span>
<span data-ttu-id="1b5ec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1b5ec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1b5ec-109">Permission type</span></span>      | <span data-ttu-id="1b5ec-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1b5ec-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b5ec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1b5ec-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b5ec-112">AdministrativeUnit.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b5ec-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b5ec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1b5ec-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b5ec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-114">Not supported.</span></span>    |
|<span data-ttu-id="1b5ec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1b5ec-115">Application</span></span> | <span data-ttu-id="1b5ec-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b5ec-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b5ec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1b5ec-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="1b5ec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1b5ec-118">Request headers</span></span>
| <span data-ttu-id="1b5ec-119">名称</span><span class="sxs-lookup"><span data-stu-id="1b5ec-119">Name</span></span>      |<span data-ttu-id="1b5ec-120">说明</span><span class="sxs-lookup"><span data-stu-id="1b5ec-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1b5ec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b5ec-121">Authorization</span></span>  | <span data-ttu-id="1b5ec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1b5ec-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="1b5ec-124">Content-type</span></span> | <span data-ttu-id="1b5ec-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1b5ec-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b5ec-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1b5ec-127">Request body</span></span>
<span data-ttu-id="1b5ec-128">在请求正文中，提供 [administrativeUnit](../resources/administrativeunit.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="1b5ec-129">由于 **administrativeUnit** 资源 [支持扩展](/graph/extensibility-overview)，因此可以使用该操作，并创建管理单元时将包含您自己的数据的 `POST` 自定义属性添加到管理单元。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="1b5ec-130">响应</span><span class="sxs-lookup"><span data-stu-id="1b5ec-130">Response</span></span>

<span data-ttu-id="1b5ec-131">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [administrativeUnit](../resources/administrativeunit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b5ec-132">示例</span><span class="sxs-lookup"><span data-stu-id="1b5ec-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b5ec-133">请求</span><span class="sxs-lookup"><span data-stu-id="1b5ec-133">Request</span></span>

<span data-ttu-id="1b5ec-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="1b5ec-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b5ec-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_administrativeunit_from_administrativeunits"
}-->
```http
POST https://graph.microsoft.com/v1.0/directory/administrativeUnits
Content-type: application/json
Content-length: 150

{
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```
# <a name="c"></a>[<span data-ttu-id="1b5ec-136">C#</span><span class="sxs-lookup"><span data-stu-id="1b5ec-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1b5ec-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b5ec-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b5ec-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b5ec-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b5ec-139">Java</span><span class="sxs-lookup"><span data-stu-id="1b5ec-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-administrativeunit-from-administrativeunits-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

<span data-ttu-id="1b5ec-140">在请求正文中，提供 [administrativeUnit](../resources/administrativeunit.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-140">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="1b5ec-141">响应</span><span class="sxs-lookup"><span data-stu-id="1b5ec-141">Response</span></span>

<span data-ttu-id="1b5ec-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-142">The following is an example of the response.</span></span> 
> <span data-ttu-id="1b5ec-143">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-143">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1b5ec-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1b5ec-144">All the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#administrativeUnits/$entity",
    "id": "7a3dc8f3-b3a0-4164-9a99-ed36f3af039f",
    "deletedDateTime": null,
    "displayName": "Seattle District Technical Schools",
    "description": "Seattle district technical schools administration",
    "visibility": "HiddenMembership"
}
```

## <a name="see-also"></a><span data-ttu-id="1b5ec-145">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1b5ec-145">See also</span></span>

- [<span data-ttu-id="1b5ec-146">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="1b5ec-146">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="1b5ec-147">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="1b5ec-147">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
