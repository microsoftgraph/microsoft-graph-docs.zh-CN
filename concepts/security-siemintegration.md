---
title: 将 Microsoft Graph 安全性 API 警报与 SIEM 集成
description: 使用 Microsoft Graph 安全性 API，可以通过一个 REST 终结点管理来自所有 Microsoft 安全产品（称为“Microsoft Graph 安全提供程序”）的安全警报。 一些组织可能已通过 Azure Monitor 将 Azure 专用日志数据引入 SIEM 解决方案。 为了简化集成，通过 Microsoft Graph 安全性 API 公开的安全警报也可由客户通过 Azure Monitor 预配到自己的订阅。 如果组织已配置了 Azure Monitor 与 SIEM 解决方案集成，那么除了通过 Azure Monitor 获取的现有数据之外，现在还可以轻松地流式处理组织的安全警报。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 92a5416f68ccbc6fbbd0001c473f1daf2fe21187
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556927"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-a-siem"></a><span data-ttu-id="41569-106">将 Microsoft Graph 安全性 API 警报与 SIEM 集成</span><span class="sxs-lookup"><span data-stu-id="41569-106">Integrate Microsoft Graph Security API alerts with a SIEM</span></span>

<span data-ttu-id="41569-107">使用 Microsoft Graph 安全性 API，可以通过一个 REST 终结点管理来自所有 Microsoft 安全产品（称为“Microsoft Graph 安全提供程序”）的安全警报。</span><span class="sxs-lookup"><span data-stu-id="41569-107">The Microsoft Graph Security API enables managing security alerts from all Microsoft security products, known as Microsoft Graph Security providers, through a single REST endpoint.</span></span> <span data-ttu-id="41569-108">一些组织可能已通过 Azure Monitor 将 Azure 专用日志数据引入 SIEM 解决方案。</span><span class="sxs-lookup"><span data-stu-id="41569-108">Some organizations may already ingest Azure-specific log data through Azure Monitor into SIEM solutions.</span></span> <span data-ttu-id="41569-109">为了简化集成，通过 Microsoft Graph 安全性 API 公开的安全警报也可由客户通过 Azure Monitor 预配到自己的订阅。</span><span class="sxs-lookup"><span data-stu-id="41569-109">To simplify integration, the security alerts available through the Microsoft Graph Security API can also be provisioned by the customer to their subscription via Azure Monitor.</span></span> <span data-ttu-id="41569-110">如果组织已配置了 Azure Monitor 与 SIEM 解决方案集成，那么除了通过 Azure Monitor 获取的现有数据之外，现在还可以轻松地流式处理组织的安全警报。</span><span class="sxs-lookup"><span data-stu-id="41569-110">If your organization has already configured Azure Monitor integration with your SIEM solution, you can now easily stream your organization’s security alerts in addition to your existing data available through Azure Monitor.</span></span>

<span data-ttu-id="41569-111">可通过 SIEM 集成收到以下安全提供程序发出的警报：</span><span class="sxs-lookup"><span data-stu-id="41569-111">Alerts from the following security providers are available via SIEM integration:</span></span>

- [<span data-ttu-id="41569-112">Azure 安全中心</span><span class="sxs-lookup"><span data-stu-id="41569-112">Azure Security Center</span></span>](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [<span data-ttu-id="41569-113">Azure Active Directory Identity Protection</span><span class="sxs-lookup"><span data-stu-id="41569-113">Azure Active Directory Identity Protection</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [<span data-ttu-id="41569-114">Microsoft Cloud App Security</span><span class="sxs-lookup"><span data-stu-id="41569-114">Microsoft Cloud App Security</span></span>](https://docs.microsoft.com/cloud-app-security/monitor-alerts)
- <span data-ttu-id="41569-115">[Azure 信息保护](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive)**（预览版）**</span><span class="sxs-lookup"><span data-stu-id="41569-115">[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(preview)**</span></span>
- <span data-ttu-id="41569-116">[Azure 高级威胁防护](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories)**（预览版）**</span><span class="sxs-lookup"><span data-stu-id="41569-116">[Azure Advanced Threat Protection](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories) **(preview)**</span></span>
- <span data-ttu-id="41569-117">[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility)**（预览版）**</span><span class="sxs-lookup"><span data-stu-id="41569-117">[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(preview)**</span></span>

<span data-ttu-id="41569-118">Azure Monitor 支持连接到多个 SIEM 产品。</span><span class="sxs-lookup"><span data-stu-id="41569-118">Azure Monitor supports connectors to several SIEM products.</span></span> <span data-ttu-id="41569-119">有关受支持 SIEM 产品的列表，请参阅[将监视数据发送到事件中心](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)。</span><span class="sxs-lookup"><span data-stu-id="41569-119">For a list of supported SIEM products, see [send monitoring data to an event hub](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub).</span></span> <span data-ttu-id="41569-120">Microsoft Graph 安全性 API 集成目前适用于 [Splunk](https://splunkbase.splunk.com/) 和 [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)。</span><span class="sxs-lookup"><span data-stu-id="41569-120">Microsoft Graph Security API integration is currently available for [Splunk](https://splunkbase.splunk.com/) and [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem).</span></span>

<span data-ttu-id="41569-121">若要了解用于特定 SIEM 解决方案的 Microsoft Graph 安全性 API 集成，请参阅：</span><span class="sxs-lookup"><span data-stu-id="41569-121">For information about Microsoft Graph Security API integration for specific SIEM solutions, see:</span></span>

- [<span data-ttu-id="41569-122">Splunk</span><span class="sxs-lookup"><span data-stu-id="41569-122">Splunk</span></span>](security-splunk-siemintegration.md)
- [<span data-ttu-id="41569-123">QRadar</span><span class="sxs-lookup"><span data-stu-id="41569-123">QRadar</span></span>](security-qradar-siemintegration.md)
