---
title: 使用 Graph 浏览器
description: 了解如何使用 Graph 浏览器中的一些重要功能。
ms.localizationpriority: high
author: RabebOthmani
ms.openlocfilehash: bfbde32a895118816bfaa3553582d7733880bbc1
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604285"
---
# <a name="working-with-graph-explorer"></a>使用 Graph 浏览器

[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/) 是一种开发人员工具，便于发起 Microsoft Graph REST API 请求并查看相应响应。 本文介绍了如何使用 Graph 浏览器中的一些重要功能。

## <a name="consent-to-permissions"></a>同意权限

用户或管理员必须通过同意流程向 Graph 浏览器授予正确权限，从而访问 Microsoft Graph 中的数据。 登录后，通过“**修改权限**”选项卡或配置文件旁边的设置齿轮中的“**选择权限**”选项同意 Graph 浏览器中的权限。 “**修改权限**”选项卡列出了在地址栏中运行查询所需的所有权限。 

要同意权限:

1.  选择并运行示例查询。
2.  选择“**修改权限**”选项卡。
3.  查看运行查询所需的权限列表。
4.  选择要同意的权限旁边的“同意”按钮。 

![突出显示了同意权限步骤的 Graph 浏览器屏幕截图](./images/modify-permissions.png)

“**修改权限**”功能当前处于预览状态，一些查询可能缺少权限。 如果查询缺少权限，则配置文件旁边的设置齿轮中的“**选择权限**”选项包含所有可用权限的列表:

1.  转到设置齿轮并点击“**选择权限**”选项。 此选项包含所有可用权限的列表。
2.  从所有权限列表中，同意所需权限。

![突出显示了“选择权限”选项的 Graph 浏览器屏幕截图](./images/select-permissions.png)

## <a name="get-an-access-or-authentication-token"></a>获取访问令牌或身份验证令牌

Graph 浏览器包含“**访问令牌**”选项卡，该选项卡会在登录后显示访问令牌。 在“**访问令牌**”选项卡上，如果需要在最喜爱的 REST 客户端应用程序中使用该令牌，则可以进行复制。

![Graph 浏览器中“访问令牌”选项卡的屏幕截图，其中突出显示了“复制”按钮](./images/access-token.png)

## <a name="copy-code-snippets"></a>复制代码片段

对于在 Graph 浏览器中选择或输入的每个 REST API 查询，可以找到如何用“**代码片段**”选项卡下展示的四种语言 - C#、Java、JavaScript 和 Objective-C 中的每一种调用该 API。 

![突出显示了“代码片段”选项卡的 Graph 浏览器屏幕截图](./images/code-snippets.png)

## <a name="ui-component-integration"></a>UI 组件集成

Graph 浏览器包含多个功能，以简化 UI 的实现。 也可以在应用中重复使用这些组件。

### <a name="microsoft-graph-toolkit-integration"></a>Microsoft Graph 工具包集成

[Microsoft Graph 工具包](../toolkit/overview.md) 集合了可重用的、与框架无关的 Web 组件和帮助程序，用于访问和使用Microsoft Graph。 这些组件功能齐全，其内置提供程序使用 Microsoft Graph 进行身份验证并从中提取数据。

Graph 浏览器提供与 Microsoft Graph 工具包组件对应的示例 REST API 查询。 “**工具包组件**”选项卡上的蓝点指示工具包为 Graph 浏览器中当前指定的 REST API 查询提供组件。 可以轻松地将组件代码复制到应用。

下表列出了当前包含工具包组件的示例查询。

| **Graph 浏览器示例查询** | **工具包示例 iFrame URL** |
| --- | --- |
| 获取我的个人资料 | [https://mgt.dev/iframe.html?id=components-mgt-person-card—个人卡悬停](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person-card--person-card-hover&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083362882%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=9FvGlMZNc78EE66JiY7hrusYVuGUm2NeflYlVgwTVwo%3D&amp;reserved=0) |
| 获取我的合作人员 | [https://mgt.dev/iframe.html?id=components-mgt-people—人员](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-people--people&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083372878%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=yMF3X0M%2FmvWTUfhMdNYkG5I7fDMXpPHS6Fwea%2B3ycPs%3D&amp;reserved=0) |
| 获取我的所有规划器任务 | [https://mgt.dev/iframe.html?id=components-mgt-tasks—任务](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-tasks--tasks&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=Vk5IhPb%2FNbni7c6bteEveIdQNn%2BPm6AchwewCJ%2Fkmzk%3D&amp;reserved=0) |
| 获取我下周的活动 | [https://mgt.dev/iframe.html?id=components-mgt-agenda—获取下周活动](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-agenda--get-events-for-next-week&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083382869%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=VVFcx3gXMmg%2B%2BdQCZXjAmkCk5zKcrntK6fI35jbdN94%3D&amp;reserved=0) |
| 获取我的照片	 | [https://mgt.dev/iframe.html?id=components-mgt-person—仅个人照片](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fmgt.dev%2Fiframe.html%3Fid%3Dcomponents-mgt-person--person-photo-only&amp;data=04%7C01%7CElise.Yang%40microsoft.com%7Ca81f0f07873240d8571b08d7dac329d4%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637218404083392872%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&amp;sdata=aI%2BUqciLPOxEqlIpbjT8wtWBgcaJWM6sqooRlLVspZ0%3D&amp;reserved=0) |

![“工具包组件”选项卡的屏幕截图，其中突出显示了用于生成组件的代码](./images/get-graph-toolkit-card.png)

### <a name="adaptive-cards-integration"></a>自适应卡片集成

“[自适应卡片](https://adaptivecards.io/)”是以 JSON 编写的与平台无关的 UI 片段，应用和服务可以公开交换这些片段。 当运行查询且自适应卡片可用时，“**自适应卡片**”选项卡上会显示蓝点。

![Graph 浏览器中“自适应卡片”选项卡的屏幕截图，其中突出显示了响应详细信息](./images/adaptive-cards.png)

## <a name="customize-the-theme-in-graph-explorer"></a>在 Graph 浏览器中自定义主题

选择设置齿轮下的“**更改主题**”选项，以选择 Graph 浏览器的主题。 主题选项为“浅色”、“深色”和“高对比度”。

![Graph 浏览器中“更改主题”选项的屏幕截图，其中突出显示了主题选项](./images/change-theme.png)

## <a name="storing-and-sharing-queries"></a>存储并共享查询

在 Graph 浏览器中运行的查询会在“**历史记录**”选项卡中保存 30 天。在“历史记录”选项卡上，可以:

1.  以 `.har` 格式导出所有历史记录项。
2.  删除所有历史记录项。
3.  查看历史记录项。
4.  运行查询。
5.  以 `.har` 格式导出历史记录项。
6.  删除历史记录项。

![突出显示了选项的“历史记录”选项卡屏幕截图](./images/storing-and-sharing-queries.png)

要共享运行的查询，请点击响应窗格中的“共享查询”按钮，并点击“**复制**”。 此操作会复制链接，以共享并允许他人查看你的查询和结果。

![突出显示了“共享和复制”选项的 Graph 浏览器屏幕截图](./images/share-query.png)

## <a name="graph-explorer-ui-features"></a>Graph 浏览器 UI 功能

要扩大请求和响应区域，请折叠并展开 Graph 浏览器中的边栏组件。 要折叠边栏组件，请选择边栏左上角的汉堡图标。

![突出显示了“展开并折叠”选项的 Graph 浏览器屏幕截图](./images/expand-collapse-sidebar-component.png)

在响应预览窗口中选择“展开”箭头，以展开并折叠响应预览。

![突出显示了“展开并折叠”选项的响应窗格屏幕截图](./images/expand-collapse-response-preview.png)

从 Graph 浏览器 UI 轻松访问 Microsoft 365 开发人员计划网站，从而免费获取包含要试验的示例数据的沙盒。 在设置齿轮下，选择“**获取包含示例数据的沙盒**”。

![突出显示了“获取包含示例数据的沙盒”选项的 Graph 浏览器屏幕截图](./images/link-to-m365-dev-program.png)


## <a name="next-steps"></a>后续步骤

- 访问 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/) 并浏览示例查询。
- 浏览 [Microsoft Graph 工具包文档](../toolkit/overview.md)。
- 在 [Graph 浏览器 GitHub 存储库](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose) 中贡献或提供反馈。
