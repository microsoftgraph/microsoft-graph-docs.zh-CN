---
title: 使用外部组管理 Microsoft Graph连接器数据源的权限
description: 外部组允许你管理在 Microsoft Graph 连接中查看外部项的权限，并连接到Azure AD组外部的数据源。
author: mecampos
doc_type: conceptualPageType
ms.prod: search
ms.localizationpriority: medium
ms.openlocfilehash: 17b6b37da6f91f08cf7397b52880bb2235dc430a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211023"
---
# <a name="use-external-groups-to-manage-permissions-to-microsoft-graph-connectors-data-sources"></a>使用外部组管理 Microsoft Graph连接器数据源的权限

[外部组](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true)允许你管理在 Microsoft Graph 连接中查看[外部项](/graph/api/resources/externalconnectors-externalitem?view=graph-rest-1.0&preserve-view=true)的权限，并连接到Azure Active Directory (Azure AD) 组外部的数据源。

对于依赖于Azure AD用户和组的数据源，在[创建](/graph/api/externalconnectors-externalconnection-put-items?view=graph-rest-beta&preserve-view=true&tabs=http&viewFallbackFrom=graph-rest-1.0)或更新外部项时，通过将访问控制列表 (ACL) 与Azure AD用户和组 ID 关联来设置外部项的权限。

但是，对于使用非Azure AD组或类似组的构造（如 Salesforce 配置文件、Dynamics Business Units、SharePoint 组、ServiceNow 本地组或 Confluence 本地组）的数据源，建议使用 *外部组*。

## <a name="common-external-group-scenarios"></a>常见的外部组方案

以下是常见的非Azure AD特定于应用程序的组示例。

Microsoft Dynamics 365 允许客户使用业务部门和团队构建其 CRM。这些业务单位和团队的成员身份信息不会存储在Azure AD中。

下图显示了业务单位和团队的结构。

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/bu-teams-D365.png" alt="Diagram of a structure in Dynamics 365. A business unit has a team and a manager under it. This manager has other users." width="400px;"/></p>

Salesforce 使用配置文件、角色和权限集进行授权。 这些信息特定于 Salesforce，并且成员身份信息在Azure AD中不可用。

下图显示了 Salesforce 中成员身份信息的结构。

<!---Using html to adjust the size of the image --->
<br><p align="center"><img src="images/connectors-images/roles-salesforce.png" alt="Diagram of a structure of roles in Salesforce. The role of vice president of sales is at the top level of the hierarchy and has three subordinates, namely, the head of sales operations, the head of sales, and the head of account management. The head of sales operations has a sales operations manager as a subordinate. The head of sales has a sales development manager as a subordinate." width="500px;"/></p>

## <a name="using-external-groups-in-your-connection"></a>在连接中使用外部组

若要在连接中使用外部组，请执行以下步骤：

1. 对于每个非Azure AD组，请使用组 API 在 Microsoft Graph 中创建外部组。
2. 根据需要为外部项定义 ACL 时，请使用外部组。
3. 使外部组的成员身份保持最新和同步。

### <a name="create-an-external-group"></a>创建外部组

外部组属于连接。 若要在连接中创建外部组，请执行以下步骤：

1. 使用 Microsoft Graph中的[组 API](/graph/api/resources/group?view=graph-rest-1.0&preserve-view=true)，如以下示例所示。

    > [!NOTE]
    > [displayName](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true#properties) 和 **description** 是可选字段。

    ```http
    POST /external/connections/{connectionId}/groups

    { 
      "id": "contosoEscalations", 
      "displayName": "Contoso Escalations", 
      "description": "Tier-1 escalations within Contoso"
    } 
    ```

2. 在 ID 字段中提供标识符或名称。 使用此值在后续请求中调用外部组。

    > [!NOTE]
    > 使用 ID 字段可以使用 URL 和文件名安全的 Base64 字符集。 其限制为 128 个字符。

    外部组可以包含以下一个或多个：
    * Azure AD用户。
    * Azure AD组。
    * 另一个外部组，包括嵌套的外部组。

3. 创建组后，可以将成员添加到组，如以下示例所示。
    
    ```http
    POST https://graph.microsoft.com/beta/external/connections/{connectionId}/groups/{groupId}/members
    
    {
      "id": "contosoSupport",
      "type": "group",
      "identitySource": "external"
    }
    ```
    ```http
    POST https://graph.microsoft.com/beta/external/connections/{connectionId}/groups/{groupId}/members
    
    {
      "id": "25f143de-be82-4afb-8a57-e032b9315752",
      "type": "user",
      "identitySource": "azureActiveDirectory"
    }
    ```
    ```http
    POST https://graph.microsoft.com/beta/external/connections/{connectionId}/groups/{groupId}/members
    
    {
      "id": "99a3b3d6-71ee-4d21-b08b-4b6f22e3ae4b",
      "type": "group",
      "identitySource": "azureActiveDirectory"
    }
    ```

### <a name="use-external-groups-in-the-acl"></a>在 ACL 中使用外部组

定义外部项 [的 ACL](connecting-external-content-manage-items.md#access-control-list) 时，可以使用外部组，如以下示例所示。 除了Azure AD用户和组之外，外部项的访问控制条目中还可以包含外部组。

```http
PUT https://graph.microsoft.com/beta/external/connections/{id}/items/{id} 

Content-type: application/json 
{ 
  "@odata.type": "microsoft.graph.externalItem", 
  "acl": [ 
    { 
      "type": "group", 
      "value": "contosEscalations", 
      "accessType": "grant", 
      "identitySource": "External" 
    }, 
    { 
      "type": "user", 
      "value": "87e9089a-08d5-4d9e-9524-b7bd6be580d5", 
      "accessType": "grant", 
      "identitySource": "azureActiveDirectory" 
    }, 
    { 
      "type": "group", 
      "value": "96fbeb4f-f71c-4405-9f0b-1d6988eda2d2", 
      "accessType": "deny", 
      "identitySource": "azureActiveDirectory" 
    } 
  ], 
  "properties": { 
    "title": "Error in the payment gateway", 
    "priority": 1, 
    "assignee": "john@contoso.com" 
  }, 
  "content": { 
    "value": "<h1>Error in payment gateway</h1><p>Error details...</p>", 
    "type": "html" 
  } 
} 
```

> [!NOTE]
> 甚至在创建组之前，就可以在 ACL 中使用外部组。

### <a name="keep-external-group-memberships-in-sync"></a>保持外部组成员身份同步

在 Microsoft Graph中使外部组的成员身份保持最新。 当自定义组中的成员身份发生更改时，请确保更改在满足你需求的时间反映在外部组中。

### <a name="manage-external-groups-and-membership"></a>管理外部组和成员身份

可以使用组 API 管理外部组和组成员身份。 有关详细信息，请参阅 [externalGroup](/graph/api/resources/externalconnectors-externalgroup?view=graph-rest-1.0&preserve-view=true) 和 [externalGroupMember](/graph/api/resources/externalconnectors-externalgroupmember?view=graph-rest-beta&preserve-view=true&viewFallbackFrom=graph-rest-1.0)。

## <a name="next-steps"></a>后续步骤

- [了解 Microsoft Graph连接器 API 限制](connecting-external-content-api-limits.md)
- [使用 Microsoft Graph 连接器 API](connecting-external-content-connectors-api-overview.md)
- [将 Postman 与 Microsoft Graph 连接器 API 一并使用](connecting-external-content-connectors-api-postman.md)
