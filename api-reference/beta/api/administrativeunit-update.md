---
title: 更新 administrativeunit
description: 更新 administrativeUnit 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 664a0f5a05b06e78aa2e54db0d7b8ff99a8f148c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318920"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="499ba-103">更新 administrativeunit</span><span class="sxs-lookup"><span data-stu-id="499ba-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="499ba-104">更新[administrativeUnit](../resources/administrativeunit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="499ba-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="499ba-105">权限</span><span class="sxs-lookup"><span data-stu-id="499ba-105">Permissions</span></span>
<span data-ttu-id="499ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="499ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="499ba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="499ba-108">Permission type</span></span>      | <span data-ttu-id="499ba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="499ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="499ba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="499ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="499ba-111">AdministrativeUnit、Directory.accessasuser.all 和所有</span><span class="sxs-lookup"><span data-stu-id="499ba-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="499ba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="499ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="499ba-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="499ba-113">Not supported.</span></span>    |
|<span data-ttu-id="499ba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="499ba-114">Application</span></span> | <span data-ttu-id="499ba-115">AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="499ba-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="499ba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="499ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="499ba-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="499ba-117">Request headers</span></span>

| <span data-ttu-id="499ba-118">名称</span><span class="sxs-lookup"><span data-stu-id="499ba-118">Name</span></span>      |<span data-ttu-id="499ba-119">说明</span><span class="sxs-lookup"><span data-stu-id="499ba-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="499ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="499ba-120">Authorization</span></span>  | <span data-ttu-id="499ba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="499ba-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="499ba-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="499ba-123">Request body</span></span>

<span data-ttu-id="499ba-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="499ba-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="499ba-127">属性</span><span class="sxs-lookup"><span data-stu-id="499ba-127">Property</span></span>   | <span data-ttu-id="499ba-128">类型</span><span class="sxs-lookup"><span data-stu-id="499ba-128">Type</span></span> |<span data-ttu-id="499ba-129">说明</span><span class="sxs-lookup"><span data-stu-id="499ba-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="499ba-130">说明</span><span class="sxs-lookup"><span data-stu-id="499ba-130">description</span></span>|<span data-ttu-id="499ba-131">string</span><span class="sxs-lookup"><span data-stu-id="499ba-131">string</span></span>|<span data-ttu-id="499ba-132">管理单元的说明。</span><span class="sxs-lookup"><span data-stu-id="499ba-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="499ba-133">displayName</span><span class="sxs-lookup"><span data-stu-id="499ba-133">displayName</span></span>|<span data-ttu-id="499ba-134">string</span><span class="sxs-lookup"><span data-stu-id="499ba-134">string</span></span>|<span data-ttu-id="499ba-135">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="499ba-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="499ba-136">visibility</span><span class="sxs-lookup"><span data-stu-id="499ba-136">visibility</span></span>|<span data-ttu-id="499ba-137">string</span><span class="sxs-lookup"><span data-stu-id="499ba-137">string</span></span>|<span data-ttu-id="499ba-138">管理单元的可见性。</span><span class="sxs-lookup"><span data-stu-id="499ba-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="499ba-139">如果未设置, 则默认值为 "public"。</span><span class="sxs-lookup"><span data-stu-id="499ba-139">If not set then the default is "public".</span></span> <span data-ttu-id="499ba-140">可以设置为 "HiddenMembership", 这将隐藏非成员的成员资格。</span><span class="sxs-lookup"><span data-stu-id="499ba-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="499ba-141">由于**administrativeUnit**资源支持[扩展](/graph/extensibility-overview), 因此您可以使用该`PATCH`操作在现有**administrativeUnit**实例中的扩展的自定义属性中添加、更新或删除您自己的应用程序特定的数据。</span><span class="sxs-lookup"><span data-stu-id="499ba-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="499ba-142">响应</span><span class="sxs-lookup"><span data-stu-id="499ba-142">Response</span></span>

<span data-ttu-id="499ba-143">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="499ba-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="499ba-144">示例</span><span class="sxs-lookup"><span data-stu-id="499ba-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="499ba-145">请求</span><span class="sxs-lookup"><span data-stu-id="499ba-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="499ba-146">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="499ba-146">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="499ba-147">C#</span><span class="sxs-lookup"><span data-stu-id="499ba-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="499ba-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="499ba-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="499ba-149">目标-C</span><span class="sxs-lookup"><span data-stu-id="499ba-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="499ba-150">Java</span><span class="sxs-lookup"><span data-stu-id="499ba-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="499ba-151">响应</span><span class="sxs-lookup"><span data-stu-id="499ba-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="499ba-152">另请参阅</span><span class="sxs-lookup"><span data-stu-id="499ba-152">See also</span></span>

- [<span data-ttu-id="499ba-153">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="499ba-153">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="499ba-154">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="499ba-154">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
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
