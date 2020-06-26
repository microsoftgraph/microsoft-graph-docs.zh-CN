---
title: 创建 schemaExtension
description: 创建一个新的 schemaExtension 定义以扩展支持资源类型。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: extensions
ms.openlocfilehash: e84c7408eb6924205e86059c969201d1c94dcd70
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44896512"
---
# <a name="create-schemaextension"></a><span data-ttu-id="b8252-103">创建 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="b8252-103">Create schemaExtension</span></span>

<span data-ttu-id="b8252-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8252-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8252-105">创建一个新的 [schemaExtension](../resources/schemaextension.md) 定义以扩展[支持资源类型](/graph/extensibility-overview#supported-resources)。</span><span class="sxs-lookup"><span data-stu-id="b8252-105">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="b8252-106">Schema extensions let you add strongly-typed custom data to a resource.</span><span class="sxs-lookup"><span data-stu-id="b8252-106">Schema extensions let you add strongly-typed custom data to a resource.</span></span> <span data-ttu-id="b8252-107">The app that creates a schema extension is the owner app.</span><span class="sxs-lookup"><span data-stu-id="b8252-107">The app that creates a schema extension is the owner app.</span></span> <span data-ttu-id="b8252-108">Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span><span class="sxs-lookup"><span data-stu-id="b8252-108">Depending on the [state](/graph/extensibility-overview#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="b8252-109">请参阅如何[定义描述培训课程的架构扩展](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course)的示例，通过架构扩展定义[使用培训课程数据创建新组](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data)，并[将培训课程数据添加到现有组](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group)。</span><span class="sxs-lookup"><span data-stu-id="b8252-109">See examples of how to [define a schema extension that describes a training course](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8252-110">权限</span><span class="sxs-lookup"><span data-stu-id="b8252-110">Permissions</span></span>
<span data-ttu-id="b8252-111">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b8252-111">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b8252-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8252-112">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b8252-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8252-113">Permission type</span></span>      | <span data-ttu-id="b8252-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8252-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8252-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8252-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b8252-116">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="b8252-116">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8252-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8252-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8252-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8252-118">Not supported.</span></span>    |
|<span data-ttu-id="b8252-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8252-119">Application</span></span> | <span data-ttu-id="b8252-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8252-120">Not supported.</span></span> |

> [!NOTE]
> <span data-ttu-id="b8252-121">此外，对于委派的流程，登录用户必须是调用应用程序的所有者或 `appId` 用于设置**owner**属性的（应用程序的所有者）。</span><span class="sxs-lookup"><span data-stu-id="b8252-121">Additionally for the delegated flow, the signed-in user must be the owner of the calling application OR the owner of the (application with the) `appId` used to set the **owner** property.</span></span>

## <a name="http-request"></a><span data-ttu-id="b8252-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8252-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="b8252-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8252-123">Request headers</span></span>
| <span data-ttu-id="b8252-124">名称</span><span class="sxs-lookup"><span data-stu-id="b8252-124">Name</span></span>       | <span data-ttu-id="b8252-125">说明</span><span class="sxs-lookup"><span data-stu-id="b8252-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b8252-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8252-126">Authorization</span></span>  | <span data-ttu-id="b8252-127">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="b8252-127">Bearer {token}.</span></span> <span data-ttu-id="b8252-128">Required.</span><span class="sxs-lookup"><span data-stu-id="b8252-128">Required.</span></span> |
| <span data-ttu-id="b8252-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8252-129">Content-Type</span></span>  | <span data-ttu-id="b8252-130">application/json</span><span class="sxs-lookup"><span data-stu-id="b8252-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8252-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8252-131">Request body</span></span>
<span data-ttu-id="b8252-132">在请求正文中，提供 [schemaExtension](../resources/schemaextension.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8252-132">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="b8252-133">下表显示创建架构扩展时可用的属性。</span><span class="sxs-lookup"><span data-stu-id="b8252-133">The following table shows the properties that are available when you create a schema extension.</span></span>

| <span data-ttu-id="b8252-134">参数</span><span class="sxs-lookup"><span data-stu-id="b8252-134">Parameter</span></span> | <span data-ttu-id="b8252-135">类型</span><span class="sxs-lookup"><span data-stu-id="b8252-135">Type</span></span> | <span data-ttu-id="b8252-136">说明</span><span class="sxs-lookup"><span data-stu-id="b8252-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8252-137">说明</span><span class="sxs-lookup"><span data-stu-id="b8252-137">description</span></span>|<span data-ttu-id="b8252-138">String</span><span class="sxs-lookup"><span data-stu-id="b8252-138">String</span></span>|<span data-ttu-id="b8252-139">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="b8252-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="b8252-140">id</span><span class="sxs-lookup"><span data-stu-id="b8252-140">id</span></span>|<span data-ttu-id="b8252-141">字符串</span><span class="sxs-lookup"><span data-stu-id="b8252-141">String</span></span>|<span data-ttu-id="b8252-142">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b8252-142">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="b8252-143">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="b8252-143">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="b8252-144">连接其中一个已验证域的域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。</span><span class="sxs-lookup"><span data-stu-id="b8252-144">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span> <span data-ttu-id="b8252-145">示例：`contoso_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="b8252-145">As an example, `contoso_mySchema`.</span></span> <span data-ttu-id="b8252-146">注意：仅支持以下顶级域下已经过验证的域：`.com`、`.net`、`.gov`、`.edu` 或 `.org`。</span><span class="sxs-lookup"><span data-stu-id="b8252-146">NOTE: Only verified domains under the following top-level domains are supported: `.com`,`.net`, `.gov`, `.edu` or `.org`.</span></span> </li><li><span data-ttu-id="b8252-147">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span><span class="sxs-lookup"><span data-stu-id="b8252-147">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="b8252-148">An example would be `extkvbmkofy_mySchema`.</span><span class="sxs-lookup"><span data-stu-id="b8252-148">An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="b8252-149">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="b8252-149">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="b8252-150">owner</span><span class="sxs-lookup"><span data-stu-id="b8252-150">owner</span></span>|<span data-ttu-id="b8252-151">String</span><span class="sxs-lookup"><span data-stu-id="b8252-151">String</span></span>|<span data-ttu-id="b8252-152">（可选）属于架构扩展所有者的应用程序的 `appId`。</span><span class="sxs-lookup"><span data-stu-id="b8252-152">(Optional) The `appId` of the application that is the owner of the schema extension.</span></span> <span data-ttu-id="b8252-153">可在创建时提供此属性以设置所有者。</span><span class="sxs-lookup"><span data-stu-id="b8252-153">This property can be supplied on creation, to set the owner.</span></span>  <span data-ttu-id="b8252-154">如果未提供，则会将调用应用程序的 `appId` 设置为所有者。</span><span class="sxs-lookup"><span data-stu-id="b8252-154">If not supplied, then the calling application's `appId` will be set as the owner.</span></span> <span data-ttu-id="b8252-155">因此，如果使用 Graph 浏览器新建一个架构扩展定义，则**必须**提供 owner 属性（以此为例）。</span><span class="sxs-lookup"><span data-stu-id="b8252-155">So, for example, if creating a new schema extension definition using Graph Explorer, you **must** supply the owner property.</span></span> <span data-ttu-id="b8252-156">设置后，此属性为只读，且无法更改。</span><span class="sxs-lookup"><span data-stu-id="b8252-156">Once set, this property is read-only and cannot be changed.</span></span>|
|<span data-ttu-id="b8252-157">properties</span><span class="sxs-lookup"><span data-stu-id="b8252-157">properties</span></span>|<span data-ttu-id="b8252-158">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b8252-158">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="b8252-159">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="b8252-159">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="b8252-160">targetTypes</span><span class="sxs-lookup"><span data-stu-id="b8252-160">targetTypes</span></span>|<span data-ttu-id="b8252-161">String collection</span><span class="sxs-lookup"><span data-stu-id="b8252-161">String collection</span></span>|<span data-ttu-id="b8252-162">此架构扩展定义适用的支持架构扩展的 Microsoft Graph 资源类型集。</span><span class="sxs-lookup"><span data-stu-id="b8252-162">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="b8252-163">响应</span><span class="sxs-lookup"><span data-stu-id="b8252-163">Response</span></span>

<span data-ttu-id="b8252-164">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8252-164">If successful, this method returns `201 Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8252-165">示例</span><span class="sxs-lookup"><span data-stu-id="b8252-165">Example</span></span>

### <a name="example-1-creating-a-schema-extension-using-a-verified-domain"></a><span data-ttu-id="b8252-166">示例1：使用已验证的域创建架构扩展</span><span class="sxs-lookup"><span data-stu-id="b8252-166">Example 1: Creating a schema extension using a verified domain</span></span>

#### <a name="request"></a><span data-ttu-id="b8252-167">请求</span><span class="sxs-lookup"><span data-stu-id="b8252-167">Request</span></span>

<span data-ttu-id="b8252-168">本示例演示如何使用经验证的域名、以及 `graphlearn` 架构名称， `courses` 以构成架构扩展定义的**id**属性的唯一字符串。</span><span class="sxs-lookup"><span data-stu-id="b8252-168">This example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition.</span></span> <span data-ttu-id="b8252-169">唯一字符串基于此格式， \{ _&#65279;domainName_ \} \_ \{ _&#65279;schemaName_ \} 。</span><span class="sxs-lookup"><span data-stu-id="b8252-169">The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="b8252-170">在请求正文中，提供 [schemaExtension](../resources/schemaextension.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8252-170">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8252-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8252-171">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b8252-172">C#</span><span class="sxs-lookup"><span data-stu-id="b8252-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8252-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8252-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8252-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8252-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8252-175">响应</span><span class="sxs-lookup"><span data-stu-id="b8252-175">Response</span></span>

<span data-ttu-id="b8252-176">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b8252-176">Here is an example of the response.</span></span> <span data-ttu-id="b8252-177">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b8252-177">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b8252-178">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b8252-178">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-creating-a-schema-extension-using-just-a-name"></a><span data-ttu-id="b8252-179">示例2：仅使用名称创建架构扩展</span><span class="sxs-lookup"><span data-stu-id="b8252-179">Example 2: Creating a schema extension using just a name</span></span>

#### <a name="request"></a><span data-ttu-id="b8252-180">请求</span><span class="sxs-lookup"><span data-stu-id="b8252-180">Request</span></span>

<span data-ttu-id="b8252-181">此示例展示了如何 `courses` 在请求的**id**属性中指定架构名称，以及[schemaExtension](../resources/schemaextension.md)对象中其余属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8252-181">This example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span> <span data-ttu-id="b8252-182">Microsoft Graph 将在响应中分配并返回一个唯一的字符串值。</span><span class="sxs-lookup"><span data-stu-id="b8252-182">Microsoft Graph will assign and return a unique string value in the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="b8252-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8252-183">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b8252-184">C#</span><span class="sxs-lookup"><span data-stu-id="b8252-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8252-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8252-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8252-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8252-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8252-187">响应</span><span class="sxs-lookup"><span data-stu-id="b8252-187">Response</span></span>

<span data-ttu-id="b8252-188">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition.</span><span class="sxs-lookup"><span data-stu-id="b8252-188">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition.</span></span> <span data-ttu-id="b8252-189">The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span><span class="sxs-lookup"><span data-stu-id="b8252-189">The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}.</span></span> <span data-ttu-id="b8252-190">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b8252-190">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b8252-191">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b8252-191">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-3-creating-a-schema-extension-setting-the-owner"></a><span data-ttu-id="b8252-192">示例3：创建架构扩展设置所有者</span><span class="sxs-lookup"><span data-stu-id="b8252-192">Example 3: Creating a schema extension setting the owner</span></span>

#### <a name="request"></a><span data-ttu-id="b8252-193">请求</span><span class="sxs-lookup"><span data-stu-id="b8252-193">Request</span></span>

<span data-ttu-id="b8252-194">本示例演示如何创建**所有者**的架构扩展设置。</span><span class="sxs-lookup"><span data-stu-id="b8252-194">This example shows how to create a schema extension setting the **owner**.</span></span>  <span data-ttu-id="b8252-195">在这种情况下，应用程序的用户可能不是应用程序的所有者（例如，如果使用的是 Microsoft Graph 资源管理器）。</span><span class="sxs-lookup"><span data-stu-id="b8252-195">In this scenario, the user of the application might not be the owner of the application (for example if you are using Microsoft Graph Explorer).</span></span>  <span data-ttu-id="b8252-196">在这种情况下，应将**owner**属性设置为您拥有的应用程序的**appId** ，否则您将不会被授权创建架构扩展。</span><span class="sxs-lookup"><span data-stu-id="b8252-196">In this case you should set the **owner** property to the **appId** of an application you own, otherwise you won't be authorized to create a schema extension.</span></span> <span data-ttu-id="b8252-197">在请求中设置**owner**属性，以及[schemaExtension](../resources/schemaextension.md)对象中的其余属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8252-197">Set the **owner** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="b8252-198">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8252-198">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b8252-199">C#</span><span class="sxs-lookup"><span data-stu-id="b8252-199">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-schemaextension-from-schemaextensions-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8252-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8252-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-schemaextension-from-schemaextensions-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8252-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8252-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-schemaextension-from-schemaextensions-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b8252-202">响应</span><span class="sxs-lookup"><span data-stu-id="b8252-202">Response</span></span>

<span data-ttu-id="b8252-203">响应包括**所有者**设置为请求中提供的值。</span><span class="sxs-lookup"><span data-stu-id="b8252-203">The response includes the **owner** set to the supplied value in the request.</span></span> <span data-ttu-id="b8252-204">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b8252-204">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b8252-205">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b8252-205">All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="b8252-206">另请参阅</span><span class="sxs-lookup"><span data-stu-id="b8252-206">See also</span></span>

- [<span data-ttu-id="b8252-207">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b8252-207">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="b8252-208">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="b8252-208">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


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
