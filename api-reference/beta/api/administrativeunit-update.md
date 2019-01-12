---
title: 更新 administrativeunit
description: 更新 administrativeUnit 对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cd82035e06fbd6135f4d2f6cbb7f6dfae9576f9a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932012"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="fab90-103">更新 administrativeunit</span><span class="sxs-lookup"><span data-stu-id="fab90-103">Update administrativeunit</span></span>

> <span data-ttu-id="fab90-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fab90-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fab90-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fab90-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fab90-106">更新[administrativeUnit](../resources/administrativeunit.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fab90-106">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fab90-107">权限</span><span class="sxs-lookup"><span data-stu-id="fab90-107">Permissions</span></span>
<span data-ttu-id="fab90-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fab90-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fab90-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fab90-110">Permission type</span></span>      | <span data-ttu-id="fab90-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fab90-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fab90-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fab90-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fab90-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fab90-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fab90-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fab90-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fab90-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fab90-115">Not supported.</span></span>    |
|<span data-ttu-id="fab90-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fab90-116">Application</span></span> | <span data-ttu-id="fab90-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fab90-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fab90-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fab90-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fab90-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fab90-119">Request headers</span></span>

| <span data-ttu-id="fab90-120">名称</span><span class="sxs-lookup"><span data-stu-id="fab90-120">Name</span></span>      |<span data-ttu-id="fab90-121">说明</span><span class="sxs-lookup"><span data-stu-id="fab90-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fab90-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fab90-122">Authorization</span></span>  | <span data-ttu-id="fab90-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fab90-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fab90-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fab90-125">Request body</span></span>

<span data-ttu-id="fab90-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="fab90-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fab90-129">属性</span><span class="sxs-lookup"><span data-stu-id="fab90-129">Property</span></span>   | <span data-ttu-id="fab90-130">类型</span><span class="sxs-lookup"><span data-stu-id="fab90-130">Type</span></span> |<span data-ttu-id="fab90-131">说明</span><span class="sxs-lookup"><span data-stu-id="fab90-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fab90-132">说明</span><span class="sxs-lookup"><span data-stu-id="fab90-132">description</span></span>|<span data-ttu-id="fab90-133">string</span><span class="sxs-lookup"><span data-stu-id="fab90-133">string</span></span>|<span data-ttu-id="fab90-134">管理单元的说明。</span><span class="sxs-lookup"><span data-stu-id="fab90-134">Description for the administrative unit.</span></span>|
|<span data-ttu-id="fab90-135">displayName</span><span class="sxs-lookup"><span data-stu-id="fab90-135">displayName</span></span>|<span data-ttu-id="fab90-136">string</span><span class="sxs-lookup"><span data-stu-id="fab90-136">string</span></span>|<span data-ttu-id="fab90-137">管理单元的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fab90-137">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="fab90-138">visibility</span><span class="sxs-lookup"><span data-stu-id="fab90-138">visibility</span></span>|<span data-ttu-id="fab90-139">string</span><span class="sxs-lookup"><span data-stu-id="fab90-139">string</span></span>|<span data-ttu-id="fab90-140">可见性管理单元。</span><span class="sxs-lookup"><span data-stu-id="fab90-140">Visibility for the administrative unit.</span></span> <span data-ttu-id="fab90-141">如果，未设置默认值为"公共"。</span><span class="sxs-lookup"><span data-stu-id="fab90-141">If not set then the default is "public".</span></span> <span data-ttu-id="fab90-142">可以设置为"HiddenMembership"，隐藏从非成员的成员身份。</span><span class="sxs-lookup"><span data-stu-id="fab90-142">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="fab90-143">由于**administrativeUnit**资源支持[扩展](/graph/extensibility-overview)，您可以使用`PATCH`操作添加、 更新或删除您自己的扩展现有**administrativeUnit**实例中的自定义属性中的特定于应用程序的数据。</span><span class="sxs-lookup"><span data-stu-id="fab90-143">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="fab90-144">响应</span><span class="sxs-lookup"><span data-stu-id="fab90-144">Response</span></span>

<span data-ttu-id="fab90-145">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="fab90-145">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fab90-146">示例</span><span class="sxs-lookup"><span data-stu-id="fab90-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fab90-147">请求</span><span class="sxs-lookup"><span data-stu-id="fab90-147">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="fab90-148">响应</span><span class="sxs-lookup"><span data-stu-id="fab90-148">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="fab90-149">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fab90-149">See also</span></span>

- [<span data-ttu-id="fab90-150">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fab90-150">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fab90-151">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="fab90-151">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
