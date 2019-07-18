---
title: 使用 Azure Monitor 将 Microsoft Graph 安全性 API 警报与 IBM QRadar SIEM 集成
description: 可通过单个 REST 终结点管理 Microsoft Graph 安全提供程序。 可以将此终结点配置为支持多个 SIEM 产品的连接器的 Azure Monitor。 本文步骤 1 和步骤 2 中的说明指的是通过事件中心支持使用的所有 Azure Monitor 连接器。 本文介绍了 QRadar SIEM 连接器的端到端集成。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 49db00a3a667922d6d7fc50365ea1ad9282c3a8d
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778276"
---
# <a name="integrate-microsoft-graph-security-api-alerts-with-ibm-qradar-siem-using-azure-monitor"></a>使用 Azure Monitor 将 Microsoft Graph 安全性 API 警报与 IBM QRadar SIEM 集成

可通过单个 REST 终结点管理 Microsoft Graph 安全提供程序。 可以将此终结点配置为支持多个 SIEM 产品的连接器的 [Azure Monitor](https://docs.microsoft.com/zh-CN/azure/monitoring-and-diagnostics/)。 本文步骤 1 和步骤 2 中的说明指的是通过事件中心支持使用的所有 Azure Monitor 连接器。 本文介绍了 [QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem) SIEM 连接器的端到端集成。

此集成过程包含下列步骤：

1. [设置 Azure 事件中心以接收租户的安全警报](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant)。
2. [配置 Azure Monitor 以将安全警报从租户发送至事件中心](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub)。
3. [下载并安装 QRadar 以使用安全警报](#step-3-download-and-install-the-qradar-to-consume-security-alerts)。

完成这些步骤后，IBM QRadar 将使用获许可租户的所有 Microsoft Graph 集成安全产品的安全警报。 许可的任何新安全产品也将通过此连接发送警报（在同一架构且无需进一步集成）。

## <a name="step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant"></a>步骤 1：在 Azure 中设置事件中心命名空间，以接收租户的安全警报

首先，需要创建 [Microsoft Azure 事件中心](https://docs.microsoft.com/zh-CN/azure/event-hubs/)命名空间和事件中心。 此命名空间和事件中心是所有组织的安全警报的目标。 事件中心命名空间是共享同一访问策略的事件中心的逻辑分组。 请注意有关你创建的事件中心命名空间和事件中心的一些详细信息：

- 我们建议使用标准事件中心命名空间（尤其是当你通过这些相同的事件中心发送其他 Azure 监控数据时）。
- 通常情况下，一个吞吐量单位就已足够。 如果随着使用情况的增加而需要扩展吞吐量，则可在以后随时手动增加命名空间的吞吐量单位数或启用自动膨胀。
- 吞吐量单位数可让你增加事件中心的吞吐量比例。 分区数可让你跨多个使用者并行使用。 单个分区可执行最多 20MBps，或大约每秒 20,000 封邮件。 分区是否支持从多个分区使用要取决于使用数据的工具。 如果不确定要设置的分区数，我们建议从设置四个分区开始。
- 我们建议将事件中心的消息保留设置为 7 天。 在你使用的工具停用多天时，该设置可确保工具能够从上次停用的位置继续工作（针对最多 7 天的事件）。
- 我们建议为事件中心使用默认的使用者组。 无需创建其他使用者组或使用单独的使用者组，除非你计划用两个不同的工具使用来自同一事件中心的同一数据。
- 通常情况下，对于使用事件中心数据的计算机，必须打开端口 5671 和 5672。

另请参阅 [Azure 事件中心常见问题解答](https://docs.microsoft.com/zh-CN/azure/event-hubs/event-hubs-faq)。

1. 登录到 [Azure 门户](https://portal.azure.com/)，并选择屏幕左上角的“创建资源”****。

    ![创建资源图像](images/create-resource.png)

2. 选择“物联网”****，并选择“事件中心”****。

    ![事件中心图像](images/event-hubs.png)

3. 在“创建命名空间”**** 中，输入命名空间名称。 确保命名空间名称可用后，选择定价层（基本或标准）。 此外，选择 Azure 订阅、资源组以及创建资源的位置。 选择“创建”**** 以创建命名空间。 你可能需要等待几分钟的时间，以使系统完全预配资源。

    ![创建命名空间图像](images/create-namespace.png)

## <a name="step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub"></a>步骤 2：配置 Azure Monitor 以将租户的安全警报发送至事件中心

通过 Azure Monitor 为整个 Azure Active Directory (Azure AD) 租户启用组织安全警报的流式处理操作已执行一次。 所有 Microsoft Graph 安全性 API 许可和启用的产品都将开始向 Azure Monitor 发送安全警报，流式处理数据以使用应用程序。 组织许可和部署的其他任何已启用 Microsoft Graph 安全性 API 的产品，也会自动通过这一相同的 Azure Monitor 配置流式处理安全警报。 无需在组织中进行进一步集成。

安全警报是具有很多特权的数据，通常只能由组织内的安全响应人员和全局管理员查看。 为此，在 SIEM 系统中配置租户安全警报集成所需的步骤将需要使用 Azure AD 全局管理员帐户。 此帐户在设置过程中只需使用一次，用以请求将组织的安全警报发送到 Azure Monitor。

> **注意：** 目前，Azure Monitor 的“诊断设置”边栏选项卡不支持配置租户级资源。 由于 Microsoft Graph 安全性 API 警报是租户级资源，因此必须使用 Azure 资源管理器 API 将 Azure Monitor 配置为支持使用组织的安全警报。

1. 在 Azure 订阅中（可在“所有服务”下找到），将“microsoft.insights”(Azure Monitor) 注册为资源提供程序。  
 > **注意：** 不要将“Microsoft.SecurityGraph”（Microsoft Graph 安全性 API）注册为 Azure 订阅中的资源提供程序，因为“Microsoft.SecurityGraph”是租户级资源（如前所述）。 租户级配置将是下面 #6 的一部分。

2. 若要使用 Azure 资源管理器 API 配置 Azure Monitor，请获取 [ARMClient](https://github.com/projectkudu/ARMClient) 工具。 此工具将用于将 REST API 调用从命令行发送到 Azure 门户。

3. 准备诊断设置请求 JSON 文件，如下所示：

    ``` json
    {
      "location": "",
      "properties": {
        "name": "securityApiAlerts",
        "serviceBusRuleId": "/subscriptions/SUBSCRIPTION_ID/resourceGroups/RESOURCE_GROUP/providers/Microsoft.EventHub/namespaces/EVENT_HUB_NAMESPACE/authorizationrules/RootManageSharedAccessKey",
        "logs": [
          {
            "category": "Alert",
            "enabled": true,
            "retentionPolicy": {
              "enabled": true,
              "days": 7
            }
          }
        ]
      }
    }
    ```

    将 JSON 文件中的值替换为以下值：

    * **SUBSCRIPTION_ID** 是托管资源组和事件中心命名空间的 Azure 订阅的订阅 ID，你将在此处发送组织的安全警报。
    * **RESOURCE_GROUP** 是包含事件中心命名空间的资源组，你将在此处发送组织的安全警报。
    * **EVENT_HUB_NAMESPACE** 是事件中心命名空间，你将在此处发送组织的安全警报。
    * **“days”** 是要将消息保留在事件中心内的天数。

4. 以 JSON 格式将文件另存到你将从中调用 ARMClient.exe 的目录。 例如，将文件命名为 **AzMonConfig.json**。

5. 运行以下命令以登录到 ARMClient 工具。 你需要使用全局管理员帐户凭据。

    ``` shell
    ARMClient.exe login
    ```

6. 运行以下命令以将 Azure Monitor 配置为向事件中心命名空间发送安全警报。 这将自动预配命名空间内的事件中心，并启动流入事件中心的安全警报的流。 确保设置名称（在此示例中是 **securityApiAlerts**）匹配在 JSON 文件中为“名称”**** 字段指定的设置名称。

    ``` shell
    ARMClient.exe put https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview  @".\AzMonConfig.json"
    ```

7. 若要验证是否正确应用了设置，运行此命令并验证输出匹配 JSON 文件设置。

    ``` shell
    ARMClient.exe get https://management.azure.com/providers/Microsoft.SecurityGraph/diagnosticSettings/securityApiAlerts?api-version=2017-04-01-preview
    ```

8. 退出 ARMClient 工具。 现在，你已完成将租户安全警报发送到事件中心的 Azure Monitor 的配置。

## <a name="step-3-download-and-install-the-qradar-to-consume-security-alerts"></a>步骤 3：下载并安装 QRadar 以使用安全警报

1. 下载并安装 [IBM QRadar](https://www.ibm.com/us-en/marketplace/ibm-qradar-siem)。 **需要使用修补程序 7 的版本 7.2.8 或更高版本**以读取 Microsoft Azure 事件中心的事件。
2. 按照[配置 Microsoft Azure 事件中心以与 IBM QRadar 进行通信](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_dsm_guide_microsoft_azure_enable_event_hubs.html)中的步骤配置事件中心。
3. 最后，按照[使用 Microsoft Azure 事件中心协议配置 QRadar 以收集 Microsoft Azure 事件中心的事件](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/t_logsource_microsoft_azure_event_hubs.html)中的步骤开始呈现安全警报。
  
 > **注意：** 与 IBM QRadar 集成的 Microsoft Azure 支持 [Microsoft Azure DSM 规范](https://www.ibm.com/support/knowledgecenter/SS42VS_DSM/c_dsm_guide_microsoft_azure_DSM_specs.html)中列出的事件。 我们目前正在与 IBM QRadar 进行合作，以添加对 Microsoft Graph 安全性 API 警报的完全支持。 现在，你将能够接收 Microsoft 安全图形 API 警报并在 IBM QRadar 控制台中查看它们。 可以使用 [DSM 编辑器](https://www.ibm.com/support/knowledgecenter/SS42VS_7.2.8/com.ibm.qradar.doc/c_qradar_adm_dsm_ed_overview.html)分析 Microsoft 安全图形 API 警报。  
