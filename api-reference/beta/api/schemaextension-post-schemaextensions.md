---
title: 创建 schemaExtension
description: 创建一个新的 schemaExtension 定义以扩展支持资源类型。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: a16c8e75d8e07f55a1592374b3d393362ef34252
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053494"
---
# <a name="create-schemaextension"></a><span data-ttu-id="806b4-103">创建 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="806b4-103">Create schemaExtension</span></span>

<span data-ttu-id="806b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="806b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="806b4-105">创建一个新的 [schemaExtension](../resources/schemaextension.md) 定义以扩展[支持资源类型](/graph/extensibility-overview#supported-resources)。</span><span class="sxs-lookup"><span data-stu-id="806b4-105">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="806b4-p101">架构扩展允许将强类型自定义数据添加到资源。创建架构扩展的应用是所有者应用。取决于扩展[状态](/graph/extensibility-overview#schema-extensions-lifecycle)，所有者应用可以且仅所有者应用可以更新或删除扩展。</span><span class="sxs-lookup"><span data-stu-id="806b4-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="806b4-109">请参阅如何[定义描述培训课程的架构扩展](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course)的示例，通过架构扩展定义[使用培训课程数据创建新组](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data)，并[将培训课程数据添加到现有组](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group)。</span><span class="sxs-lookup"><span data-stu-id="806b4-109">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="806b4-110">权限</span><span class="sxs-lookup"><span data-stu-id="806b4-110">Permissions</span></span>
<span data-ttu-id="806b4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="806b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="806b4-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="806b4-113">Permission type</span></span>      | <span data-ttu-id="806b4-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="806b4-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="806b4-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="806b4-115">Delegated (work or school account)</span></span> | <span data-ttu-id="806b4-116">Application.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="806b4-116">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="806b4-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="806b4-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="806b4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="806b4-118">Not supported.</span></span>    |
|<span data-ttu-id="806b4-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="806b4-119">Application</span></span> | <span data-ttu-id="806b4-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="806b4-120">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="806b4-121">此外，对于委派的流程，登录用户必须是调用应用程序的所有者或用于设置 **所有者** 属性的（所带应用程序）`appId`所有者。</span><span class="sxs-lookup"><span data-stu-id="806b4-121">Additionally for the delegated flow, the signed-in user must be the owner of the calling application OR the owner of the (application with the) `appId` used to set the **owner** property.</span></span>

## <a name="http-request"></a><span data-ttu-id="806b4-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="806b4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="806b4-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="806b4-123">Request headers</span></span>
| <span data-ttu-id="806b4-124">名称</span><span class="sxs-lookup"><span data-stu-id="806b4-124">Name</span></span>       | <span data-ttu-id="806b4-125">说明</span><span class="sxs-lookup"><span data-stu-id="806b4-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="806b4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="806b4-126">Authorization</span></span>  | <span data-ttu-id="806b4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="806b4-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="806b4-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="806b4-129">Content-Type</span></span>  | <span data-ttu-id="806b4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="806b4-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="806b4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="806b4-131">Request body</span></span>
<span data-ttu-id="806b4-132">在请求正文中，提供 [schemaExtension](../resources/schemaextension.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="806b4-132">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="806b4-133">下表显示创建架构扩展时可用的属性。</span><span class="sxs-lookup"><span data-stu-id="806b4-133">The following table shows the properties that are available when you create a schema extension.</span></span>

| <span data-ttu-id="806b4-134">参数</span><span class="sxs-lookup"><span data-stu-id="806b4-134">Parameter</span></span> | <span data-ttu-id="806b4-135">类型</span><span class="sxs-lookup"><span data-stu-id="806b4-135">Type</span></span> | <span data-ttu-id="806b4-136">说明</span><span class="sxs-lookup"><span data-stu-id="806b4-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="806b4-137">说明</span><span class="sxs-lookup"><span data-stu-id="806b4-137">description</span></span>|<span data-ttu-id="806b4-138">String</span><span class="sxs-lookup"><span data-stu-id="806b4-138">String</span></span>|<span data-ttu-id="806b4-139">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="806b4-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="806b4-140">id</span><span class="sxs-lookup"><span data-stu-id="806b4-140">id</span></span>|<span data-ttu-id="806b4-141">String</span><span class="sxs-lookup"><span data-stu-id="806b4-141">String</span></span>|<span data-ttu-id="806b4-142">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="806b4-142">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="806b4-143">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="806b4-143">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="806b4-144">连接其中一个已验证域的域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。</span><span class="sxs-lookup"><span data-stu-id="806b4-144">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="806b4-145">示例：`contoso_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="806b4-145">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="806b4-146">注意：仅支持以下顶级域下已经过验证的域：`.com`、`.net`、`.gov`、`.edu` 或 `.org`。</span><span class="sxs-lookup"><span data-stu-id="806b4-146">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="806b4-p105">提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="806b4-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="806b4-149">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="806b4-149">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="806b4-150">owner</span><span class="sxs-lookup"><span data-stu-id="806b4-150">owner</span></span>|<span data-ttu-id="806b4-151">String</span><span class="sxs-lookup"><span data-stu-id="806b4-151">String</span></span>|<span data-ttu-id="806b4-152">（可选）属于架构扩展所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="806b4-152">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="806b4-153">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="806b4-153">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="806b4-154">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="806b4-154">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="806b4-155">因此，如果使用 Graph 浏览器新建一个架构扩展定义，则 **必须** 提供 owner 属性（以此为例）。</span><span class="sxs-lookup"><span data-stu-id="806b4-155">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="806b4-156">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="806b4-156">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="806b4-157">properties</span><span class="sxs-lookup"><span data-stu-id="806b4-157">properties</span></span>|<span data-ttu-id="806b4-158">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="806b4-158">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="806b4-159">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="806b4-159">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="806b4-160">targetTypes</span><span class="sxs-lookup"><span data-stu-id="806b4-160">targetTypes</span></span>|<span data-ttu-id="806b4-161">String collection</span><span class="sxs-lookup"><span data-stu-id="806b4-161">String collection</span></span>|<span data-ttu-id="806b4-162">此架构扩展定义适用的支持架构扩展的 Microsoft Graph 资源类型集。</span><span class="sxs-lookup"><span data-stu-id="806b4-162">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="806b4-163">响应</span><span class="sxs-lookup"><span data-stu-id="806b4-163">Response</span></span>

<span data-ttu-id="806b4-164">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="806b4-164">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="806b4-165">示例</span><span class="sxs-lookup"><span data-stu-id="806b4-165">Example</span></span>

### <a name="example-1-creating-a-schema-extension-using-a-verified-domain"></a><span data-ttu-id="806b4-166">示例 1：使用验证的域创建架构扩展</span><span class="sxs-lookup"><span data-stu-id="806b4-166">Example 1: Creating a schema extension using a verified domain</span></span>

#### <a name="request"></a><span data-ttu-id="806b4-167">请求</span><span class="sxs-lookup"><span data-stu-id="806b4-167">Request</span></span>

<span data-ttu-id="806b4-168">这个示例演示了如何使用已验证的域名 `graphlearn` 和架构名称 `courses` 为架构扩展定义的 **id** 属性形成唯一的字符串。</span><span class="sxs-lookup"><span data-stu-id="806b4-168">This example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition.</span></span> <span data-ttu-id="806b4-169">唯一字符串采用此格式：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span><span class="sxs-lookup"><span data-stu-id="806b4-169">The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="806b4-170">在请求正文中，提供 [schemaExtension](../resources/schemaextension.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="806b4-170">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="806b4-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="806b4-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="806b4-172">C#</span><span class="sxs-lookup"><span data-stu-id="806b4-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="806b4-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="806b4-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="806b4-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="806b4-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="806b4-175">Java</span><span class="sxs-lookup"><span data-stu-id="806b4-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="806b4-176">响应</span><span class="sxs-lookup"><span data-stu-id="806b4-176">Response</span></span>

<span data-ttu-id="806b4-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="806b4-177">Here is an example of the response.</span></span> <span data-ttu-id="806b4-178">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="806b4-178">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

### <a name="example-2-creating-a-schema-extension-using-just-a-name"></a><span data-ttu-id="806b4-179">示例 2：仅使用名称创建架构扩展</span><span class="sxs-lookup"><span data-stu-id="806b4-179">Example 2: Creating a schema extension using just a name</span></span>

#### <a name="request"></a><span data-ttu-id="806b4-180">请求</span><span class="sxs-lookup"><span data-stu-id="806b4-180">Request</span></span>

<span data-ttu-id="806b4-181">这个示例演示了如何在请求的 **id** 属性中，仅指定架构名称、`courses` 以及 [schemaExtension](../resources/schemaextension.md) 对象中剩余属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="806b4-181">This example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span> <span data-ttu-id="806b4-182">Microsoft Graph 将在响应中分配并返回一个唯一的字符串值。</span><span class="sxs-lookup"><span data-stu-id="806b4-182">Microsoft Graph will assign and return a unique string value in the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="806b4-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="806b4-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="806b4-184">C#</span><span class="sxs-lookup"><span data-stu-id="806b4-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="806b4-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="806b4-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="806b4-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="806b4-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="806b4-187">Java</span><span class="sxs-lookup"><span data-stu-id="806b4-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="806b4-188">响应</span><span class="sxs-lookup"><span data-stu-id="806b4-188">Response</span></span>

<span data-ttu-id="806b4-189">该响应在 **id** 属性中包含一个基于请求中提供的架构名称的唯一字符串，以及新创建的架构定义的其余部分。</span><span class="sxs-lookup"><span data-stu-id="806b4-189">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition.</span></span> <span data-ttu-id="806b4-190">响应中的 **id** 值基于架构名称 中的 ext \{ _&#65279;8-random-alphanumeric-chars_&#65279;\} \_ \{ _格式_ \} 。</span><span class="sxs-lookup"><span data-stu-id="806b4-190">The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="806b4-191">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="806b4-191">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

### <a name="example-3-creating-a-schema-extension-setting-the-owner"></a><span data-ttu-id="806b4-192">示例 3：设置所有者来创建架构扩展</span><span class="sxs-lookup"><span data-stu-id="806b4-192">Example 3: Creating a schema extension setting the owner</span></span>

#### <a name="request"></a><span data-ttu-id="806b4-193">请求</span><span class="sxs-lookup"><span data-stu-id="806b4-193">Request</span></span>

<span data-ttu-id="806b4-194">此示例演示如何设置 **所有者** 来创建架构扩展。</span><span class="sxs-lookup"><span data-stu-id="806b4-194">This example shows how to create a schema extension setting the **owner**.</span></span>  <span data-ttu-id="806b4-195">在此方案中，应用程序的用户可能不是应用程序的所有者（例如，当你使用的是 Microsoft Graph 资源管理器）。</span><span class="sxs-lookup"><span data-stu-id="806b4-195">In this scenario, the user of the application might not be the owner of the application (for example if you are using Microsoft Graph Explorer).</span></span>  <span data-ttu-id="806b4-196">在这种情况下，应将 **owner** 属性设置为你拥有的应用程序的 **appId** ，否则你将无权创建架构扩展。</span><span class="sxs-lookup"><span data-stu-id="806b4-196">In this case you should set the **owner** property to the **appId** of an application you own, otherwise you won't be authorized to create a schema extension.</span></span> <span data-ttu-id="806b4-197">在请求中设置 **owner** 属性，以及 [schemaExtension](../resources/schemaextension.md) 对象中其他属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="806b4-197">Set the **owner** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="806b4-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="806b4-198">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_3"
}-->

```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "owner": "50897f70-a455-4adf-87bc-4cf17091d5ac",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="806b4-199">C#</span><span class="sxs-lookup"><span data-stu-id="806b4-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="806b4-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="806b4-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="806b4-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="806b4-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="806b4-202">Java</span><span class="sxs-lookup"><span data-stu-id="806b4-202">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-schemaextension-from-schemaextensions-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="806b4-203">响应</span><span class="sxs-lookup"><span data-stu-id="806b4-203">Response</span></span>

<span data-ttu-id="806b4-204">该响应包括 **owner** 设置为请求中提供的值。</span><span class="sxs-lookup"><span data-stu-id="806b4-204">The response includes the **owner** set to the supplied value in the request.</span></span> <span data-ttu-id="806b4-205">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="806b4-205">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "50897f70-a455-4adf-87bc-4cf17091d5ac",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="806b4-206">另请参阅</span><span class="sxs-lookup"><span data-stu-id="806b4-206">See also</span></span>

- [<span data-ttu-id="806b4-207">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="806b4-207">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="806b4-208">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="806b4-208">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


