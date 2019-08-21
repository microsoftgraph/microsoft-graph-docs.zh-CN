---
title: 使用 Microsoft Graph 安全性 API 实现安全解决方案集成
description: 可使用本文中描述的任一选项与 Microsoft Graph 安全性 API 进行连接。 这些选项让你能够通过单个集成在受支持的 Microsoft 和合作伙伴安全提供商之间按统一的格式处理数据。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 362dde5c75180bfe1edbf42f49bcbe009af9015a
ms.sourcegitcommit: 496269b62d42cb7a96752a77b0f2e0cb16918f0b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2019
ms.locfileid: "36484406"
---
# <a name="security-solution-integrations-using-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API 实现安全解决方案集成

你可使用下述任一选项与 Microsoft Graph 安全性 API 进行连接。 这些选项让你能够通过单个集成在[受支持的 Microsoft 和合作伙伴安全提供商](https://aka.ms/graphsecurityalerts)之间按统一的格式处理数据。

- **直接使用受支持的集成选项** - 要直接连接应用程序来获取丰富的见解，请参阅[受支持的集成选项列表](https://docs.microsoft.com/graph/security-concept-overview#why-use-the-microsoft-graph-security-api)（例如编写代码）。 通过[示例](https://aka.ms/graphsecurityapicode)实现入门。
- **使用 Microsoft 合作伙伴构建的本机集成和连接器** - 要使用这些集成，请参阅 [Microsoft Graph 安全性 API 合作伙伴解决方案](https://aka.ms/graphsecuritypartnerships)。  
- **使用 Microsoft 构建的连接器** - 请参阅[连接器列表](https://aka.ms/graphsecuritysolutionsconnectors)，你可使用这些连接器通过各种解决方案与 API 相连接，以使用安全事件和管理 (SIEM)、安全响应和编排 (SOAR)、事件跟踪和服务管理 (ITSM) 以及报告功能等等。  

## <a name="list-of-connectors-from-microsoft"></a>Microsoft 连接器列表

| 解决方案类型 | 名称 | 连接器 | 公告 |
|:-----|:--------|:--------|:----------|
| SIEM |Splunk |[适用于 Splunk 的 Microsoft Graph 安全性 API 加载项](https://aka.ms/graphsecuritysplunkaddon) | [博客文章](https://aka.ms/graphsecuritysplunkaddonblogpost) |
| SOAR | Azure 逻辑应用/Microsoft Flow | [适用于 Azure 逻辑应用、Microsoft Flow 和 PowerApps 的 Microsoft Graph 安全性连接器](https://aka.ms/graphsecurityconnectors) | [博客文章](https://aka.ms/graphsecurityconnectorsblogpost) |
| 自动化 | PowerShell 模块 | [Microsoft Graph 安全性 PowerShell 模块](https://aka.ms/graphsecuritypowershellmodule) | [博客文章](https://aka.ms/graphsecuritypowershellmodulepost) |
| 报告 | Power BI | [适用于 Power BI 的 Microsoft Graph 安全性连接器](https://aka.ms/graphsecuritypowerbiconnectordoc) | [博客文章](https://aka.ms/graphsecuritypowerbiconnectorblogpost) |

如果你想要在解决方案中支持本机集成或者你是 Microsoft Graph 安全性 API 的数据提供商，请参阅[合作伙伴关系机遇](https://docs.microsoft.com/graph/security-partner-overview)。
