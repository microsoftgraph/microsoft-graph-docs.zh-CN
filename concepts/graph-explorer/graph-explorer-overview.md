---
title: 使用 Graph 浏览器尝试 Microsoft Graph API
description: 使用 Microsoft Graph 浏览器在默认示例租户上试用 Microsoft Graph API，以浏览功能或登录到自己的租户，并将其用作原型工具来满足应用方案。
ms.localizationpriority: high
author: RabebOthmani
ms.openlocfilehash: 9f1d112cc47493b36fe455d817aa637e7fda783e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176591"
---
# <a name="use-graph-explorer-to-try-microsoft-graph-apis"></a>使用 Graph 浏览器尝试 Microsoft Graph API

[Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/) 是一种开发人员工具，便于发起 Microsoft Graph REST API 请求并查看相应响应。 使用 Microsoft Graph 浏览器在默认示例租户上试用 API，以浏览功能或登录到自己的租户，并将其用作原型工具来满足应用方案。 此工具包含代码片段（C#、Java 和 JavaScript）等有用功能、Microsoft Graph 工具包和自适应卡片集成等。

使用 Graph 浏览器：

- 发出 Microsoft Graph API 请求（GET、POST、PUT、PATCH 和 DELETE）并查看响应，包括响应代码以及任何标头和正文。
- 同意权限。 Graph 浏览器仅支持[委派权限](/graph/auth/auth-concepts#delegated-and-application-permissions)。
- 将请求正文和请求标头添加到查询。
- 查看和复制访问令牌。
- 查看 Microsoft Graph 中不同服务的示例查询。
- 查看、下载或删除最近 30 天内运行的查询。
- 查看和复制在 C#、Java 和 JavaScript 中运行的每个查询的代码片段。
- 访问 Microsoft Graph 工具包和适应卡了解部分示例查询。
- 共享查询，包括请求正文和请求标头。

Graph 浏览器为你处理身份验证过程。 通过折叠边栏或更改主题来自定义体验。

## <a name="get-started"></a>开始行动

Graph 浏览器是托管在 [Microsoft Graph 开发人员中心](https://developer.microsoft.com/en-us/graph)上的 Web 应用程序。 这是一个开源项目，我们欢迎你在 [GitHub 存储库](https://github.com/microsoftgraph/microsoft-graph-explorer-v4)中提供贡献和反馈。

Graph 浏览器包括以下元素：

1. HTTP 谓词下拉列表
2. API 版本下拉列表
3. 请求查询地址栏
4. 示例查询
5. 示例查询文档链接

:::image type="content" source="./images/getting-started.png" alt-text="Graph 浏览器用户界面的屏幕截图。" border="true":::

## <a name="make-a-get-request-in-graph-explorer"></a>在 Graph 浏览器中获取 GET 请求

若要在 Graph 浏览器中运行 GET 请求，无需登录。 只需选择一个示例查询，即可在响应预览中显示示例数据。 

:::image type="content" source="./images/making-a-get-request.png" alt-text="Graph 浏览器中示例请求的屏幕截图。" border="true":::

如果要发出请求：

1. 选择并运行示例查询。
2. 获取 HTTP 响应代码。
3. 使用示例数据查看 Microsoft Graph API 的响应。

登录到 Graph 浏览器并单击同一查询时，将从已登录的租户返回响应及实际数据。

## <a name="run-non-get-requests-in-graph-explorer"></a>在 Graph 浏览器中运行非 GET 请求

要尝试 POST、PUT、PATCH 和 DELETE 请求，请通过使用 Microsoft 365 帐户登录到 Graph 浏览器。 这可以是用于测试或演示用途的组织帐户。 若要获取免费示例 Microsoft 365 E5 开发人员订阅，以及工具和其他资源，以帮助你为 Microsoft 365 平台生成解决方案，请加入 [Microsoft 365开发人员计划](https://developer.microsoft.com/microsoft-365/dev-program)。 

>[!IMPORTANT]
>如果选择通过使用组织帐户登录，则运行非 GET 请求可能会影响租户中的数据。

例如，若要运行 POST 请求，请在 HTTP 谓词的下拉列表中选择 POST，并根据需要添加请求正文和请求标头。

:::image type="content" source="./images/making-a-post-request.png" alt-text="Graph 浏览器中 POST 请求的屏幕截图。" border="true":::

1. 选择 POST 示例查询。
2. 更新 **请求正文**；例如，为应用程序命名。
3. 选择 **运行查询**。
4. 请查看来自 Microsoft Graph API 的响应。

要以非默认 JSON 的格式查看响应，请在请求窗格中选择“**请求标头**”选项卡，定义密钥/值对，然后选择“**添加**”。

:::image type="content" source="./images/adding-key-value-pairs.png" alt-text="显示 Graph 浏览器中的&quot;请求标头&quot;选项卡屏幕截图。" border="true":::

## <a name="next-steps"></a>后续步骤

- 试用 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/)。
- 详细了解 [Graph 浏览器功能](./graph-explorer-features.md)。
- 在 [GitHub 存储库](https://github.com/microsoftgraph/microsoft-graph-explorer-v4/issues/new/choose) 中贡献或提供反馈。
