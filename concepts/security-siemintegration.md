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
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a><span data-ttu-id="b9e2e-106">与 SIEM 集成 Microsoft Graph 安全 API 通知</span><span class="sxs-lookup"><span data-stu-id="b9e2e-106">Integrate Microsoft Graph Security API alerts with a SIEM</span></span>

<span data-ttu-id="b9e2e-107">Microsoft Graph 安全 API，从所有 Microsoft 安全产品，称为 Microsoft Graph 安全提供程序，通过单个的 REST 终结点的管理安全警告。</span><span class="sxs-lookup"><span data-stu-id="b9e2e-107">The Microsoft Graph Security API enables managing security alerts from all Microsoft security products, known as Microsoft Graph Security providers, through a single REST endpoint.</span></span> <span data-ttu-id="b9e2e-108">某些组织可能已引入到 SIEM 解决方案 Azure 特定的日志数据通过 Azure 监视器。</span><span class="sxs-lookup"><span data-stu-id="b9e2e-108">Some organizations may already ingest Azure-specific log data through Azure Monitor into SIEM solutions.</span></span> <span data-ttu-id="b9e2e-109">为了简化集成，可还设置 Azure 监视器通过其订阅到客户可通过 Microsoft Graph 安全 API 安全警告。</span><span class="sxs-lookup"><span data-stu-id="b9e2e-109">To simplify integration, the security alerts available through the Microsoft Graph Security API can also be provisioned by the customer to their subscription via Azure Monitor.</span></span> <span data-ttu-id="b9e2e-110">如果您的组织已配置了 Azure 监视器集成与 SIEM 解决方案，您可以立即轻松 stream 贵组织的安全警告除了您可通过 Azure 监视器的现有数据。</span><span class="sxs-lookup"><span data-stu-id="b9e2e-110">If your organization has already configured Azure Monitor integration with your SIEM solution, you can now easily stream your organization’s security alerts in addition to your existing data available through Azure Monitor.</span></span>

<span data-ttu-id="b9e2e-111">Azure 监视器支持连接到多个 SIEM 产品的连接器。</span><span class="sxs-lookup"><span data-stu-id="b9e2e-111">Azure Monitor supports connectors to several SIEM products.</span></span> <span data-ttu-id="b9e2e-112">支持 SIEM 产品的列表，请参阅[监控数据到一个事件集线器发送](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)。</span><span class="sxs-lookup"><span data-stu-id="b9e2e-112">For a list of supported SIEM products, see [send monitoring data to an event hub](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub).</span></span> <span data-ttu-id="b9e2e-113">当前可供[Splunk](https://splunkbase.splunk.com/)和[QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)Microsoft Graph 安全 API 集成。</span><span class="sxs-lookup"><span data-stu-id="b9e2e-113">Microsoft Graph Security API integration is currently available for [Splunk](https://splunkbase.splunk.com/) and [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).</span></span>

<span data-ttu-id="b9e2e-114">有关 Microsoft Graph 安全 API 集成特定 SIEM 解决方案的信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="b9e2e-114">For information about Microsoft Graph Security API integration for specific SIEM solutions, see:</span></span>

- [<span data-ttu-id="b9e2e-115">Splunk</span><span class="sxs-lookup"><span data-stu-id="b9e2e-115">Splunk</span></span>](security-splunk-siemintegration.md)
- [<span data-ttu-id="b9e2e-116">QRadar</span><span class="sxs-lookup"><span data-stu-id="b9e2e-116">QRadar</span></span>](security-qradar-siemintegration.md)
