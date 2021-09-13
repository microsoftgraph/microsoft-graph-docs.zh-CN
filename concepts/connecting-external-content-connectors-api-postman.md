---
title: 将 Postman 与 Microsoft Graph 连接器 API 一并使用
description: 使用 Postman 试用连接器 API
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 15587804b130a009abc936ceb8af4379f67fcea2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139357"
---
# <a name="use-postman-with-the-microsoft-graph-connectors-api"></a>将 Postman 与 Microsoft Graph 连接器 API 一并使用

本主题介绍如何将 Microsoft Graph 连接器 API 与 Postman 一并使用。

## <a name="prerequisites"></a>先决条件

* Microsoft 帐户或者工作或学校帐户。
* 访问 Microsoft 365 开发人员租户。如果没有，可以注册 [Microsoft 365 开发人员计划]，以获取免费的开发人员订阅。

## <a name="step-1---import-the-microsoft-graph-postman-collection"></a>步骤 1 - 导入 Microsoft Graph Postman 集合

要使用 Postman 集合，需要将其导入到 Postman 工作区。从 Web 浏览器执行此操作。

1. 转到 [Postman](https://identity.getpostman.com/signup) 并登录。 如果已有 Postman 帐户， [登录](https://identity.getpostman.com/login)。

2. 登录后，转到" **工作区**。

![屏幕截图显示"发布人"中的"工作区"选项卡和"选择我的工作区"的选项](./images/connectors-images/02-postman-my-workspace.png)

3. 转到 **"我的工作区"** 后， 选择 **"导入** 按钮。

![一张屏幕截图，显示 Postman 中的"我的工作区"部分和"导入"选项](./images/connectors-images/03-postman-import.png)

4. 在打开的对话框中，选择 **链接** 选项卡，然后输入以下 URL - 在文本框中：  `https://www.postman.com/collections/61bfc772fe030514b062`。

!["导入"对话框的屏幕截图](./images/connectors-images/04-postman-link.png)

5. 选择 **继续**。
6. 选择“**导入**”。

![输入 URL 后"导入"对话框的屏幕截图](./images/connectors-images/05-postman-link-continue.png)

现在，你应该在 Postman 内看到 Microsoft Graph 连接器 API 集合。

![显示 Postman 中的 Microsoft Graph Connector API 的屏幕截图](./images/connectors-images/06-postman-collection-tab.png)

> [!NOTE]
> Microsoft Graph connector API 最近已添加到 [Microsoft Graph 邮政编码集合中](https://www.postman.com/microsoftgraph/workspace/microsoft-graph/overview)。
将很快编辑此文档以改为使用该集合。

## <a name="step-2---download-the-postman-agent-optional---postman-web-browser-only"></a>步骤 2 - 下载Postman代理（可选 - 仅适用于 Postman Web 浏览器）

要在 web 浏览器中使用此 Postman 集合，请下载 [Postman 桌面代理](https://www.postman.com/downloads)。 由于 web 浏览器的限制，无法在未下载此代理的情况下在 web 上使用 Postman。
“每个Microsoft 365租户的最大[连接](/graph/api-reference/resources/externalconnection?view=graph-rest-beta&preserve-view=true)资源数。”

> [!NOTE]
> 如果你正在使用 Postman for Windows 应用，则不需要此代理。 如果打开 Postman for Windows 后，你会在工作区中看到这个分支集合。

## <a name="step-3---create-an-azure-ad-application"></a>第三步 - 创建 Azure AD 应用程序

要在你的开发者租户中使用此集合，请创建一个 Azure AD 应用程序并根据想要调用的请求给予其合适的权限。

1. 转到 [portal.azure.com](https://portal.azure.com/) ， 并使用您的开发人员租户管理员帐户 **登录**。
2. 在 Azure 服务下， 选择 **Azure Active Directory**。
3. 在左侧菜单上，选择 **注册**。
4. 在水平菜单中，单击“**新建注册**”。
5. 将应用程序名称设置为"部件库存"。
6. 将"重定向 URI"设置为 https://oauth.pstmn.io/v1/browser-callback。
7. 选择“**注册**”。
8. 在左侧菜单上，选择 **API 权限**。
9. 在水平菜单中，**Microsoft Graph** > **权限或** > **权限添加**。
10. 开始键入内容 `ExternalItem.ReadWrite.All` 并选中 `ExternalItem.ReadWrite.All`。
11. 选择 **权限**，键入"用户"，然后选中 **权限**。
12. 展开 **用户选项，** 并选中 **`ExternalItem.ReadWrite.All`**。
13. 选择 **添加权限**。
14. 在水平菜单中，选择 **授予管理员对** 许可， **"是**。
15. 在左侧的菜单中，选择 **概述**。 在这里，你可以获取应用程序（客户端）ID 和目录（租户）ID。 这些会在第四步中用到。
16. 在左侧的菜单中， **证书和秘诀**。
17. 选择“**新建客户端机密**”，并输入简短说明，然后选择“**添加**”。 复制新的客户端密码值，将在步骤 4 中需要该密码。

现在，Azure AD应用程序具有代表用户发出呼叫请求`ExternalItem.ReadWrite.All`的权限，并作为`ExternalItem.ReadWrite.All`的应用程序。

## <a name="step-4--configure-authentication"></a>步骤 4：配置身份验证

在 Postman 中设置变量。 此信息用于生成访问令牌。

1. 选择 **Microsoft Graph connectors API** 选项卡，然后转到" **变量** 部分。

![Microsoft Graph 连接器 API 选项卡和"变量"部分屏幕截图](./images/connectors-images/07-postman.png)

2. 在"变量"部分，使用步骤 3 中的信息提供所需信息。

- 从步骤3.15开始，将 **客户端\_id** 的 **当前值** 设置为应用程序（客户端）ID值。
- 从步骤3.17开始，将 **客户端\_密码** 的 **当前值** 设置为客户端密码值。
- 从步骤3.15开始，将 **租户** 的 **当前值** 设置为目录（租户）ID 值。
- 将 **用户名** 的 **当前值** 设置为`admin@xxxxxxx.onmicrosoft.com`
- 将 **密码** 的 **当前值** 设置为租户管理员密码。

![显示所选变量的屏幕截图](./images/connectors-images/08-postman.png)

3. 选择“**保存**” / “**更新**”。

## <a name="step-5---get-an-authentication-token"></a>步骤 5 - 获取身份验证令牌

由于这是你第一次通过应用程序身份验证流程运行请求，你需要获取访问令牌。 通过以下 POST 请求获取应用访问令牌：

!["获取应用访问令牌"分区的屏幕截图](./images/connectors-images/09-postman.png)


以下示例显示了如何获取共享密码的访问令牌：
```html
POST /{{tenant}}/oauth2/v2.0/token HTTP/1.1 //Line breaks for clarity
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id={{client_id}} 
&scope=https%3A%2F%2Fgraph.microsoft.com%2F.default 
&client_secret={{client_secret}} 
&grant_type=client_credentials 
```
以下示例显示了成功响应：
```html
{ 
    "token_type": "Bearer", 
    "expires_in": 3599, 
    "ext_expires_in": 3599, 
    "access_token": "eyJ0eXAiOiJKV1QiLCJu… " 
} 
```

请注意，你正在通过此处 [客户端凭据](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 流。 请确保获取应用访问令牌，而不是用户访问令牌。

## <a name="step-6--create-a-new-connection"></a>步骤 6 - 创建新连接

[连接](/concepts/connecting-external-content-manage-connections.md)是外部数据的逻辑容器，您可以作为一个单元进行管理。 选择连接名称、ID 和说明。 从管理员获取连接到数据源的必要详细信息，并提供一种机制，在设置连接时授权处理内容源。 可使用 [Microsoft Graph SDK](/graph/sdks/sdks-overview) 和API对连接器设置进行编程。 如果要存储凭据，则可以使用Azure Key Vault。

```http
POST /external/connections
```

下面展示了示例请求。

```http
POST https://graph.microsoft.com/beta/external/connections 
Content-type: application/json 

{ 
  "id": "contosotasks", 
  "name": "Contoso Tasks", 
  "description": "Connection to index Contoso task management system" 
} 
```

下面介绍响应示例。

```http
HTTP/1.1 201 Created 
Content-type: application/json 
 
{ 
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connections/$entity", 
    "id": "contosotasks", 
    "name": "Contoso Tasks", 
    "description": "Connection to index Contoso task management system", 
    "state": null, 
    "configuration": { 
        "authorizedApps": [ 
            "a47b35b7-6271-4e6d-9e27-2450a8b9c6b6" 
        ] 
    } 
} 
```

以下是 **“创建连接”** 部分的屏幕快照。

 !["创建连接"分区的屏幕截图](./images/connectors-images/10-postman.png)

## <a name="step-7---register-connection-schema"></a>步骤 7 - 注册连接架构

连接架构确定各种 Microsoft Graph 体验中如何使用你的内容。 架构是计划添加到连接中的所有属性的简单列表及其属性、标签和别名。 向连接添加项目前，必须注册架构。

```http
POST /external/connections/{id}/schema 
```

下面展示了示例请求。

```http
POST https://graph.microsoft.com/beta/external/connections/contosotasks/schema 
Content-type: application/json 
Prefer: respond-async 

{ 
  "baseType": "microsoft.graph.externalItem", 
  "properties": [ 
    { 
"name": "title", 
      "type": "String", 
      "isSearchable": "true", 
"isQueryable": "true", 
      "isRetrievable": "true", 
      "labels": [ 
        "title" 
      ] 
    }, 
    { 
"aliases": "creator", 
      "name": "createdBy", 
      "type": "String", 
      "isSearchable": "true", 
"isQueryable": "true", 
      "isRetrievable": "false", 
"isRefinable": "false", 
      "labels": [ 
        "createdBy" 
      ] 
    }, 
    { 
"aliases": "editedDate", 
      "name": "lastEditedDate", 
      "type": "DateTime", 
      "isSearchable": "false", 
"isQueryable": "true", 
      "isRetrievable": "true", 
"isRefinable": "true", 
      "labels": [ 
   "lastModifiedDateTime" 
] 
    } 
  ] 
} 
```

下面介绍响应示例。

```http
HTTP/1.1 202 Accepted 
Location: https://graph.microsoft.com/beta/external/connections/contosotasks/operations/616bfeed-666f-4ce0-8cd9-058939010bfc 
```

> [!NOTE]
> 注册连接架构是一个异步操作，因此在连接架构进入“完成”状态之前，请勿将项目进入连接中。要检查连接架构状态，请执行以下请求：
> ```http
> GET /external/connections/contosotasks/operations/616bfeed-666f-4ce0-8cd9-058939010bfc 
> ```

下面是另一个请求示例。
```http
Request 
GET https://graph.microsoft.com/beta/external/connections/operations/616bfeed-666f-4ce0-8cd9-058939010bfc 
```

以及下一个各自答复示例。

```http
HTTP/1.1 200 OK 
Content-type: application/json 

{
    @odata.context":"https://graph.microsoft.com/beta/$metadata#external/connections('coursecatalog')/operations/$entity", 
    "id": "aa9186d2-893c-4361-ca51-431d88fa45d8", 
    "name": "Contoso Tasks", 
    "status": "inprogress", 
    "error": null  
}
```

以下是 **“获取操作状态”** 部分的屏幕截图。

![显示正在进行状态的"获取操作状态"分区的屏幕截图](./images/connectors-images/11-postman.png)

将连接架构操作状态从 **“进行中”** 更改为 **“完成”后，** 您可以提取该连接的项目。

以下屏幕截图显示状态为"已完成"。

 ![显示状态已完成的"获取操作状态"分区的屏幕截图](./images/connectors-images/12-postman.png)

以下屏幕截图将状态显示为"草稿"。

 ![显示状态草稿的"获取操作状态"分区的屏幕截图](./images/connectors-images/13-postman.png)

连接状态从 **草稿****准备就绪**（如下一个屏幕截图所示）后，您可以将项目放入当前连接。

![显示状态已准备就绪的"获取操作状态"分区的屏幕截图](./images/connectors-images/14-postman.png)

## <a name="step-8---add-external-group-member-optional"></a>步骤 8 - 添加外部团队成员（可选）

如果外部服务使用非 Azure AD ACL，请同步这些权限。  

外部组（以及 Azure Active Directory 用户和组）用于设置 `externalItems` Microsoft Graph 连接的权限。 有关详细信息，请参阅 [externalGroups](/graph/api/resources/externalgroup?view=graph-rest-beta)。

这是一个请求示例。

```http
POST https://graph.microsoft.com/beta/external/connections/contosotasks/groups/31bea3d537902000/members 
Content-Type: application/json 
 
{ 
  "@odata.type": "#microsoft.graph.externalGroupMember", 
  "id": "1431b9c38ee647f6a", 
  "type": "group", 
  "identitySource": "external" 
} 
```

下面是一个响应示例。

```http
HTTP/1.1 201 Created 
Content-Type: application/json 

{ 
  "@odata.type": "#microsoft.graph.externalGroupMember", 
  "id": "14m1b9c38qe647f6a", 
  "type": "group", 
  "identitySource": "external" 
} 
```

以下屏幕截图显示了 **“创建外部组”** 部分。

!["创建外部组"分区的屏幕截图](./images/connectors-images/15-postman.png)

## <a name="step-9---ingest-items"></a>步骤 9 - 正在购买项目

创建连接后，可以添加内容。 数据源中的每个项目必须用唯一项目 id `externalItem` Microsoft Graph 中表示为对象。此 ID 用于创建、更新或删除 Microsoft Graph 中的项目。 可使用数据源中的主键作为源 `itemId` 或来自一个或多个字段的主键。 控件 `externalItem` 三个关键组件：访问控制列表、属性和内容。

如果有二进制文件，则必须进行分析以获得元数据和内容的文本版本。 如果有 PDF 或 BMP 文件等非文本内容，则必须使用对象字符识别将内容转换为文本。  

你负责转换源权限以授予或拒绝。 拒绝优先于授予。

请求示例如下所示。

```http
PUT https://graph.microsoft.com/beta/connections/contosohr/items/TSP228082938 
Content-type: application/json 

{ 
  "@odata.type": "microsoft.graph.externalItem", 
  "acl": [ 
    { 
      "type": "user", 
      "value": "e811976d-83df-4cbd-8b9b-5215b18aa874", 
      "accessType": "grant", 
      "identitySource": "azureActiveDirectory" 
    }, 
    { 
      "type": "group", 
      "value": "14m1b9c38qe647f6a", 
      "accessType": "deny", 
      "identitySource": "external" 
    } 
  ], 
  "properties": { 
    "ticketID": "1158", 
    "priority": 1, 
    "title": "Filter design", 
  }, 
  "content": { 
    "value": "Build filtering capability by...", 
    "type": "text" 
  } 
} 
```

下面是成功响应的示例。

```http
HTTP/1.1 200 OK
```

## <a name="error-handling"></a>错误处理

若要详细了解如何解决错误，请参阅 [Microsoft Graph 授权](/graph/resolve-auth-errors)。
