---
title: 将 Microsoft Graph 安全性 API 警报与 SIEM 集成
description: 使用 Microsoft Graph 安全性 API，可以通过一个 REST 终结点管理来自所有 Microsoft 安全产品（称为“Microsoft Graph 安全提供程序”）的安全警报。 一些组织可能已通过 Azure Monitor 将 Azure 专用日志数据引入 SIEM 解决方案。 为了简化集成，通过 Microsoft Graph 安全性 API 公开的安全警报也可由客户通过 Azure Monitor 预配到自己的订阅。 如果组织已配置了 Azure Monitor 与 SIEM 解决方案集成，那么除了通过 Azure Monitor 获取的现有数据之外，现在还可以轻松地流式处理组织的安全警报。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 92a5416f68ccbc6fbbd0001c473f1daf2fe21187
ms.sourcegitcommit: 10adbecb5f82556e5acc2301fc226ae6884e142b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2019
ms.locfileid: "30693685"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>将 Microsoft Graph 安全性 API 警报与 SIEM 集成

使用 Microsoft Graph 安全性 API，可以通过一个 REST 终结点管理来自所有 Microsoft 安全产品（称为“Microsoft Graph 安全提供程序”）的安全警报。 一些组织可能已通过 Azure Monitor 将 Azure 专用日志数据引入 SIEM 解决方案。 为了简化集成，通过 Microsoft Graph 安全性 API 公开的安全警报也可由客户通过 Azure Monitor 预配到自己的订阅。 如果组织已配置了 Azure Monitor 与 SIEM 解决方案集成，那么除了通过 Azure Monitor 获取的现有数据之外，现在还可以轻松地流式处理组织的安全警报。

可通过 SIEM 集成收到以下安全提供程序发出的警报：

- [Azure 安全中心](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Azure Active Directory Identity Protection](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts)
- [Azure 信息保护](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览版）**
- [Azure 高级威胁防护](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories)**（预览版）**
- [Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility)**（预览版）**

Azure Monitor 支持连接到多个 SIEM 产品。 有关受支持 SIEM 产品的列表，请参阅[将监视数据发送到事件中心](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)。 Microsoft Graph 安全性 API 集成目前适用于 [Splunk](https://splunkbase.splunk.com/) 和 [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)。

若要了解用于特定 SIEM 解决方案的 Microsoft Graph 安全性 API 集成，请参阅：

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
