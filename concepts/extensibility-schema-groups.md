---
title: '使用架构扩展向组添加自定义数据 '
description: '本文将通过一个示例逐步介绍如何使用 *架构扩展*。 '
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: c4226a642c2e6651cf4168c81d7188f0edd76270
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240654"
---
# <a name="add-custom-data-to-groups-using-schema-extensions"></a>使用架构扩展向组添加自定义数据 

本文将通过一个示例逐步介绍如何使用 *架构扩展*。 

假设你是一个名为“Graph Learn”的学习管理软件公司的开发人员，工作是为企业构建培训课程和材料。Microsoft 365 组具有丰富的协作体验，是为在线课程和教师引导式课程的参与者提供交付课程内容和记录练习的绝佳方式。你可能希望将那些 Microsoft 365 组用于使培训课程可轻松地被识别为培训课程，从而使其他开发人员可以发现你的组，并在你的学习课程的基础上构建丰富的体验。

在此情况下，本文将介绍如何：

1. 查看可以使用的可用架构扩展定义。
2. 注册以培训课程组为目标的架构扩展定义。
3. 根据你刚刚注册的架构扩展定义，创建具有扩展数据的新组。
4. 根据架构扩展定义向现有组添加、更新或删除自定义数据。
5. 读回组和扩展数据。

>**注意：** 本主题介绍如何在 **组** 资源上创建和读取架构扩展值（步骤 3-5）。**管理单元**、**设备**、**事件**、**邮件**、**组织**、**帖子** 和 **用户** 资源类型也支持相同方法。你可以对任意资源执行与本文中的请求示例相似的操作。请注意，**administrativeUnit** 仅适用于 beta 终结点。

## <a name="1-view-available-schema-extensions"></a>1.查看可用的架构扩展
首先，作为开发人员，可能希望找到应用可以重复使用的任何其他架构扩展定义。这可以通过查询 **schemaExtension** 资源来完成。  
在下面的示例中，将按 **id** 查询特定的架构扩展。

请注意响应中返回的扩展将 **可用** 作为 **状态** 值，即表示具有 **targetTypes** 属性中的资源访问权限的所有应用都可使用此扩展并通过增量更改更新此扩展。通常，无论 **状态** 如何，此操作都将返回满足指定筛选器的所有架构扩展，因此在使用扩展前请务必先检查其状态。


### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-get"
}-->
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json

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
如果找不到 *符合* 你的需求的架构扩展，则可以在 **组** 资源上为培训课程创建并注册新的扩展定义。  

在创建架构扩展定义时，应为 **id** 属性提供一个字符串。可以通过两种方式来执行此操作。以下示例演示首选方法，它使用一个经租户验证的虚域名 (`graphlearn.com`)。将验证的域名 (`graphlearn`) 与架构扩展的名称 (`courses`) 相连接，并使用结果字符串 `graphlearn_courses` 分配 **id**。  

然后，还要指定说明（以启用可发现性）、目标类型（定义该扩展适用于哪些资源）以及构成架构的自定义属性。在本示例中，指定 `courseId`、`courseName` 和 `courseType` 自定义属性及其类型。

请参阅 [分配请求中 **id** 的其他方法示例](/graph/api/schemaextension-post-schemaextensions#request-2)，仅需要提供架构名称。

请注意，初次创建架构扩展时，其状态是 **InDevelopment**。在开发扩展期间，可以将其保持在此状态，在此期间仅创建该扩展的应用可以使用增量更改更新它或将其删除。准备共享此扩展以供其他应用使用时，请将 **状态** 设置为 **可用**

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-createExtension"
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

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
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

## <a name="3-create-a-new-group-with-extended-data"></a>3.创建具有扩展数据的新组 
使用我们刚刚注册的 `graphlearn_courses` 架构扩展定义创建一个 _新_ 组并使用额外数据进行扩展。这是 **组** 资源的标准 ```POST```，其他 `graphlearn_courses` 复杂类型扩展在请求正文中定义。响应将不会返回任何数据扩展的镜像。我们需要使用 ```GET``` 操作按名称显式 ```$select``` 扩展。

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-createGroupWithExtension"
}-->
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
### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
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

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a>4.在现有组中添加、更新或删除自定义数据
可以使用在 ```PATCH``` 请求的正文中定义的其他 `graphlearn_courses` 复杂类型扩展来扩展自定义数据并将其添加到 _现有_ 组实例。  

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-updateGroupWithExtension"
}-->
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

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

如果要更新扩展数据的值，请将整个扩展复杂类型置于 ```PATCH``` 请求正文中（类似于向现有资源添加自定义数据）。

还可以将相应的扩展属性设置为 null，从而删除添加到资源实例中的自定义数据。 

若要将架构扩展从资源实例中删除，请将该实例中的扩展复杂类型设置为 null。


## <a name="5-get-a-group-and-its-extension-data"></a>5.获取组及其扩展数据
查找组的简便方法有：使用 `$filter` 匹配特定的扩展属性值，比如扩展名或 ID。 

然后，使用 `$select` 按名称包含扩展（在此情况下按 `graphlearn_courses`）获取组中的自定义数据。

下面的示例查找了具有 `graphlearn_courses` 扩展且 `courseId` 属性值与 `123` 相匹配的组，获取了组属性 **displayName**、 **id** 和 **description**，以及 `graphlearn_courses` 扩展中的自定义数据。（在实际查询中，请确保根据需要应用 URL 编码。）

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "schemaextensions-groups-getGroupSelectExtension"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
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

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](extensibility-overview.md)
- [使用开放扩展向用户添加自定义数据（预览）](extensibility-open-users.md)
- [Microsoft 365 域](/office365/servicedescriptions/office-365-platform-service-description/domains)
- [添加并验证新 Microsoft 365 的域](/microsoft-365/admin/setup/add-domain)
- [schemaExtension 资源类型](/graph/api/resources/schemaextension)