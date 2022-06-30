---
title: 使用 Microsoft Graph 安全性 API 实现安全解决方案集成
description: 使用这些选项连接到 Microsoft Graph 安全性 API，并在受支持的 Microsoft 和合作伙伴安全提供商之间按统一格式处理数据。
author: preetikr
ms.localizationpriority: high
ms.prod: security
ms.openlocfilehash: c221192e91d357c442dfd3eaa8ad32ae1685358e
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437546"
---
# <a name="security-solution-integrations-using-the-microsoft-graph-security-api"></a>使用 Microsoft Graph 安全性 API 实现安全解决方案集成

你可使用下述任一选项与 Microsoft Graph 安全性 API 进行连接。 这些选项让你能够通过单个集成在[受支持的 Microsoft 和合作伙伴安全提供商](/graph/api/resources/security-api-overview#alerts)之间按统一的格式处理数据：

- **使用受支持的集成选项：** 请参阅 [受支持的集成选项列表](./security-concept-overview.md#why-use-the-microsoft-graph-security-api)，例如编写代码以直接连接应用程序来获取丰富的见解。 通过[示例](https://aka.ms/graphsecurityapicode)实现入门。
- **使用 Microsoft 合作伙伴构建的本机集成和连接器：** 请参阅 [Microsoft Graph 安全性 API 合作伙伴解决方案](https://aka.ms/graphsecuritypartnerships) 以使用这些集成。  
- **使用 Microsoft 构建的连接器** - 请参阅 [连接器列表](#list-of-connectors-from-microsoft)，你可使用这些连接器通过各种解决方案与 API 相连接，以使用安全事件和管理 (SIEM)、安全响应和编排 (SOAR)、事件跟踪和服务管理 (ITSM) 以及报告功能等等。  

## <a name="list-of-connectors-from-microsoft"></a>Microsoft 连接器列表

| 解决方案类型 | 名称 | 连接器 | 公告 |
|:-----|:--------|:--------|:----------|
| SIEM |Splunk Enterprise 和 Splunk Cloud|[适用于 Splunk 的 Microsoft Graph 安全性 API 加载项](https://aka.ms/graphsecuritysplunkaddon) | [博客文章](https://aka.ms/graphsecuritysplunkaddonblogpost)<br>[Splunk on Cloud 博客文章](https://aka.ms/graphsecuritysplunkcloudblogpost)|
| SIEM |QRadar|[Microsoft Graph 安全性 API 协议和支持的 QRadar DSM](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/com.ibm.dsm.doc/c_logsource_Microsoft_Graph_Security_protocol.html)| - |
| ITSM |ServiceNow|[Microsoft Graph 安全性 API 接收集成](https://docs.servicenow.com/bundle/orlando-security-management/page/product/secops-integration-sir/secops-integration-ms-graph/concept/ms-graph-about.html)| - |
| SOAR | Azure 逻辑应用/Microsoft Flow | [适用于 Azure 逻辑应用、Microsoft Flow 和 PowerApps 的 Microsoft Graph 安全性连接器](/azure/connectors/connectors-integrate-security-operations-create-api-microsoft-graph-security) | [博客文章](https://aka.ms/graphsecurityconnectorsblogpost) |
| 自动化 | PowerShell 模块 | [Microsoft Graph 安全性 PowerShell 模块](https://aka.ms/graphsecuritypowershellmodule) | [博客文章](https://aka.ms/graphsecuritypowershellmodulepost) |
| 报告 | Power BI | [适用于 Power BI 的 Microsoft Graph 安全性连接器](/power-bi/connect-data/desktop-connect-graph-security) | [博客文章](https://aka.ms/graphsecuritypowerbiconnectorblogpost) |

若要在解决方案中支持本机集成或成为 Microsoft Graph 安全性 API的数据提供商，请参阅 [合作机会](./security-partner-overview.md)。
