---
title: 更新 schemaExtension
description: 更新指定 schemaExtension 的定义中的属性。
ms.openlocfilehash: a09b3a4e2e48eb550acd5e77c60ab7213cc52de8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009838"
---
# <a name="update-schemaextension"></a><span data-ttu-id="b4676-103">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="b4676-103">Update schemaExtension</span></span>

<span data-ttu-id="b4676-104">更新指定 [schemaExtension](../resources/schemaextension.md) 的定义中的属性。</span><span class="sxs-lookup"><span data-stu-id="b4676-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="b4676-p101">此更新适用于该扩展的 **targetTypes** 属性中包含的所有资源。这些资源属于[支持的资源类型](/graph/extensibility-overview#supported-resources)。</span><span class="sxs-lookup"><span data-stu-id="b4676-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="b4676-p102">仅在该扩展处于 **InDevelopment** 或 **Available** 状态时创建架构扩展的应用（所有者应用）可以对扩展进行增量更新。这表示该应用无法删除定义中的自定义属性或目标资源类型。但是此应用可以更改扩展说明。</span><span class="sxs-lookup"><span data-stu-id="b4676-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4676-110">权限</span><span class="sxs-lookup"><span data-stu-id="b4676-110">Permissions</span></span>
<span data-ttu-id="b4676-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4676-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b4676-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4676-113">Permission type</span></span>      | <span data-ttu-id="b4676-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4676-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4676-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4676-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b4676-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4676-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4676-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4676-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4676-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4676-118">Not supported.</span></span>    |
|<span data-ttu-id="b4676-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4676-119">Application</span></span> | <span data-ttu-id="b4676-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4676-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4676-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4676-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="b4676-122">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="b4676-122">Optional request headers</span></span>

| <span data-ttu-id="b4676-123">名称</span><span class="sxs-lookup"><span data-stu-id="b4676-123">Name</span></span>      |<span data-ttu-id="b4676-124">说明</span><span class="sxs-lookup"><span data-stu-id="b4676-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b4676-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4676-125">Authorization</span></span>  | <span data-ttu-id="b4676-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4676-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b4676-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4676-128">Content-Type</span></span>   | <span data-ttu-id="b4676-129">application/json</span><span class="sxs-lookup"><span data-stu-id="b4676-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b4676-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4676-130">Request body</span></span>

<span data-ttu-id="b4676-p105">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b4676-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4676-134">属性</span><span class="sxs-lookup"><span data-stu-id="b4676-134">Property</span></span>   | <span data-ttu-id="b4676-135">类型</span><span class="sxs-lookup"><span data-stu-id="b4676-135">Type</span></span> |<span data-ttu-id="b4676-136">说明</span><span class="sxs-lookup"><span data-stu-id="b4676-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4676-137">说明</span><span class="sxs-lookup"><span data-stu-id="b4676-137">description</span></span>|<span data-ttu-id="b4676-138">String</span><span class="sxs-lookup"><span data-stu-id="b4676-138">String</span></span>|<span data-ttu-id="b4676-139">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="b4676-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="b4676-140">properties</span><span class="sxs-lookup"><span data-stu-id="b4676-140">properties</span></span>|<span data-ttu-id="b4676-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b4676-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="b4676-p106">构成架构扩展定义的属性名称和类型的集合。仅允许增量更改。</span><span class="sxs-lookup"><span data-stu-id="b4676-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="b4676-144">status</span><span class="sxs-lookup"><span data-stu-id="b4676-144">status</span></span>|<span data-ttu-id="b4676-145">String</span><span class="sxs-lookup"><span data-stu-id="b4676-145">String</span></span>|<span data-ttu-id="b4676-146">架构扩展的生命周期状态。</span><span class="sxs-lookup"><span data-stu-id="b4676-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="b4676-147">在创建时的初始状态是**InDevelopment**。</span><span class="sxs-lookup"><span data-stu-id="b4676-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="b4676-148">可能的状态切换为**InDevelopment**到**有空**和到**已否决**的**有空**。</span><span class="sxs-lookup"><span data-stu-id="b4676-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="b4676-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="b4676-149">targetTypes</span></span>|<span data-ttu-id="b4676-150">String collection</span><span class="sxs-lookup"><span data-stu-id="b4676-150">String collection</span></span>|<span data-ttu-id="b4676-p108">架构扩展适用的支持扩展的 Microsoft Graph 类型集。仅允许增量更改。</span><span class="sxs-lookup"><span data-stu-id="b4676-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="b4676-153">响应</span><span class="sxs-lookup"><span data-stu-id="b4676-153">Response</span></span>

<span data-ttu-id="b4676-154">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b4676-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b4676-155">示例</span><span class="sxs-lookup"><span data-stu-id="b4676-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b4676-156">请求</span><span class="sxs-lookup"><span data-stu-id="b4676-156">Request</span></span>

<span data-ttu-id="b4676-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4676-157">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b4676-158">响应</span><span class="sxs-lookup"><span data-stu-id="b4676-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="b4676-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b4676-159">See also</span></span>

- [<span data-ttu-id="b4676-160">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b4676-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b4676-161">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b4676-161">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->