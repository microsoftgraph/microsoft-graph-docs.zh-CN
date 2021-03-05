---
title: 更新管理单元
description: 更新 administrativeUnit 对象的属性。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 195ae89d8f32659f975be172fcf586f0cc7a02eb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442570"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="70742-103">更新管理单元</span><span class="sxs-lookup"><span data-stu-id="70742-103">Update administrativeunit</span></span>

<span data-ttu-id="70742-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70742-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="70742-105">更新 [administrativeUnit 对象](../resources/administrativeunit.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="70742-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="70742-106">权限</span><span class="sxs-lookup"><span data-stu-id="70742-106">Permissions</span></span>
<span data-ttu-id="70742-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70742-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="70742-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70742-109">Permission type</span></span>      | <span data-ttu-id="70742-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70742-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70742-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70742-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70742-112">AdministrativeUnit.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="70742-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="70742-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70742-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70742-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="70742-114">Not supported.</span></span>    |
|<span data-ttu-id="70742-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="70742-115">Application</span></span> | <span data-ttu-id="70742-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70742-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70742-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70742-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /directory/administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70742-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="70742-118">Request headers</span></span>

| <span data-ttu-id="70742-119">名称</span><span class="sxs-lookup"><span data-stu-id="70742-119">Name</span></span>      |<span data-ttu-id="70742-120">说明</span><span class="sxs-lookup"><span data-stu-id="70742-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="70742-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70742-121">Authorization</span></span>  | <span data-ttu-id="70742-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70742-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70742-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="70742-124">Request body</span></span>

<span data-ttu-id="70742-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="70742-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="70742-128">属性</span><span class="sxs-lookup"><span data-stu-id="70742-128">Property</span></span>   | <span data-ttu-id="70742-129">类型</span><span class="sxs-lookup"><span data-stu-id="70742-129">Type</span></span> |<span data-ttu-id="70742-130">说明</span><span class="sxs-lookup"><span data-stu-id="70742-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70742-131">说明</span><span class="sxs-lookup"><span data-stu-id="70742-131">description</span></span>|<span data-ttu-id="70742-132">string</span><span class="sxs-lookup"><span data-stu-id="70742-132">string</span></span>|<span data-ttu-id="70742-133">管理单元的说明。</span><span class="sxs-lookup"><span data-stu-id="70742-133">Description for the administrative unit.</span></span>|
|<span data-ttu-id="70742-134">displayName</span><span class="sxs-lookup"><span data-stu-id="70742-134">displayName</span></span>|<span data-ttu-id="70742-135">string</span><span class="sxs-lookup"><span data-stu-id="70742-135">string</span></span>|<span data-ttu-id="70742-136">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="70742-136">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="70742-137">visibility</span><span class="sxs-lookup"><span data-stu-id="70742-137">visibility</span></span>|<span data-ttu-id="70742-138">string</span><span class="sxs-lookup"><span data-stu-id="70742-138">string</span></span>|<span data-ttu-id="70742-139">管理单元的可见性。</span><span class="sxs-lookup"><span data-stu-id="70742-139">Visibility for the administrative unit.</span></span> <span data-ttu-id="70742-140">如果未设置，则默认值为"public"。</span><span class="sxs-lookup"><span data-stu-id="70742-140">If not set then the default is "public".</span></span> <span data-ttu-id="70742-141">可以设置为"HiddenMembership"，这将对非成员隐藏成员身份。</span><span class="sxs-lookup"><span data-stu-id="70742-141">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="70742-142">由于 **administrativeUnit** 资源 [](/graph/extensibility-overview)支持扩展，因此可以使用该操作在现有 administrativeUnit 实例中扩展的自定义属性中添加、更新或删除你自己的特定于 `PATCH` **应用** 的数据。</span><span class="sxs-lookup"><span data-stu-id="70742-142">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="70742-143">响应</span><span class="sxs-lookup"><span data-stu-id="70742-143">Response</span></span>

<span data-ttu-id="70742-144">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="70742-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="70742-145">示例</span><span class="sxs-lookup"><span data-stu-id="70742-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="70742-146">请求</span><span class="sxs-lookup"><span data-stu-id="70742-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="70742-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="70742-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="70742-148">C#</span><span class="sxs-lookup"><span data-stu-id="70742-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70742-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70742-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70742-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70742-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70742-151">Java</span><span class="sxs-lookup"><span data-stu-id="70742-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


##### <a name="response"></a><span data-ttu-id="70742-152">响应</span><span class="sxs-lookup"><span data-stu-id="70742-152">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="70742-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="70742-153">See also</span></span>

- [<span data-ttu-id="70742-154">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="70742-154">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="70742-155">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="70742-155">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
