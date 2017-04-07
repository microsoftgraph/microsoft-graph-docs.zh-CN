# <a name="add-custom-data-to-groups-using-schema-extensions-preview"></a>使用架构扩展向组添加自定义数据（预览）

我们将引导你完成一个示例，演示如何使用*架构扩展*。 

假设你是一个名为“Graph Learn”的学习管理软件公司的开发人员，工作是为企业构建培训课程和材料。Office 365 组具有丰富的协作体验，是为在线课程和教师引导式课程的参与者提供交付课程内容和记录练习的绝佳方式。你可能希望将 Office 365 组用于使培训课程可轻松地被识别为培训课程，从而使其他开发人员可以发现你的组，并在你的学习课程的基础上构建丰富的体验。

针对这种应用场景，我们将介绍如何操作：

1. 查看可以使用的可用架构扩展定义
2. 注册以培训课程组为目标的架构扩展定义
3. 根据你刚刚注册的架构扩展定义，创建具有扩展数据的新组
4. 根据架构扩展定义向现有组添加或更新自定义数据
5. 读回组和扩展数据

>**注意：**本主题介绍如何在**组**资源上创建和读取架构扩展值（步骤 3-5）。**设备**、**事件**、**邮件**、**帖子**和**用户**资源类型也支持同一方法。因此可以在任意资源上执行与以下示例请求相似的操作。

## <a name="1-view-available-schema-extensions"></a>1.查看可用的架构扩展
首先，作为开发人员，可能希望找到应用可以重复使用的任何其他架构扩展定义。这可以通过查询 **schemaExtension** 资源来完成。  
在下面的示例中，将按 **id** 查询特定的架构扩展。

请注意响应中返回的扩展将**可用**作为**状态**值，即表示具有 **targetTypes** 属性中的资源访问权限的所有应用都可使用此扩展并通过增量更改更新此扩展。通常，无论**状态**如何，此操作都将返回满足指定筛选器的所有架构扩展，因此在使用扩展前请务必先检查其状态。


##### <a name="request"></a>请求
```http
GET https://graph.microsoft.com/beta/schemaExtensions/$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a>响应
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
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a>2.注册可描述培训课程的架构扩展定义
如果找不到*符合*你的需求的架构扩展，则可以在**组**资源上为培训课程创建并注册新的扩展定义。  

在创建架构扩展定义时，应为 **id** 属性提供一个字符串。可以通过两种方式来执行此操作。以下示例演示首选方法，它使用一个经租户验证的虚域名 (`graphlearn.com`)。将验证的域名 (`graphlearn`) 与架构扩展的名称 (`courses`) 相连接，并使用结果字符串 `graphlearn_courses` 分配 **id**。此外，还要指定说明（以启用可发现性）、目标类型（定义该扩展适用于哪些资源）以及构成架构的自定义属性。在本示例中，指定 `courseId`、`courseName` 和 `courseType` 自定义属性及其类型。

请参阅[分配请求中 **id** 的其他方法示例](../api-reference/beta/api/schemaextension_post_schemaextensions.md#request-2)，仅需要提供架构名称。

请注意，初次创建架构扩展时，其状态是 **InDevelopment**。在开发扩展期间，可以将其保持在此状态，在此期间仅创建该扩展的应用可以使用增量更改更新它或将其删除。准备共享此扩展以供其他应用使用时，请将**状态**设置为**可用**

##### <a name="request"></a>请求
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
##### <a name="response"></a>响应
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "graphlearn_course",
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

## <a name="3-create-a-new-group-with-extended-data"></a>3.创建具有扩展数据的新组 
使用我们刚刚注册的 `graphlearn_courses` 架构扩展定义创建一个使用额外数据扩展的新组。这是**组**资源的标准 ```POST```，其他 `graphlearn_courses` 复杂类型扩展在请求正文中定义。响应将不会返回任何数据扩展的镜像。我们需要使用 ```GET``` 操作按名称显式 ```$select``` 扩展。

##### <a name="request"></a>请求
```http
POST https://graph.microsoft.com/beta/groups
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
##### <a name="response"></a>响应
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

## <a name="4-add-or-update-custom-data-to-an-existing-group"></a>4.将自定义数据添加或更新到现有组
与上一个示例类似，我们可以使用在 ```PATCH``` 的请求正文中定义的其他 `graphlearn_courses` 复杂类型扩展来扩展现有组资源。  

##### <a name="request"></a>请求
```http
PATCH https://graph.microsoft.com/beta/groups/dfc8016f-db97-4c47-a582-49cb8f849355
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
##### <a name="response"></a>响应
```http
HTTP/1.1 204 No Content
```

如果要更新扩展数据的值，请将整个扩展复杂类型置于 ```PATCH``` 请求正文中（类似于向现有资源添加自定义数据）。

## <a name="5-get-a-group-and-its-extension-data"></a>5.获取组及其扩展数据
要获取组**及**其扩展数据，我们需要使用 `$select` 按名称指定扩展，在本例中为 `graphlearn_courses`。

#### <a name="request"></a>请求
```http
GET https://graph.microsoft.com/beta/groups/dfc8016f-db97-4c47-a582-49cb8f849355?$select=displayName,id,description,graphlearn_courses
```

##### <a name="response"></a>响应
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据（预览）](extensibility_open_users.md)
- [Office 365 域](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)
- [添加并验证新 Office 365 的域](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [schemaExtension 资源类型](../api-reference/beta/resources/schemaextension.md)
- [列出 schemaExtension](../api-reference/beta/api/schemaextension_list.md)
- [创建 schemaExtension](../api-reference/beta/api/schemaextension_post_schemaextensions.md)
- [获取 schemaExtension](../api-reference/beta/api/schemaextension_get.md)
- [更新 schemaExtension](../api-reference/beta/api/schemaextension_update.md)
- [删除 schemaExtension](../api-reference/beta/api/schemaextension_delete.md)）
