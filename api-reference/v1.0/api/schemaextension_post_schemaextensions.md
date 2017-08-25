# <a name="create-schemaextension"></a><span data-ttu-id="28391-101">创建 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="28391-101">Create schemaExtension</span></span>

<span data-ttu-id="28391-102">创建一个新的 [schemaExtension](../resources/schemaextension.md) 定义以扩展[支持资源类型](../../../concepts/extensibility_overview.md#supported-resources)。</span><span class="sxs-lookup"><span data-stu-id="28391-102">Create a new [schemaExtension](../resources/schemaextension.md) definition to extend a [supporting resource type](../../../concepts/extensibility_overview.md#supported-resources).</span></span>

<span data-ttu-id="28391-p101">架构扩展允许将强类型自定义数据添加到资源。创建架构扩展的应用是所有者应用。取决于扩展[状态](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle)，所有者应用可以且仅所有者应用可以更新或删除扩展。</span><span class="sxs-lookup"><span data-stu-id="28391-p101">Schema extensions let you add strongly-typed custom data to a resource. The app that creates a schema extension is the owner app. Depending on the [state](../../../concepts/extensibility_overview.md#schema-extensions-lifecycle) of the extension, the owner app, and only the owner app, may update or delete the extension.</span></span> 

<span data-ttu-id="28391-106">请参阅如何[定义描述培训课程的架构扩展](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course)的示例，通过架构扩展定义[使用培训课程数据创建新组](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data)，并[将培训课程数据添加到现有组](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group)。</span><span class="sxs-lookup"><span data-stu-id="28391-106">See examples of how to [define a schema extension that describes a training course](../../../concepts/extensibility_schema_groups.md#2-register-a-schema-extension-definition-that-describes-a-training-course), use the schema extension definition to [create a new group with training course data](../../../concepts/extensibility_schema_groups.md#3-create-a-new-group-with-extended-data), and [add training course data to an existing group](../../../concepts/extensibility_schema_groups.md#4-add-update-or-remove-custom-data-in-an-existing-group).</span></span>

## <a name="permissions"></a><span data-ttu-id="28391-107">权限</span><span class="sxs-lookup"><span data-stu-id="28391-107">Permissions</span></span>
<span data-ttu-id="28391-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="28391-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="28391-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="28391-110">Permission type</span></span>      | <span data-ttu-id="28391-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28391-111">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="28391-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28391-112">Delegated (work or school account)</span></span> | <span data-ttu-id="28391-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28391-113">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="28391-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28391-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28391-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28391-115">Not supported.</span></span>    | 
|<span data-ttu-id="28391-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="28391-116">Application</span></span> | <span data-ttu-id="28391-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="28391-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="28391-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28391-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /schemaExtensions
```

## <a name="request-headers"></a><span data-ttu-id="28391-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="28391-119">Request headers</span></span>
| <span data-ttu-id="28391-120">名称</span><span class="sxs-lookup"><span data-stu-id="28391-120">Name</span></span>       | <span data-ttu-id="28391-121">说明</span><span class="sxs-lookup"><span data-stu-id="28391-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28391-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28391-122">Authorization</span></span>  | <span data-ttu-id="28391-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="28391-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="28391-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="28391-125">Content-Type</span></span>  | <span data-ttu-id="28391-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28391-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="28391-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="28391-127">Request body</span></span>
<span data-ttu-id="28391-128">在请求正文中，提供 [schemaExtension](../resources/schemaextension.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28391-128">In the request body, supply a JSON representation of [schemaExtension](../resources/schemaextension.md) object.</span></span>

<span data-ttu-id="28391-129">下表显示创建架构扩展时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="28391-129">The following table shows the properties that are required when you create a schema extension.</span></span>

| <span data-ttu-id="28391-130">参数</span><span class="sxs-lookup"><span data-stu-id="28391-130">Parameter</span></span> | <span data-ttu-id="28391-131">类型</span><span class="sxs-lookup"><span data-stu-id="28391-131">Type</span></span> | <span data-ttu-id="28391-132">说明</span><span class="sxs-lookup"><span data-stu-id="28391-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28391-133">说明</span><span class="sxs-lookup"><span data-stu-id="28391-133">description</span></span>|<span data-ttu-id="28391-134">String</span><span class="sxs-lookup"><span data-stu-id="28391-134">String</span></span>|<span data-ttu-id="28391-135">架构扩展的说明。</span><span class="sxs-lookup"><span data-stu-id="28391-135">Description for the schema extension.</span></span>|
|<span data-ttu-id="28391-136">id</span><span class="sxs-lookup"><span data-stu-id="28391-136">id</span></span>|<span data-ttu-id="28391-137">String</span><span class="sxs-lookup"><span data-stu-id="28391-137">String</span></span>|<span data-ttu-id="28391-138">架构扩展定义的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="28391-138">The unique identifier for the schema extension definition.</span></span> <br><span data-ttu-id="28391-139">你可以使用下面两种方法之一分配值：</span><span class="sxs-lookup"><span data-stu-id="28391-139">You can assign a value in one of two ways:</span></span> <ul><li><span data-ttu-id="28391-p104">连接已验证域名与架构扩展名称，形成此格式的唯一字符串：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。例如 `contoso_mySchema`。 </span><span class="sxs-lookup"><span data-stu-id="28391-p104">Concatenate the name of one of your verified domains with a name for the schema extension to form a unique string in this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. As an example, `contoso_mySchema`. </span></span></li><li><span data-ttu-id="28391-p105">提供一个架构名称，并让 Microsoft Graph 使用此格式的架构名称完成 **id** 分配：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。例如 `extkvbmkofy_mySchema`。</span><span class="sxs-lookup"><span data-stu-id="28391-p105">Provide a schema name, and let Microsoft Graph use that schema name to complete the **id** assignment in this format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. An example would be `extkvbmkofy_mySchema`.</span></span></li></ul><span data-ttu-id="28391-144">此属性一旦创建，便无法更改。</span><span class="sxs-lookup"><span data-stu-id="28391-144">This property cannot be changed after creation.</span></span> |
|<span data-ttu-id="28391-145">属性</span><span class="sxs-lookup"><span data-stu-id="28391-145">properties</span></span>|<span data-ttu-id="28391-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28391-146">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="28391-147">构成架构扩展定义的属性名称和类型的集合。</span><span class="sxs-lookup"><span data-stu-id="28391-147">The collection of property names and types that make up the schema extension definition.</span></span>|
|<span data-ttu-id="28391-148">targetTypes</span><span class="sxs-lookup"><span data-stu-id="28391-148">targetTypes</span></span>|<span data-ttu-id="28391-149">String collection</span><span class="sxs-lookup"><span data-stu-id="28391-149">String collection</span></span>|<span data-ttu-id="28391-150">此架构扩展定义适用的支持架构扩展的 Microsoft Graph 资源类型集。</span><span class="sxs-lookup"><span data-stu-id="28391-150">Set of Microsoft Graph resource types (that support schema extensions) that this schema extension definition can be applied to.</span></span>|

## <a name="response"></a><span data-ttu-id="28391-151">响应</span><span class="sxs-lookup"><span data-stu-id="28391-151">Response</span></span>

<span data-ttu-id="28391-152">如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [schemaExtension](../resources/schemaextension.md)对象。</span><span class="sxs-lookup"><span data-stu-id="28391-152">If successful, this method returns `201, Created` response code and [schemaExtension](../resources/schemaextension.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28391-153">示例</span><span class="sxs-lookup"><span data-stu-id="28391-153">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="28391-154">请求 1</span><span class="sxs-lookup"><span data-stu-id="28391-154">Request 1</span></span>

<span data-ttu-id="28391-p106">第一个示例演示了如何使用已验证的域名 `graphlearn` 和架构名称 `courses` 为架构扩展定义的 **id** 属性形成唯一的字符串。唯一字符串采用此格式：\{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}。</span><span class="sxs-lookup"><span data-stu-id="28391-p106">The first example shows using a verified domain name, `graphlearn`, and a schema name, `courses`, to form a unique string for the **id** property of the schema extension definition. The unique string is based on this format, \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.</span></span>

<span data-ttu-id="28391-157">在请求正文中，提供 [schemaExtension](../resources/schemaextension.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28391-157">In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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

##### <a name="response-1"></a><span data-ttu-id="28391-158">响应 1</span><span class="sxs-lookup"><span data-stu-id="28391-158">Response 1</span></span>

<span data-ttu-id="28391-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28391-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="28391-162">请求 2</span><span class="sxs-lookup"><span data-stu-id="28391-162">Request 2</span></span>

<span data-ttu-id="28391-p108">第二个示例演示了如何在请求的 **id** 属性中，仅指定架构名称、`courses` 以及 [schemaExtension](../resources/schemaextension.md) 对象中剩余属性的 JSON 表示形式。Microsoft Graph 将在响应中分配并返回一个唯一的字符串值。</span><span class="sxs-lookup"><span data-stu-id="28391-p108">The second example shows specifying just a schema name, `courses`, in the **id** property in the request, together with the JSON representation of the rest of the properties in the [schemaExtension](../resources/schemaextension.md) object. Microsoft Graph will assign and return a unique string value in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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

##### <a name="response-2"></a><span data-ttu-id="28391-165">响应 2</span><span class="sxs-lookup"><span data-stu-id="28391-165">Response 2</span></span>

<span data-ttu-id="28391-p109">该响应包括一个基于请求中提供的架构名称的 **id** 属性中唯一的字符串，以及新创建的架构定义的其余部分。响应中的 **id** 中的值采用此格式：ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="28391-p109">The response includes a unique string in the **id** property that is based on the schema name provided in the request, together with the rest of the newly created schema definition. The value in **id** in the response is based on the format, ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


## <a name="see-also"></a><span data-ttu-id="28391-170">另请参阅</span><span class="sxs-lookup"><span data-stu-id="28391-170">See also</span></span>

- [<span data-ttu-id="28391-171">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="28391-171">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="28391-172">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="28391-172">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->