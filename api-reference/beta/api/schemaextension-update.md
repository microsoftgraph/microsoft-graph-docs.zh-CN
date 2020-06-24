---
title: 更新 schemaExtension
description: 更新指定 schemaExtension 的定义中的属性。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: 083e3a998ddacd25c9a29e19ccf07be66e23f594
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862475"
---
# <a name="update-schemaextension"></a><span data-ttu-id="29a8e-103">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="29a8e-103">Update schemaExtension</span></span>

<span data-ttu-id="29a8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29a8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29a8e-105">更新指定[schemaExtension](../resources/schemaextension.md)的定义中的属性。</span><span class="sxs-lookup"><span data-stu-id="29a8e-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="29a8e-106">更新适用于扩展的**targetTypes**属性中包含的所有资源。</span><span class="sxs-lookup"><span data-stu-id="29a8e-106">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="29a8e-107">这些资源是[支持资源类型](/graph/extensibility-overview#supported-resources)中的一种。</span><span class="sxs-lookup"><span data-stu-id="29a8e-107">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="29a8e-108">只有创建了架构扩展（所有者应用程序）的应用程序可以在扩展处于**InDevelopment**或**可用**状态时对扩展进行增量更新。</span><span class="sxs-lookup"><span data-stu-id="29a8e-108">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="29a8e-109">这意味着应用程序无法从定义中删除自定义属性或目标资源类型。</span><span class="sxs-lookup"><span data-stu-id="29a8e-109">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="29a8e-110">但是，该应用程序可以更改扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="29a8e-110">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="29a8e-111">权限</span><span class="sxs-lookup"><span data-stu-id="29a8e-111">Permissions</span></span>

<span data-ttu-id="29a8e-112">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="29a8e-112">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="29a8e-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29a8e-113">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="29a8e-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="29a8e-114">Permission type</span></span>      | <span data-ttu-id="29a8e-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29a8e-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29a8e-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29a8e-116">Delegated (work or school account)</span></span> | <span data-ttu-id="29a8e-117">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="29a8e-117">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="29a8e-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29a8e-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="29a8e-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="29a8e-119">Not supported.</span></span>    |
|<span data-ttu-id="29a8e-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="29a8e-120">Application</span></span> | <span data-ttu-id="29a8e-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="29a8e-121">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="29a8e-122">此外，对于委派的流程，登录用户只能更新自己拥有的 Schemaextension （其中 schemaExtension 的**owner**属性是 `appId` 登录用户拥有的应用程序的）。</span><span class="sxs-lookup"><span data-stu-id="29a8e-122">Additionally for the delegated flow, the signed-in user can only update schemaExtensions they own (where the **owner** property of the schemaExtension is the `appId` of an application the signed-in user owns).</span></span>

## <a name="http-request"></a><span data-ttu-id="29a8e-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29a8e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="29a8e-124">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="29a8e-124">Optional request headers</span></span>

| <span data-ttu-id="29a8e-125">名称</span><span class="sxs-lookup"><span data-stu-id="29a8e-125">Name</span></span>      |<span data-ttu-id="29a8e-126">说明</span><span class="sxs-lookup"><span data-stu-id="29a8e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="29a8e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="29a8e-127">Authorization</span></span>  | <span data-ttu-id="29a8e-128">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="29a8e-128">Bearer {token}.</span></span> <span data-ttu-id="29a8e-129">Required.</span><span class="sxs-lookup"><span data-stu-id="29a8e-129">Required.</span></span> |
| <span data-ttu-id="29a8e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="29a8e-130">Content-Type</span></span>   | <span data-ttu-id="29a8e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="29a8e-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="29a8e-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="29a8e-132">Request body</span></span>

<span data-ttu-id="29a8e-133">In the request body, supply the values for relevant fields that should be updated.</span><span class="sxs-lookup"><span data-stu-id="29a8e-133">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="29a8e-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span><span class="sxs-lookup"><span data-stu-id="29a8e-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="29a8e-135">For best performance you shouldn't include existing values that haven't changed.</span><span class="sxs-lookup"><span data-stu-id="29a8e-135">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="29a8e-136">属性</span><span class="sxs-lookup"><span data-stu-id="29a8e-136">Property</span></span>   | <span data-ttu-id="29a8e-137">类型</span><span class="sxs-lookup"><span data-stu-id="29a8e-137">Type</span></span> |<span data-ttu-id="29a8e-138">Description</span><span class="sxs-lookup"><span data-stu-id="29a8e-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29a8e-139">说明</span><span class="sxs-lookup"><span data-stu-id="29a8e-139">description</span></span>|<span data-ttu-id="29a8e-140">String</span><span class="sxs-lookup"><span data-stu-id="29a8e-140">String</span></span>|<span data-ttu-id="29a8e-141">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="29a8e-141">Description for the schema extension.</span></span>|
|<span data-ttu-id="29a8e-142">properties</span><span class="sxs-lookup"><span data-stu-id="29a8e-142">properties</span></span>|<span data-ttu-id="29a8e-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="29a8e-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="29a8e-144">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="29a8e-144">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="29a8e-145">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="29a8e-145">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="29a8e-146">status</span><span class="sxs-lookup"><span data-stu-id="29a8e-146">status</span></span>|<span data-ttu-id="29a8e-147">String</span><span class="sxs-lookup"><span data-stu-id="29a8e-147">String</span></span>|<span data-ttu-id="29a8e-148">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="29a8e-148">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="29a8e-149">创建时的初始状态为**InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="29a8e-149">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="29a8e-150">可能的状态过渡从**InDevelopment**到**可用**，并**可供\*\*\*\*弃用**。</span><span class="sxs-lookup"><span data-stu-id="29a8e-150">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="29a8e-151">targetTypes</span><span class="sxs-lookup"><span data-stu-id="29a8e-151">targetTypes</span></span>|<span data-ttu-id="29a8e-152">String collection</span><span class="sxs-lookup"><span data-stu-id="29a8e-152">String collection</span></span>|<span data-ttu-id="29a8e-153">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="29a8e-153">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="29a8e-154">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="29a8e-154">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="29a8e-155">响应</span><span class="sxs-lookup"><span data-stu-id="29a8e-155">Response</span></span>

<span data-ttu-id="29a8e-156">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="29a8e-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="29a8e-157">示例</span><span class="sxs-lookup"><span data-stu-id="29a8e-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="29a8e-158">请求</span><span class="sxs-lookup"><span data-stu-id="29a8e-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29a8e-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="29a8e-159">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="29a8e-160">C#</span><span class="sxs-lookup"><span data-stu-id="29a8e-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29a8e-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29a8e-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29a8e-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29a8e-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="29a8e-163">响应</span><span class="sxs-lookup"><span data-stu-id="29a8e-163">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="29a8e-164">另请参阅</span><span class="sxs-lookup"><span data-stu-id="29a8e-164">See also</span></span>

- [<span data-ttu-id="29a8e-165">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="29a8e-165">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="29a8e-166">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="29a8e-166">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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
