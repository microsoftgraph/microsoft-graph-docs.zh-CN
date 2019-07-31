---
title: 更新 schemaExtension
description: 更新指定 schemaExtension 的定义中的属性。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: deb87928753794db7cc87d93694c0bf97c0c17f4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35982942"
---
# <a name="update-schemaextension"></a><span data-ttu-id="92425-103">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="92425-103">Update schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92425-104">更新指定[schemaExtension](../resources/schemaextension.md)的定义中的属性。</span><span class="sxs-lookup"><span data-stu-id="92425-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="92425-105">更新适用于扩展的**targetTypes**属性中包含的所有资源。</span><span class="sxs-lookup"><span data-stu-id="92425-105">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="92425-106">这些资源是[支持资源类型](/graph/extensibility-overview#supported-resources)中的一种。</span><span class="sxs-lookup"><span data-stu-id="92425-106">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="92425-107">只有创建了架构扩展 (所有者应用程序) 的应用程序可以在扩展处于**InDevelopment**或**可用**状态时对扩展进行增量更新。</span><span class="sxs-lookup"><span data-stu-id="92425-107">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="92425-108">这意味着应用程序无法从定义中删除自定义属性或目标资源类型。</span><span class="sxs-lookup"><span data-stu-id="92425-108">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="92425-109">但是, 该应用程序可以更改扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="92425-109">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="92425-110">权限</span><span class="sxs-lookup"><span data-stu-id="92425-110">Permissions</span></span>

<span data-ttu-id="92425-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92425-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="92425-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="92425-113">Permission type</span></span>      | <span data-ttu-id="92425-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92425-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92425-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92425-115">Delegated (work or school account)</span></span> | <span data-ttu-id="92425-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="92425-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="92425-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92425-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92425-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="92425-118">Not supported.</span></span>    |
|<span data-ttu-id="92425-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="92425-119">Application</span></span> | <span data-ttu-id="92425-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="92425-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92425-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92425-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="92425-122">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="92425-122">Optional request headers</span></span>

| <span data-ttu-id="92425-123">名称</span><span class="sxs-lookup"><span data-stu-id="92425-123">Name</span></span>      |<span data-ttu-id="92425-124">说明</span><span class="sxs-lookup"><span data-stu-id="92425-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="92425-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="92425-125">Authorization</span></span>  | <span data-ttu-id="92425-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92425-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="92425-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="92425-128">Content-Type</span></span>   | <span data-ttu-id="92425-129">application/json</span><span class="sxs-lookup"><span data-stu-id="92425-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="92425-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="92425-130">Request body</span></span>

<span data-ttu-id="92425-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="92425-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="92425-134">属性</span><span class="sxs-lookup"><span data-stu-id="92425-134">Property</span></span>   | <span data-ttu-id="92425-135">类型</span><span class="sxs-lookup"><span data-stu-id="92425-135">Type</span></span> |<span data-ttu-id="92425-136">说明</span><span class="sxs-lookup"><span data-stu-id="92425-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92425-137">说明</span><span class="sxs-lookup"><span data-stu-id="92425-137">description</span></span>|<span data-ttu-id="92425-138">String</span><span class="sxs-lookup"><span data-stu-id="92425-138">String</span></span>|<span data-ttu-id="92425-139">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="92425-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="92425-140">properties</span><span class="sxs-lookup"><span data-stu-id="92425-140">properties</span></span>|<span data-ttu-id="92425-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92425-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="92425-142">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="92425-142">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="92425-143">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="92425-143">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="92425-144">status</span><span class="sxs-lookup"><span data-stu-id="92425-144">status</span></span>|<span data-ttu-id="92425-145">String</span><span class="sxs-lookup"><span data-stu-id="92425-145">String</span></span>|<span data-ttu-id="92425-146">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="92425-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="92425-147">创建时的初始状态为**InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="92425-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="92425-148">可能的状态过渡从**InDevelopment**到**可用**, 并**可供\*\*\*\*弃用**。</span><span class="sxs-lookup"><span data-stu-id="92425-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="92425-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="92425-149">targetTypes</span></span>|<span data-ttu-id="92425-150">String collection</span><span class="sxs-lookup"><span data-stu-id="92425-150">String collection</span></span>|<span data-ttu-id="92425-151">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="92425-151">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="92425-152">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="92425-152">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="92425-153">响应</span><span class="sxs-lookup"><span data-stu-id="92425-153">Response</span></span>

<span data-ttu-id="92425-154">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="92425-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="92425-155">示例</span><span class="sxs-lookup"><span data-stu-id="92425-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="92425-156">请求</span><span class="sxs-lookup"><span data-stu-id="92425-156">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="92425-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="92425-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="92425-158">C#</span><span class="sxs-lookup"><span data-stu-id="92425-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="92425-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="92425-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="92425-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="92425-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="92425-161">Java</span><span class="sxs-lookup"><span data-stu-id="92425-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="92425-162">响应</span><span class="sxs-lookup"><span data-stu-id="92425-162">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="92425-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="92425-163">See also</span></span>

- [<span data-ttu-id="92425-164">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="92425-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="92425-165">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="92425-165">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
