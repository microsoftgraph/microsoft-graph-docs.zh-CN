# <a name="add-custom-data-to-groups-using-schema-extensions"></a><span data-ttu-id="7dc98-101">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7dc98-101">Add custom data to groups using schema extensions</span></span> 

<span data-ttu-id="7dc98-102">我们将引导你完成一个示例，演示如何使用*架构扩展*。</span><span class="sxs-lookup"><span data-stu-id="7dc98-102">We're going to walk you through an example to demonstrate how to use *schema extensions*.</span></span> 

<span data-ttu-id="7dc98-p101">假设你是一个名为“Graph Learn”的学习管理软件公司的开发人员，工作是为企业构建培训课程和材料。Office 365 组具有丰富的协作体验，是为在线课程和教师引导式课程的参与者提供交付课程内容和记录练习的绝佳方式。你可能希望将那些 Office 365 组用于使培训课程可轻松地被识别为培训课程，从而使其他开发人员可以发现你的组，并在你的学习课程的基础上构建丰富的体验。</span><span class="sxs-lookup"><span data-stu-id="7dc98-p101">Imagine you're a developer in a Learning Management Software company called “Graph Learn” that builds training courses and materials for businesses.  Office 365 groups, with their rich collaborative experiences, is a fantastic way to deliver course content and record exercises among participants for both online courses and instructor-led courses.  You may want to make those Office 365 groups used for training courses easily identifiable as training courses, which will allow other developers to discover your groups and build rich experiences on top of your learning courses.</span></span>

<span data-ttu-id="7dc98-106">针对这种应用场景，我们将介绍如何操作：</span><span class="sxs-lookup"><span data-stu-id="7dc98-106">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="7dc98-107">查看可以使用的可用架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="7dc98-107">View available schema extension definitions that you could use.</span></span>
2. <span data-ttu-id="7dc98-108">注册以培训课程组为目标的架构扩展定义。</span><span class="sxs-lookup"><span data-stu-id="7dc98-108">Register a schema extension definition that targets groups for training courses.</span></span>
3. <span data-ttu-id="7dc98-109">根据你刚刚注册的架构扩展定义，创建具有扩展数据的新组。</span><span class="sxs-lookup"><span data-stu-id="7dc98-109">Create a new group with extended data based on the schema extension definition that you just registered.</span></span>
4. <span data-ttu-id="7dc98-110">根据架构扩展定义向现有组添加、更新或删除自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7dc98-110">Add, update, or remove custom data in an existing group based on a schema extension definition.</span></span>
5. <span data-ttu-id="7dc98-111">读回组和扩展数据。</span><span class="sxs-lookup"><span data-stu-id="7dc98-111">Read back a group and the extension data.</span></span>

><span data-ttu-id="7dc98-p102">**注意：**本主题介绍如何在**组**资源上创建和读取架构扩展值（步骤 3-5）。**管理单元**、**设备**、**事件**、**邮件**、**组织**、**帖子**和**用户**资源类型也支持相同方法。因此，可以对任意资源执行与以下示例请求相似的操作。请注意，**administrativeUnit** 仅适用于 beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="7dc98-p102">**Note:** This topic shows you how to create and read schema extension values on a **group** resource (steps 3-5).  The same methods are supported for the **administrativeUnit**, **device**, **event**, **message**, **organization**, **post**, and **user** resource types as well.  So you can carry out similar operations as the example requests below on any of those resources. Note that **administrativeUnit** is available only in the beta endpoint.</span></span>

## <a name="1-view-available-schema-extensions"></a><span data-ttu-id="7dc98-116">1.查看可用的架构扩展</span><span class="sxs-lookup"><span data-stu-id="7dc98-116">1. View available schema extensions</span></span>
<span data-ttu-id="7dc98-p103">首先，作为开发人员，可能希望找到应用可以重复使用的任何其他架构扩展定义。这可以通过查询 **schemaExtension** 资源来完成。</span><span class="sxs-lookup"><span data-stu-id="7dc98-p103">First, as a developer, you might want to find any other schema extension definitions that our app could reuse.  This can be done by querying the **schemaExtension** resource.</span></span>  
<span data-ttu-id="7dc98-119">在下面的示例中，将按 **id** 查询特定的架构扩展。</span><span class="sxs-lookup"><span data-stu-id="7dc98-119">In the example below, you're going to query for a specific schema extension by **id**.</span></span>

<span data-ttu-id="7dc98-p104">请注意响应中返回的扩展将**可用**作为**状态**值，即表示具有 **targetTypes** 属性中的资源访问权限的所有应用都可使用此扩展并通过增量更改更新此扩展。通常，无论**状态**如何，此操作都将返回满足指定筛选器的所有架构扩展，因此在使用扩展前请务必先检查其状态。</span><span class="sxs-lookup"><span data-stu-id="7dc98-p104">Notice that the extension returned in the response has **Available** as the **status** value, which indicates that any app which has permission to the resources in the **targetTypes** property can use and update the extension with additive changes. In general, this operation returns any schema extensions that satisfy the specified filter regardless of **status**, so do check the extension status before using it.</span></span>


##### <a name="request"></a><span data-ttu-id="7dc98-122">请求</span><span class="sxs-lookup"><span data-stu-id="7dc98-122">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="7dc98-123">响应</span><span class="sxs-lookup"><span data-stu-id="7dc98-123">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420
{
    "value": [
        {
            "id":"graphlearn_test",
            "description": "Yet another test schema",
            "targetTypes": [
                "User", "Group"
            ],
            "status": "Available",
            "owner": "24d3b144-21ae-4080-943f-7067b395b913",
            "properties": [
                {
                    "name": "testName",
                    "type": "String"
                }
            ]
        }
    ]
}
```
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a><span data-ttu-id="7dc98-124">2.注册可描述培训课程的架构扩展定义</span><span class="sxs-lookup"><span data-stu-id="7dc98-124">2. Register a schema extension definition that describes a training course</span></span>
<span data-ttu-id="7dc98-125">如果找不到*符合*你的需求的架构扩展，则可以在**组**资源上为培训课程创建并注册新的扩展定义。</span><span class="sxs-lookup"><span data-stu-id="7dc98-125">If you can't find a schema extension that *is* appropriate for your needs, you can create and register a new extension definition for training courses on the **group** resource.</span></span>  

<span data-ttu-id="7dc98-p105">在创建架构扩展定义时，应为 **id** 属性提供一个字符串。可以通过两种方式来执行此操作。以下示例演示首选方法，它使用一个经租户验证的虚域名 (`graphlearn.com`)。将验证的域名 (`graphlearn`) 与架构扩展的名称 (`courses`) 相连接，并使用结果字符串 `graphlearn_courses` 分配 **id**。</span><span class="sxs-lookup"><span data-stu-id="7dc98-p105">When creating a schema extension definition, you should provide a string for the **id** property. There are two ways to do this. The following example shows the preferred way, which uses a vanity domain name (`graphlearn.com`) that has been verified with your tenant. Concatenate the verified domain name (`graphlearn`) with a name for the schema extension (`courses`), and assign **id** with the resultant string, `graphlearn_courses`.</span></span>  

<span data-ttu-id="7dc98-p106">然后，还要指定说明（以启用可发现性）、目标类型（定义该扩展适用于哪些资源）以及构成架构的自定义属性。在本示例中，指定 `courseId`、`courseName` 和 `courseType` 自定义属性及其类型。</span><span class="sxs-lookup"><span data-stu-id="7dc98-p106">Then, specify a description (to enable discoverability), target types (defining which resources this extension applies to), and the custom properties that make up the schema.  In this example, specify the `courseId`, `courseName` and `courseType` custom properties and their types.</span></span>

<span data-ttu-id="7dc98-132">请参阅[分配请求中 **id** 的其他方法示例](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md#request-2)，仅需要提供架构名称。</span><span class="sxs-lookup"><span data-stu-id="7dc98-132">See an [example of the other way to assign **id** in the request](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md#request-2), that requires you to provide only a schema name.</span></span>

<span data-ttu-id="7dc98-p107">请注意，初次创建架构扩展时，其状态是 **InDevelopment**。在开发扩展期间，可以将其保持在此状态，在此期间仅创建该扩展的应用可以使用增量更改更新它或将其删除。准备共享此扩展以供其他应用使用时，请将**状态**设置为**可用**</span><span class="sxs-lookup"><span data-stu-id="7dc98-p107">Notice that when you initially create a schema extension, its status is **InDevelopment**. While you're developing the extension, you can keep it in this status, during which only your app that created it can update it with additive changes or delete it. When you are ready to share the extension for use by other apps, set **status** to **Available**.</span></span>

##### <a name="request"></a><span data-ttu-id="7dc98-136">请求</span><span class="sxs-lookup"><span data-stu-id="7dc98-136">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="7dc98-137">响应</span><span class="sxs-lookup"><span data-stu-id="7dc98-137">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
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

## <a name="3-create-a-new-group-with-extended-data"></a><span data-ttu-id="7dc98-138">3.创建具有扩展数据的新组</span><span class="sxs-lookup"><span data-stu-id="7dc98-138">3. Create a new group with extended data</span></span> 
<span data-ttu-id="7dc98-p108">使用我们刚刚注册的 `graphlearn_courses` 架构扩展定义创建一个_新_组并使用额外数据进行扩展。这是**组**资源的标准 ```POST```，其他 `graphlearn_courses` 复杂类型扩展在请求正文中定义。响应将不会返回任何数据扩展的镜像。我们需要使用 ```GET``` 操作按名称显式 ```$select``` 扩展。</span><span class="sxs-lookup"><span data-stu-id="7dc98-p108">Create a _new_ group and extend it with extra data using the `graphlearn_courses` schema extension definition that we just registered.  This is a standard ```POST``` to the **group** resource, with the additional `graphlearn_courses` complex type extension defined in the request body.  The response will not mirror back any data extensions. We need to explicitly ```$select``` the extension by name using a ```GET``` operation.</span></span>

##### <a name="request"></a><span data-ttu-id="7dc98-143">请求</span><span class="sxs-lookup"><span data-stu-id="7dc98-143">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "groupTypes": ["Unified"],
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "graphlearn_courses": {
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```
##### <a name="response"></a><span data-ttu-id="7dc98-144">响应</span><span class="sxs-lookup"><span data-stu-id="7dc98-144">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "dfc8016f-db97-4c47-a582-49cb8f849355",
    "createdDateTime": "2017-02-09T00:17:05Z",
    "description": "New Managers training course for March 2017",
    "displayName": "New Managers March 2017",
    "groupTypes": [
        "Unified"
    ],
    "mail": "newMan201703@graphlearn.com",
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a><span data-ttu-id="7dc98-145">4.在现有组中添加、更新或删除自定义数据</span><span class="sxs-lookup"><span data-stu-id="7dc98-145">4. Add, update, or remove custom data in an existing group</span></span>
<span data-ttu-id="7dc98-146">可以使用在 ```PATCH``` 请求的正文中定义的其他 `graphlearn_courses` 复杂类型扩展来扩展自定义数据并将其添加到_现有_组实例。</span><span class="sxs-lookup"><span data-stu-id="7dc98-146">You can extend and add custom data to an _existing_ group instance with the additional `graphlearn_courses` complex type extension defined in the body of a ```PATCH``` request.</span></span>  

##### <a name="request"></a><span data-ttu-id="7dc98-147">请求</span><span class="sxs-lookup"><span data-stu-id="7dc98-147">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
Content-length: 230
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```
##### <a name="response"></a><span data-ttu-id="7dc98-148">响应</span><span class="sxs-lookup"><span data-stu-id="7dc98-148">Response</span></span>
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="7dc98-149">如果要更新扩展数据的值，请将整个扩展复杂类型置于 ```PATCH``` 请求正文中（类似于向现有资源添加自定义数据）。</span><span class="sxs-lookup"><span data-stu-id="7dc98-149">If you want to update the values of the extension data, put the entire extension complex type in the body of a ```PATCH``` request (similar to adding custom data to an existing resource).</span></span>

<span data-ttu-id="7dc98-150">还可以将相应的扩展属性设置为 null，从而删除添加到资源实例中的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7dc98-150">You can also remove custom data added to a resource instance by setting the corresponding extension property to null.</span></span> 

<span data-ttu-id="7dc98-151">若要将架构扩展从资源实例中删除，请将该实例中的扩展复杂类型设置为 null。</span><span class="sxs-lookup"><span data-stu-id="7dc98-151">To remove a schema extension from a resource instance, set the extension complex type in that instance to null.</span></span>


## <a name="5-get-a-group-and-its-extension-data"></a><span data-ttu-id="7dc98-152">5.获取组及其扩展数据</span><span class="sxs-lookup"><span data-stu-id="7dc98-152">5. Get a group and its extension data</span></span>
<span data-ttu-id="7dc98-153">查找组的简便方法有：使用 `$filter` 匹配特定的扩展属性值，比如扩展名或 ID。</span><span class="sxs-lookup"><span data-stu-id="7dc98-153">A handy way to look for a group (or groups) is to use `$filter` to match for specific extension property values, such as an extension name or ID.</span></span> 

<span data-ttu-id="7dc98-154">然后，使用 `$select` 按名称包含扩展（在此情况下按 `graphlearn_courses`）获取组中的自定义数据。</span><span class="sxs-lookup"><span data-stu-id="7dc98-154">Then, to get the custom data in a group, use `$select` to include the extension by name (in this case by `graphlearn_courses`).</span></span>

<span data-ttu-id="7dc98-p109">下面的示例查找了具有 `graphlearn_courses` 扩展且 `courseId` 属性值与 `123` 相匹配的组，获取了组属性 **displayName**、 **id** 和 **description**，以及 `graphlearn_courses` 扩展中的自定义数据。（在实际查询中，请确保根据需要应用 URL 编码。）</span><span class="sxs-lookup"><span data-stu-id="7dc98-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

#### <a name="request"></a><span data-ttu-id="7dc98-157">请求</span><span class="sxs-lookup"><span data-stu-id="7dc98-157">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <a name="response"></a><span data-ttu-id="7dc98-158">响应</span><span class="sxs-lookup"><span data-stu-id="7dc98-158">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="7dc98-159">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7dc98-159">See also</span></span>

- [<span data-ttu-id="7dc98-160">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="7dc98-160">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="7dc98-161">使用开放扩展向用户添加自定义数据（预览）</span><span class="sxs-lookup"><span data-stu-id="7dc98-161">Add custom data to users using open extensions (preview)</span></span>](extensibility_open_users.md)
- [<span data-ttu-id="7dc98-162">Office 365 域</span><span class="sxs-lookup"><span data-stu-id="7dc98-162">Office 365 domains</span></span>](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)
- [<span data-ttu-id="7dc98-163">添加并验证新 Office 365 的域</span><span class="sxs-lookup"><span data-stu-id="7dc98-163">Adding and Verifying a Domain for the NEW Office 365</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="7dc98-164">schemaExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="7dc98-164">schemaExtension resource type</span></span>](../api-reference/v1.0/resources/schemaextension.md)
- [<span data-ttu-id="7dc98-165">列出 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="7dc98-165">List schemaExtensions</span></span>](../api-reference/v1.0/api/schemaextension_list.md)
- [<span data-ttu-id="7dc98-166">创建 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="7dc98-166">Create schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [<span data-ttu-id="7dc98-167">获取 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="7dc98-167">Get schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_get.md)
- [<span data-ttu-id="7dc98-168">更新 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="7dc98-168">Update schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_update.md)
- [<span data-ttu-id="7dc98-169">删除 schemaExtension</span><span class="sxs-lookup"><span data-stu-id="7dc98-169">Delete schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_delete.md)
