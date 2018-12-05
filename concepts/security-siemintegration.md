---
title: 与 SIEM 集成 Microsoft Graph 安全 API 通知
description: Microsoft Graph 安全 API，从所有 Microsoft 安全产品，称为 Microsoft Graph 安全提供程序，通过单个的 REST 终结点的管理安全警告。 某些组织可能已引入到 SIEM 解决方案 Azure 特定的日志数据通过 Azure 监视器。 为了简化集成，可还设置 Azure 监视器通过其订阅到客户可通过 Microsoft Graph 安全 API 安全警告。 如果您的组织已配置了 Azure 监视器集成与 SIEM 解决方案，您可以立即轻松 stream 贵组织的安全警告除了您可通过 Azure 监视器的现有数据。
ms.openlocfilehash: ca2952163ab8894cae4c22f726b45b1be94a8b1f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091843"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a>与 SIEM 集成 Microsoft Graph 安全 API 通知

Microsoft Graph 安全 API，从所有 Microsoft 安全产品，称为 Microsoft Graph 安全提供程序，通过单个的 REST 终结点的管理安全警告。 某些组织可能已引入到 SIEM 解决方案 Azure 特定的日志数据通过 Azure 监视器。 为了简化集成，可还设置 Azure 监视器通过其订阅到客户可通过 Microsoft Graph 安全 API 安全警告。 如果您的组织已配置了 Azure 监视器集成与 SIEM 解决方案，您可以立即轻松 stream 贵组织的安全警告除了您可通过 Azure 监视器的现有数据。

Azure 监视器支持连接到多个 SIEM 产品的连接器。 支持 SIEM 产品的列表，请参阅[监控数据到一个事件集线器发送](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)。 当前可供[Splunk](https://splunkbase.splunk.com/)和[QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)Microsoft Graph 安全 API 集成。

有关 Microsoft Graph 安全 API 集成特定 SIEM 解决方案的信息，请参阅：

- [Splunk](security-splunk-siemintegration.md)
- [QRadar](security-qradar-siemintegration.md)
