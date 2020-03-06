---
title: 更新 schemaExtension
description: 更新指定 schemaExtension 的定义中的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c1e6e58c19f6561c16f51967a3b3a0c4ae346158
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509939"
---
# <a name="update-schemaextension"></a><span data-ttu-id="c675e-103">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="c675e-103">Update schemaExtension</span></span>

<span data-ttu-id="c675e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c675e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c675e-105">更新指定[schemaExtension](../resources/schemaextension.md)的定义中的属性。</span><span class="sxs-lookup"><span data-stu-id="c675e-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="c675e-106">更新适用于扩展的**targetTypes**属性中包含的所有资源。</span><span class="sxs-lookup"><span data-stu-id="c675e-106">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="c675e-107">这些资源是[支持资源类型](/graph/extensibility-overview#supported-resources)中的一种。</span><span class="sxs-lookup"><span data-stu-id="c675e-107">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="c675e-108">只有创建了架构扩展（所有者应用程序）的应用程序可以在扩展处于**InDevelopment**或**可用**状态时对扩展进行增量更新。</span><span class="sxs-lookup"><span data-stu-id="c675e-108">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="c675e-109">这意味着应用程序无法从定义中删除自定义属性或目标资源类型。</span><span class="sxs-lookup"><span data-stu-id="c675e-109">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="c675e-110">但是，该应用程序可以更改扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="c675e-110">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="c675e-111">权限</span><span class="sxs-lookup"><span data-stu-id="c675e-111">Permissions</span></span>
<span data-ttu-id="c675e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c675e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c675e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="c675e-114">Permission type</span></span>      | <span data-ttu-id="c675e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c675e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c675e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c675e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c675e-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c675e-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c675e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c675e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c675e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="c675e-119">Not supported.</span></span>    |
|<span data-ttu-id="c675e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="c675e-120">Application</span></span> | <span data-ttu-id="c675e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="c675e-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c675e-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c675e-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="c675e-123">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="c675e-123">Optional request headers</span></span>

| <span data-ttu-id="c675e-124">名称</span><span class="sxs-lookup"><span data-stu-id="c675e-124">Name</span></span>      |<span data-ttu-id="c675e-125">说明</span><span class="sxs-lookup"><span data-stu-id="c675e-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c675e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c675e-126">Authorization</span></span>  | <span data-ttu-id="c675e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c675e-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c675e-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c675e-129">Content-Type</span></span>   | <span data-ttu-id="c675e-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c675e-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c675e-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c675e-131">Request body</span></span>

<span data-ttu-id="c675e-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c675e-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c675e-135">属性</span><span class="sxs-lookup"><span data-stu-id="c675e-135">Property</span></span>   | <span data-ttu-id="c675e-136">类型</span><span class="sxs-lookup"><span data-stu-id="c675e-136">Type</span></span> |<span data-ttu-id="c675e-137">说明</span><span class="sxs-lookup"><span data-stu-id="c675e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c675e-138">说明</span><span class="sxs-lookup"><span data-stu-id="c675e-138">description</span></span>|<span data-ttu-id="c675e-139">String</span><span class="sxs-lookup"><span data-stu-id="c675e-139">String</span></span>|<span data-ttu-id="c675e-140">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="c675e-140">Description for the schema extension.</span></span>|
|<span data-ttu-id="c675e-141">properties</span><span class="sxs-lookup"><span data-stu-id="c675e-141">properties</span></span>|<span data-ttu-id="c675e-142">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c675e-142">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="c675e-143">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="c675e-143">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="c675e-144">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="c675e-144">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="c675e-145">状态</span><span class="sxs-lookup"><span data-stu-id="c675e-145">status</span></span>|<span data-ttu-id="c675e-146">String</span><span class="sxs-lookup"><span data-stu-id="c675e-146">String</span></span>|<span data-ttu-id="c675e-147">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="c675e-147">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="c675e-148">创建时的初始状态为**InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="c675e-148">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="c675e-149">可能的状态过渡从**InDevelopment**到**可用**，并**可供\*\*\*\*弃用**。</span><span class="sxs-lookup"><span data-stu-id="c675e-149">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="c675e-150">targetTypes</span><span class="sxs-lookup"><span data-stu-id="c675e-150">targetTypes</span></span>|<span data-ttu-id="c675e-151">String collection</span><span class="sxs-lookup"><span data-stu-id="c675e-151">String collection</span></span>|<span data-ttu-id="c675e-152">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="c675e-152">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="c675e-153">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="c675e-153">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="c675e-154">响应</span><span class="sxs-lookup"><span data-stu-id="c675e-154">Response</span></span>

<span data-ttu-id="c675e-155">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c675e-155">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c675e-156">示例</span><span class="sxs-lookup"><span data-stu-id="c675e-156">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c675e-157">请求</span><span class="sxs-lookup"><span data-stu-id="c675e-157">Request</span></span>

<span data-ttu-id="c675e-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c675e-158">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c675e-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="c675e-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
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
# <a name="c"></a>[<span data-ttu-id="c675e-160">C#</span><span class="sxs-lookup"><span data-stu-id="c675e-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c675e-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c675e-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c675e-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c675e-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c675e-163">Java</span><span class="sxs-lookup"><span data-stu-id="c675e-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c675e-164">响应</span><span class="sxs-lookup"><span data-stu-id="c675e-164">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="c675e-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c675e-165">See also</span></span>

- [<span data-ttu-id="c675e-166">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c675e-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c675e-167">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c675e-167">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
