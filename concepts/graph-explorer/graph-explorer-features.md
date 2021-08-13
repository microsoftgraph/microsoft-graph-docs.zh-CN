---
title: 使用 Graph 资源管理器
description: 了解如何使用资源管理器中的一Graph功能。
localization_priority: Normal
author: bettirosengugi
ms.openlocfilehash: dab8803be00de3cc8ab27fc80c5f3b8cc0f0ac4307f29b9f276516ad13c86888
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138374"
---
# <a name="working-with-graph-explorer"></a>使用 Graph 资源管理器

[Graph资源管理器](https://developer.microsoft.com/graph/graph-explorer/)是一款开发人员工具，可方便你使用 Microsoft Graph REST API 请求并查看相应的响应。 本文介绍如何使用资源管理器中的一Graph功能。

## <a name="consent-to-permissions"></a>同意权限

用户或管理员必须通过同意Graph向浏览器授予正确的权限，以访问 Microsoft Graph。 登录时Graph"修改权限"选项卡或配置文件旁的设置齿轮中的"选择权限"选项，同意在资源管理器中授予权限。 " **修改权限** "选项卡列出了在地址栏中运行查询所需的所有权限。 

同意权限：

1.  选择一个示例查询并运行它。
2.  选择" **修改权限"** 选项卡。
3.  请参阅运行查询所需的权限列表。
4.  选择要同意的权限旁边的同意按钮。 

![Screenshot of Graph Explorer with the steps to consent to permissions highlighted](./images/modify-permissions.png)

" **修改权限"** 功能当前处于预览阶段，并且某些查询可能缺少权限。 如果查询缺少权限，则配置文件旁边的设置齿轮中的"选择权限"选项将包含所有可用权限的列表：

1.  转到设置齿轮，然后单击 **"选择权限"** 选项。 此选项包含所有可用权限的列表。
2.  从所有权限列表中，同意所需的权限。

![突出显示"Graph"选项的"资源管理器"屏幕截图](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a>获取访问或身份验证令牌

Graph资源管理器包含 **一个访问** 令牌选项卡，该选项卡显示登录时的访问令牌。 如果需要 **在** 最喜爱的 REST 客户端应用程序中使用令牌，可以在"访问令牌"选项卡上复制令牌。

![Screenshot of the Access token tab in Graph Explorer with the Copy button highlighted](./images/access-token.png)

## <a name="copy-code-snippets"></a>复制代码段

对于你在 Graph 资源管理器中选择或输入的每个 REST API 查询，你可以找到如何在代码段选项卡 -C#、Java、JavaScript 和Objective-C 下展示的四种语言中调用该 API。 

![突出显示代码Graph选项卡的"资源管理器"屏幕截图](./images/code-snippets.png)

## <a name="ui-component-integration"></a>UI 组件集成

GraphExplorer 包括多个功能，以便更轻松地实现 UI。 在应用中也重复使用这些组件。

### <a name="microsoft-graph-toolkit-integration"></a>Microsoft Graph Toolkit 集成

[Microsoft Graph Toolkit](../toolkit/overview.md)是可重用的、与框架无关的 Web 组件和帮助程序的集合，用于访问和使用 Microsoft Graph。 这些组件功能完全正常，内置提供程序使用 Microsoft Graph 进行身份验证和提取数据。

Graph资源管理器提供与 Microsoft 组件组件Graph Toolkit REST API 查询。 "组件"Toolkit **选项卡** 上的一个蓝色点指示Toolkit在资源管理器中为当前指定的 REST API 查询Graph组件。 你可以方便地将组件的代码复制到你的应用。

下表列出了当前包含应用程序组件Toolkit查询。

| **Graph资源管理器示例查询** | **Toolkit示例 iFrame URL** |
| --- | --- |
| 获取我的个人资料 | [https://mgt.dev/iframe.html?id=components-mgt-person-card—person-card-hover](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| 获取我合作的人 | [https://mgt.dev/iframe.html?id=components-mgt-people—people](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| 获取我的所有规划器任务 | [https://mgt.dev/iframe.html?id=components-mgt-tasks— 任务](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| 获取下一周的事件 | [https://mgt.dev/iframe.html?id=components-mgt-agenda—get-events-for-next-week](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| 获取我的照片	 | [https://mgt.dev/iframe.html?id=components-mgt-person—仅个人照片](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![Screenshot showing the Toolkit components tab with the code to generate the component highlighted](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a>自适应卡片集成

[自适应卡片](https://adaptivecards.io/) 是 UI 的平台不可知的代码段，以 JSON 编写，应用和服务可以开放交换。 运行查询且自适应卡片可用时，自适应卡片选项卡上会显示一个 **蓝色** 点。

![突出显示响应详细信息的 Graph 资源管理器中自适应卡片选项卡的屏幕截图](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a>在资源管理器中Graph主题

通过选择设置齿轮 **Graph"更改主题**"选项，为浏览器选择主题。 主题选项为浅色、深色和高对比度。

![Screenshot of the Change theme option in Graph Explorer with the theme options highlighted](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a>存储和共享查询

在资源管理器中Graph查询在"历史记录"选项卡中保存 30 **天。** 在"历史记录"选项卡上，您可以：

1.  导出 .har 格式的所有历史记录项。
2.  删除所有历史记录项。
3.  查看此历史记录项。
4.  运行此查询。
5.  以 .har 格式导出此历史记录项。
6.  删除此历史记录项。

![突出显示选项的"历史记录"选项卡的屏幕截图](./images/storing-and-sharing-queries.png)

若要共享您运行的查询，请单击响应窗格中的"共享查询"按钮，然后单击"复制 **"。** 这会复制链接进行共享，并允许其他人查看查询和结果。

![突出显示"Graph和复制"选项的浏览器屏幕截图](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a>Graph资源管理器 UI 功能

在希望扩大请求和响应Graph资源管理器中折叠和展开边栏组件。 若要折叠边栏组件，请选择边栏左上方的汉堡包图标。

![突出显示展开Graph折叠选项的浏览器屏幕截图](./images/expand-collapse-sidebar-component.png)

通过选择响应预览窗口中的展开箭头展开和折叠响应预览。

![突出显示展开和折叠选项的响应窗格屏幕截图](./images/expand-collapse-response-preview.png)

方便地从 Microsoft 365 资源管理器 UI 访问 Graph 开发人员计划网站，获取包含要试验的示例数据的免费沙盒。 在设置齿轮下，选择 **"获取包含示例数据的沙盒"。**

![突出显示了Graph示例数据"选项的"获取沙盒"的浏览器屏幕截图](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a>后续步骤

- 访问[Graph资源管理器](https://developer.microsoft.com/graph/graph-explorer/)并浏览示例查询。
- 浏览[Microsoft Graph Toolkit文档](../toolkit/overview.md)。
- 在资源管理器资源管理器存储库Graph或[GitHub反馈](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose)。