---
title: 更新 administrativeunit
description: 更新 administrativeUnit 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 30d8470c16e2d7556b65ea797b2298025cfc74d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441688"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="d52ea-103">更新 administrativeunit</span><span class="sxs-lookup"><span data-stu-id="d52ea-103">Update administrativeunit</span></span>

<span data-ttu-id="d52ea-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d52ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d52ea-105">更新[administrativeUnit](../resources/administrativeunit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d52ea-105">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d52ea-106">权限</span><span class="sxs-lookup"><span data-stu-id="d52ea-106">Permissions</span></span>
<span data-ttu-id="d52ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d52ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d52ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d52ea-109">Permission type</span></span>      | <span data-ttu-id="d52ea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d52ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d52ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d52ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d52ea-112">AdministrativeUnit、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="d52ea-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d52ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d52ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d52ea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d52ea-114">Not supported.</span></span>    |
|<span data-ttu-id="d52ea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d52ea-115">Application</span></span> | <span data-ttu-id="d52ea-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52ea-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d52ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d52ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d52ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d52ea-118">Request headers</span></span>

| <span data-ttu-id="d52ea-119">名称</span><span class="sxs-lookup"><span data-stu-id="d52ea-119">Name</span></span>      |<span data-ttu-id="d52ea-120">说明</span><span class="sxs-lookup"><span data-stu-id="d52ea-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d52ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d52ea-121">Authorization</span></span>  | <span data-ttu-id="d52ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d52ea-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d52ea-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="d52ea-124">Request body</span></span>

<span data-ttu-id="d52ea-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="d52ea-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d52ea-128">属性</span><span class="sxs-lookup"><span data-stu-id="d52ea-128">Property</span></span>   | <span data-ttu-id="d52ea-129">类型</span><span class="sxs-lookup"><span data-stu-id="d52ea-129">Type</span></span> |<span data-ttu-id="d52ea-130">说明</span><span class="sxs-lookup"><span data-stu-id="d52ea-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d52ea-131">说明</span><span class="sxs-lookup"><span data-stu-id="d52ea-131">description</span></span>|<span data-ttu-id="d52ea-132">string</span><span class="sxs-lookup"><span data-stu-id="d52ea-132">string</span></span>|<span data-ttu-id="d52ea-133">管理单元的说明。</span><span class="sxs-lookup"><span data-stu-id="d52ea-133">Description for the administrative unit.</span></span>|
|<span data-ttu-id="d52ea-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d52ea-134">displayName</span></span>|<span data-ttu-id="d52ea-135">string</span><span class="sxs-lookup"><span data-stu-id="d52ea-135">string</span></span>|<span data-ttu-id="d52ea-136">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d52ea-136">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="d52ea-137">visibility</span><span class="sxs-lookup"><span data-stu-id="d52ea-137">visibility</span></span>|<span data-ttu-id="d52ea-138">string</span><span class="sxs-lookup"><span data-stu-id="d52ea-138">string</span></span>|<span data-ttu-id="d52ea-139">管理单元的可见性。</span><span class="sxs-lookup"><span data-stu-id="d52ea-139">Visibility for the administrative unit.</span></span> <span data-ttu-id="d52ea-140">如果未设置，则默认值为 "public"。</span><span class="sxs-lookup"><span data-stu-id="d52ea-140">If not set then the default is "public".</span></span> <span data-ttu-id="d52ea-141">可以设置为 "HiddenMembership"，这将隐藏非成员的成员资格。</span><span class="sxs-lookup"><span data-stu-id="d52ea-141">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="d52ea-142">由于**administrativeUnit**资源支持[扩展](/graph/extensibility-overview)，因此您可以使用该`PATCH`操作在现有**administrativeUnit**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="d52ea-142">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="d52ea-143">响应</span><span class="sxs-lookup"><span data-stu-id="d52ea-143">Response</span></span>

<span data-ttu-id="d52ea-144">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d52ea-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d52ea-145">示例</span><span class="sxs-lookup"><span data-stu-id="d52ea-145">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d52ea-146">请求</span><span class="sxs-lookup"><span data-stu-id="d52ea-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="d52ea-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="d52ea-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```
# <a name="c"></a>[<span data-ttu-id="d52ea-148">C#</span><span class="sxs-lookup"><span data-stu-id="d52ea-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d52ea-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d52ea-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d52ea-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d52ea-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d52ea-151">响应</span><span class="sxs-lookup"><span data-stu-id="d52ea-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="d52ea-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d52ea-152">See also</span></span>

- [<span data-ttu-id="d52ea-153">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="d52ea-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="d52ea-154">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="d52ea-154">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
