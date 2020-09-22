---
title: 创建 administrativeUnit
description: 使用此 API 创建新的 administrativeUnit。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d939dc871a1a22aa426a621470fa5ebaa227e1a8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997233"
---
# <a name="create-administrativeunit"></a><span data-ttu-id="d242f-103">创建 administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="d242f-103">Create administrativeUnit</span></span>

<span data-ttu-id="d242f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d242f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d242f-105">使用此 API 创建新的 [administrativeUnit](../resources/administrativeunit.md)。</span><span class="sxs-lookup"><span data-stu-id="d242f-105">Use this API to create a new [administrativeUnit](../resources/administrativeunit.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d242f-106">权限</span><span class="sxs-lookup"><span data-stu-id="d242f-106">Permissions</span></span>
<span data-ttu-id="d242f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d242f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d242f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d242f-109">Permission type</span></span>      | <span data-ttu-id="d242f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d242f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d242f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d242f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d242f-112">AdministrativeUnit、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="d242f-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d242f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d242f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d242f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d242f-114">Not supported.</span></span>    |
|<span data-ttu-id="d242f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d242f-115">Application</span></span> | <span data-ttu-id="d242f-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d242f-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d242f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d242f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits

```
## <a name="request-headers"></a><span data-ttu-id="d242f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d242f-118">Request headers</span></span>
| <span data-ttu-id="d242f-119">名称</span><span class="sxs-lookup"><span data-stu-id="d242f-119">Name</span></span>      |<span data-ttu-id="d242f-120">说明</span><span class="sxs-lookup"><span data-stu-id="d242f-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d242f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d242f-121">Authorization</span></span>  | <span data-ttu-id="d242f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d242f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d242f-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="d242f-124">Content-type</span></span> | <span data-ttu-id="d242f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d242f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d242f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d242f-127">Request body</span></span>
<span data-ttu-id="d242f-128">在请求正文中，提供 [administrativeUnit](../resources/administrativeunit.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d242f-128">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

<span data-ttu-id="d242f-129">由于 **administrativeUnit** 资源支持 [扩展](/graph/extensibility-overview)，因此您可以使用 `POST` 操作，并在创建自定义属性时将自己的数据添加到管理单元中。</span><span class="sxs-lookup"><span data-stu-id="d242f-129">Because the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the administrative unit while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="d242f-130">响应</span><span class="sxs-lookup"><span data-stu-id="d242f-130">Response</span></span>

<span data-ttu-id="d242f-131">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d242f-131">If successful, this method returns a `201 Created` response code and an [administrativeUnit](../resources/administrativeunit.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d242f-132">示例</span><span class="sxs-lookup"><span data-stu-id="d242f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d242f-133">请求</span><span class="sxs-lookup"><span data-stu-id="d242f-133">Request</span></span>

<span data-ttu-id="d242f-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d242f-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d242f-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d242f-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d242f-136">C#</span><span class="sxs-lookup"><span data-stu-id="d242f-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-administrativeunit-from-administrativeunits-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d242f-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d242f-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-administrativeunit-from-administrativeunits-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d242f-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d242f-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-administrativeunit-from-administrativeunits-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="d242f-139">在请求正文中，提供 [administrativeUnit](../resources/administrativeunit.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d242f-139">In the request body, supply a JSON representation of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="d242f-140">响应</span><span class="sxs-lookup"><span data-stu-id="d242f-140">Response</span></span>

<span data-ttu-id="d242f-141">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="d242f-141">The following is an example of the response.</span></span> 
> <span data-ttu-id="d242f-142">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d242f-142">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="d242f-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d242f-143">All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="d242f-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d242f-144">See also</span></span>

- [<span data-ttu-id="d242f-145">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d242f-145">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d242f-146">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="d242f-146">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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


