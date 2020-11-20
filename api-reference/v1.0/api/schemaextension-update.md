---
title: 更新 schemaExtension
description: 更新指定 schemaExtension 的定义中的属性。
localization_priority: Normal
author: dkershaw10
ms.prod: extensions
doc_type: apiPageType
ms.openlocfilehash: ac657ee517a11201cab50c8aa161ad20c9352ff8
ms.sourcegitcommit: ea3b1a8b781a347015d9542826c5c0c24d50d35d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49352442"
---
# <a name="update-schemaextension"></a><span data-ttu-id="ddd22-103">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="ddd22-103">Update schemaExtension</span></span>

<span data-ttu-id="ddd22-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddd22-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddd22-105">更新指定 [schemaExtension](../resources/schemaextension.md)的定义中的属性。</span><span class="sxs-lookup"><span data-stu-id="ddd22-105">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span> 

<span data-ttu-id="ddd22-106">这意味着无法从定义中删除自定义属性或目标资源类型，但可以添加新的自定义属性，并更改扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="ddd22-106">This means custom properties or target resource types cannot be removed from the definition, but new custom properties can be added and the description of the extension changed.</span></span>

<span data-ttu-id="ddd22-107">仅当扩展处于 **InDevelopment** 或 **可用** 状态时，才可对扩展进行累加性更新。</span><span class="sxs-lookup"><span data-stu-id="ddd22-107">Additive updates to the extension can only be made when the extension is in the **InDevelopment** or **Available** status.</span></span> 

<span data-ttu-id="ddd22-108">更新适用于扩展的 **targetTypes** 属性中包含的所有资源。</span><span class="sxs-lookup"><span data-stu-id="ddd22-108">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="ddd22-109">这些资源是 [支持资源类型](/graph/extensibility-overview#supported-resources)中的一种。</span><span class="sxs-lookup"><span data-stu-id="ddd22-109">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="ddd22-110">对于委派的流，只要扩展的 **owner** 属性设置为已登录用户拥有的应用程序的 **appId** ，登录用户就可以更新架构扩展。</span><span class="sxs-lookup"><span data-stu-id="ddd22-110">For delegated flows, the signed-in user can update a schema extension as long as the **owner** property of the extension is set to the **appId** of an application the signed-in user owns.</span></span> <span data-ttu-id="ddd22-111">该应用程序可以是最初创建扩展的应用程序，也可以是由登录用户拥有的其他应用程序。</span><span class="sxs-lookup"><span data-stu-id="ddd22-111">That application can be the one that initially created the extension, or some other application owned by the signed-in user.</span></span> 

<span data-ttu-id="ddd22-112">**Owner** 属性的此条件允许登录用户通过不拥有的其他应用程序（如 Microsoft Graph 资源管理器）进行更新。</span><span class="sxs-lookup"><span data-stu-id="ddd22-112">This criteria for the **owner** property allows a signed-in user to make updates through other applications they don't own, such as Microsoft Graph Explorer.</span></span> <span data-ttu-id="ddd22-113">使用 Graph 浏览器更新 **schemaExtension** 资源时，请将 **owner** 属性包括在修补程序请求正文中。</span><span class="sxs-lookup"><span data-stu-id="ddd22-113">When using Graph Explorer to update a **schemaExtension** resource, include the **owner** property in the PATCH request body.</span></span> <span data-ttu-id="ddd22-114">有关详细信息，请参阅[Microsoft Graph 已知问题](/graph/known-issues)中的[扩展](/graph/known-issues#extensions)部分。</span><span class="sxs-lookup"><span data-stu-id="ddd22-114">For more information, see the [Extensions](/graph/known-issues#extensions) section in [Known issues with Microsoft Graph](/graph/known-issues).</span></span>

## <a name="permissions"></a><span data-ttu-id="ddd22-115">权限</span><span class="sxs-lookup"><span data-stu-id="ddd22-115">Permissions</span></span>
<span data-ttu-id="ddd22-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddd22-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ddd22-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddd22-118">Permission type</span></span>      | <span data-ttu-id="ddd22-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddd22-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddd22-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddd22-120">Delegated (work or school account)</span></span> | <span data-ttu-id="ddd22-121">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddd22-121">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddd22-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddd22-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddd22-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddd22-123">Not supported.</span></span>    |
|<span data-ttu-id="ddd22-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddd22-124">Application</span></span> | <span data-ttu-id="ddd22-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddd22-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddd22-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddd22-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ddd22-127">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="ddd22-127">Optional request headers</span></span>

| <span data-ttu-id="ddd22-128">名称</span><span class="sxs-lookup"><span data-stu-id="ddd22-128">Name</span></span>      |<span data-ttu-id="ddd22-129">说明</span><span class="sxs-lookup"><span data-stu-id="ddd22-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ddd22-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd22-130">Authorization</span></span>  | <span data-ttu-id="ddd22-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddd22-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ddd22-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ddd22-133">Content-Type</span></span>   | <span data-ttu-id="ddd22-134">application/json</span><span class="sxs-lookup"><span data-stu-id="ddd22-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ddd22-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddd22-135">Request body</span></span>

<span data-ttu-id="ddd22-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ddd22-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ddd22-139">属性</span><span class="sxs-lookup"><span data-stu-id="ddd22-139">Property</span></span>   | <span data-ttu-id="ddd22-140">类型</span><span class="sxs-lookup"><span data-stu-id="ddd22-140">Type</span></span> |<span data-ttu-id="ddd22-141">说明</span><span class="sxs-lookup"><span data-stu-id="ddd22-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ddd22-142">说明</span><span class="sxs-lookup"><span data-stu-id="ddd22-142">description</span></span>|<span data-ttu-id="ddd22-143">String</span><span class="sxs-lookup"><span data-stu-id="ddd22-143">String</span></span>|<span data-ttu-id="ddd22-144">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="ddd22-144">Description for the schema extension.</span></span>|
|<span data-ttu-id="ddd22-145">properties</span><span class="sxs-lookup"><span data-stu-id="ddd22-145">properties</span></span>|<span data-ttu-id="ddd22-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ddd22-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="ddd22-147">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="ddd22-147">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="ddd22-148">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="ddd22-148">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="ddd22-149">status</span><span class="sxs-lookup"><span data-stu-id="ddd22-149">status</span></span>|<span data-ttu-id="ddd22-150">String</span><span class="sxs-lookup"><span data-stu-id="ddd22-150">String</span></span>|<span data-ttu-id="ddd22-151">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="ddd22-151">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="ddd22-152">创建时的初始状态为 **InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="ddd22-152">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="ddd22-153">可能的状态过渡从 **InDevelopment** 到 **可用**，并 **可供\*\*\*\*弃用**。</span><span class="sxs-lookup"><span data-stu-id="ddd22-153">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="ddd22-154">targetTypes</span><span class="sxs-lookup"><span data-stu-id="ddd22-154">targetTypes</span></span>|<span data-ttu-id="ddd22-155">String collection</span><span class="sxs-lookup"><span data-stu-id="ddd22-155">String collection</span></span>|<span data-ttu-id="ddd22-156">架构扩展适用的支持扩展的 Microsoft Graph 类型集。</span><span class="sxs-lookup"><span data-stu-id="ddd22-156">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="ddd22-157">仅允许进行累加性更改。</span><span class="sxs-lookup"><span data-stu-id="ddd22-157">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="ddd22-158">响应</span><span class="sxs-lookup"><span data-stu-id="ddd22-158">Response</span></span>

<span data-ttu-id="ddd22-159">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ddd22-159">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ddd22-160">示例</span><span class="sxs-lookup"><span data-stu-id="ddd22-160">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ddd22-161">请求</span><span class="sxs-lookup"><span data-stu-id="ddd22-161">Request</span></span>

<span data-ttu-id="ddd22-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddd22-162">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ddd22-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd22-163">HTTP</span></span>](#tab/http)
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
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="ddd22-164">C#</span><span class="sxs-lookup"><span data-stu-id="ddd22-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddd22-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddd22-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddd22-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddd22-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddd22-167">Java</span><span class="sxs-lookup"><span data-stu-id="ddd22-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-schemaextension-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ddd22-168">响应</span><span class="sxs-lookup"><span data-stu-id="ddd22-168">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="ddd22-169">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ddd22-169">See also</span></span>

- [<span data-ttu-id="ddd22-170">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="ddd22-170">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ddd22-171">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="ddd22-171">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

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

