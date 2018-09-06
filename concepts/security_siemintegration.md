# <a name="integrate-microsoft-graph-security-api-alerts-with-your-siem-using-azure-monitor"></a>使用 Azure Monitor 将 Microsoft Graph 安全 API 警报与 SIEM 集成

Microsoft Graph 安全 API 通过单个的 REST 终结点，从所有 Microsoft 安全产品（统称提供程序）启用管理安全警告。 某些组织可能已将 Azure 特定日志数据通过 Azure Monitor 引入 SIEM 解决方案。 为了简化集成，通过 Microsoft Graph 安全 API 实现可用的安全警告也可以通过 Azure Monitor 由客户对其订阅进行设置。 如果组织已使用 SIEM 解决方案配置了 Azure Monitor 集成，就可以将组织的安全警报轻松地添加到通过 Azure Monitor 获取的数据中。 本文将指导你完成启用此集成的步骤。

Azure Monitor 支持连接到多个 SIEM 产品的连接器。 可以在[发送监控数据到一个事件中心](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)中找到支持的 SIEM 产品列表。 本文步骤 1 和 2 的说明涉及所有支持通过事件中心消耗的 Azure Monitor 连接器。 本文介绍了 Splunk SIEM 连接器的端到端集成。

此集成过程包含下列步骤：

1. [设置 Azure 事件中心以接收租户的安全警报](#step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant)
2. [配置 Azure Monitor 以将租户的安全警报发送至事件中心](#step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub)
3. [下载和安装 Splunk 的 Azure Monitor 加载项，以允许 Splunk 使用安全警报](#step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts)
4. [使用租户 Azure Active Directory 注册一个供 Splunk 从事件中心进行读取的应用程序](#step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub )
5. [创建 Azure Key Vault 以存储事件中心的访问密钥](#step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub)
6. [配置 Splunk 数据输入以使用存储在事件中心的安全警报](#step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub)

完成这些步骤后，Splunk Enterprise 将使用获许可租户的所有 Microsoft Graph 集成安全产品的安全警报。 许可的任何新安全产品也将通过此连接发送警报（在同一架构且无需进一步集成）。

## <a name="step-1-set-up-an-event-hubs-namespace-in-azure-to-receive-security-alerts-for-your-tenant"></a>步骤 1：在 Azure 中设置事件中心命名空间，以接收租户的安全警报。

首先，需要创建 Microsoft Azure 事件中心命名空间和事件中心。 此命名空间和事件中心是所有组织的安全警报的目标。 事件中心命名空间是共享同一访问策略的事件中心的逻辑分组。 请注意有关你创建的事件中心命名空间和事件中心的一些详细信息：

- 我们建议使用标准事件中心命名空间（尤其是当你通过这些相同的事件中心发送其他 Azure 监控数据时）。
- 通常情况下，一个吞吐量单位就已足够。 如果随着使用情况的增加而需要扩展吞吐量，则可在以后随时手动增加命名空间的吞吐量单位数或启用自动膨胀。
- 吞吐量单位数可让你增加事件中心的吞吐量比例。 分区数可让你跨多个使用者并行使用。 单个分区可执行最多 20MBps，或大约每秒 20,000 封邮件。 分区是否支持从多个分区使用要取决于使用数据的工具。 如果不确定要设置的分区数，我们建议从设置四个分区开始。
- 我们建议将事件中心的消息保留设置为 7 天。 在你使用的工具停用多天时，该设置可确保工具能够从上次停用的位置继续工作（针对最多 7 天的事件）。
- 我们建议为事件中心使用默认的使用者组。 无需创建其他使用者组或使用单独的使用者组，除非你计划用两个不同的工具使用来自同一事件中心的同一数据。
- 通常情况下，对于使用事件中心数据的计算机，必须打开端口 5671 和 5672。

另请参阅 [Azure 事件中心常见问题解答](https://docs.microsoft.com/en-us/azure/event-hubs/event-hubs-faq)。

1. 登录到 [Azure 门户](https://portal.azure.com/)，并选择屏幕左上角的“创建资源”****。

    ![创建资源图像](../concepts/images/create-resource.png)

2. 选择“物联网”****，并选择“事件中心”****。

    ![事件中心图像](../concepts/images/event-hubs.png)

3. 在“创建命名空间”**** 中，输入命名空间名称。 确保命名空间名称可用后，选择定价层（基本或标准）。 此外，选择 Azure 订阅、资源组以及创建资源的位置。 选择“创建”**** 以创建命名空间。 你可能需要等待几分钟的时间，以使系统完全预配资源。

    ![创建命名空间图像](../concepts/images/create-namespace.png)

## <a name="step-2-configure-azure-monitor-to-send-security-alerts-from-your-tenant-to-the-event-hub"></a>步骤 2：配置 Azure Monitor 以将租户的安全警报发送至事件中心

通过 Azure Monitor 为整个 Azure Active Directory (Azure AD) 租户启用组织安全警报的流式处理操作已执行一次。 所有安全 API 许可和启用的产品都将开始向 Azure Monitor 发送安全警报，流式处理数据以使用应用程序。 由组织许可和部署的任何其他启用了安全 API 的产品都将通过此相同的 Azure Monitor 配置自动流式处理安全警报。 无需在组织中进行进一步集成。

安全警报是具有很多特权的数据，通常只能由组织内的安全响应人员和全局管理员查看。 为此，在 SIEM 系统中配置租户安全警报集成所需的步骤将需要使用 Azure AD 全局管理员帐户。 此帐户在设置过程中只需使用一次，用以请求将组织的安全警报发送到 Azure Monitor。

> **注意：** 目前，Azure Monitor 诊断设置边栏选项卡不支持配置租户级资源。 Microsoft Graph 安全 API 警报是租户级资源，要求使用 Azure 资源管理器 API 配置 Azure Monitor，以支持您组织的安全警告消耗。

1. 在 Azure 订阅中，将“microsoft.insights”(Azure Monitor) 注册为资源提供程序。  
> **注意：** 不要将 "Microsoft.SecurityGraph”（Microsoft Graph 安全 API）注册为您的 Azure 订阅中的资源提供程序，因为如上文所述，"Microsoft.SecurityGraph” 是租户级资源。 租户级配置将是下面 #6 的一部分。

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

     **SUBSCRIPTION_ID** 是托管资源组和事件中心命名空间的 Azure 订阅的订阅 ID，你将在此处发送组织的安全警报。

     **RESOURCE_GROUP** 是包含事件中心命名空间的资源组，你将在此处发送组织的安全警报。

     **EVENT_HUB_NAMESPACE** 是事件中心命名空间，你将在此处发送组织的安全警报。

     **“天”：** 是你想要在事件中心保留消息的天数。

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

## <a name="step-3-download-and-install-the-azure-monitor-add-on-for-splunk-which-will-allow-splunk-to-consume-security-alerts"></a>步骤 3：下载和安装 Splunk 的 Azure Monitor 加载项，以允许 Splunk 使用安全警报

1. 这种集成仅支持 Splunk 企业部署。
2. 下载并安装 [Splunk 的 Azure Monitor 加载项](https://github.com/Microsoft/AzureMonitorAddonForSplunk)。 有关详细的安装说明，请参阅[安装](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Installation)。 **仅支持 Splunk 版本 1.2.9 或更高版本的 Azure Monitor 加载项。**
3. 成功安装加载项之后，按照 [Azure Monitor 加载项配置 wiki](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk ) 中所述的配置步骤对 Splunk 进行配置。
4. 如加载项安装说明中所述，需要在 Splunk Web 中的“管理应用”页面上通过执行禁用/启用循环，才可使加载项正常工作。 或者，可以重启 Splunk。

## <a name="step-4-register-an-application-with-your-tenant-azure-active-directory-which-splunk-will-use-to-read-from-the-event-hub"></a>步骤 4：使用租户 Azure Active Directory 注册一个供 Splunk 从事件中心进行读取的应用程序

Splunk 需要在您的组织的 Azure Active Directory 中进行应用程序注册，才能获得对 Azure Monitor 事件中心进行身份验证所需的权限和应用程序凭据。

1. 在 Azure 门户中，转到**应用注册**，然后选择**新应用程序注册**。

    ![应用注册图像](../concepts/images/app-registration.png)

2. 为应用程序选择一个名称，为类型选择 **Web 应用/API**，为登录 URL 选择 **`http://localhost`**。 然后选择“创建”****。

    ![Web API 配置](../concepts/images/app-web-config.png)

3. 应用程序创建后，复制“应用程序 ID”**** 并将其保存，以供在以后配置 Splunk 数据输入时使用。 然后，转到应用程序设置并选择“密钥”****。

    ![Web 应用 ID](../concepts/images/app-id.png)

    这将允许你生成新密钥，称为“应用程序密码”。 新密钥生成后，复制“应用程序密码”**** 并将其保存，以供在以后配置 Splunk 数据输入时使用。

4. 在包含组织安全警报的事件中心的 Azure 订阅中授予应用程序****“读取器”角色。

    ![添加 Azure 子类](../concepts/images/add-azure-sub.png)

    选择你的订阅，然后选择“访问控制 (IAM)”****。 选择“添加”**** 以添加权限。 选择应用程序并为其选择“读取器”**** 的“角色”****。

    ![添加读取器权限](../concepts/images/add-reader-perms.png)

    选择“保存”****，以将授予应用程序的权限添加到订阅。

## <a name="step-5-create-an-azure-key-vault-to-store-the-access-key-for-the-event-hub"></a>步骤 5：创建 Azure Key Vault 以存储事件中心的访问密钥

Azure Key Vault 用于存储应用程序在运行时所使用的标识、密码和证书等机密。 在此步骤中，你将创建一个 Azure Key Vault，以存储 Splunk 从包含组织安全警报的 Azure 事件中心连接和读取所需的密码。

1. 在 Azure 门户中，转到“密钥保管库”**** 并选择“添加”****。

    ![添加密钥保管库](../concepts/images/add-key-vaults.png)

2. 创建新密钥保管库后，选择“访问策略”****，为刚在步骤 4 中注册的应用程序添加新访问策略。 向应用程序授予“获取”**** 密码权限。 这将允许 Splunk（充当注册的应用程序）访问存储在此 Azure Key Vault 中的密钥（密码）。

    ![添加访问策略](../concepts/images/add-access-policies.png)

    选择“创建”****，以完成新 Azure Key Vault 的创建过程。

3. 在密钥保管库中生成新密码，以将访问密钥存储到事件中心命名空间。 首先，将访问密钥捕捉到事件中心命名空间，方法是打开事件中心命名空间并选择“共享的访问策略”****。 从列表中选择 **RootManageSharedAccessKey** 策略并从中复制“主键”****。

    ![添加共享的访问策略](../concepts/images/get-shared-policies.png)

4. 打开密钥保管库并选择“密码”****。 选择“生成/导入”****，以将新密码添加到密钥保管库。 粘贴事件中心命名空间 **RootManageSharedAccessKey** 中的“主键”****。

    ![生成新密码](../concepts/images/generate-new-secret.png)

5. 创建后，选择该密码并复制密码的“机密版本”****。 稍后将在步骤 6 中使用它来配置 Splunk 数据输入。

    ![机密版本](../concepts/images/secret-version.png)

## <a name="step-6-configure-the-splunk-data-inputs-to-consume-security-alerts-stored-in-the-event-hub"></a>步骤 6：配置 Splunk 数据输入以使用存储在事件中心的安全警报

完成设置过程的最后一步是配置 Splunk 数据输入，以利用事件中心、应用程序和在上一步骤中创建的密码。

1. 按照[配置 Splunk](https://github.com/Microsoft/AzureMonitorAddonForSplunk/wiki/Configuration-of-Splunk) 主题中的说明进行操作，打开和配置 Azure Monitor 加载项的 Splunk 数据输入。 转到“设置”**** 和“数据输入”****。 选择“Azure Monitor 诊断日志”****。
2. 选择“新建”****，并使用在上一步骤中获取的值来输入所有必填的字段。 下图显示使用本文前面示例中值的所有必填的字段。

    ![Azure Monitor 字段](../concepts/images/azure-monitor-fields.png)

3. 选择**下一步**，开始搜索从 Azure Monitor 中引入的组织安全警报。

## <a name="optional-use-splunk-search-to-explore-data"></a>（可选）使用 Splunk 搜索以浏览数据

一旦您完成 Azure Monitor Splunk 插件设置，您的 Splunk 实例将启动检索配置的事件中心事件。 默认情况下，splunk 将索引 Graph 安全警报架构的各个属性以允许搜索。

若要搜索 Graph 安全警报，创建仪表板，或使用搜索查询设置 Splunk 警报，请导航到 Splunk 中的应用程序 -> 搜索和报告应用程序。

**示例**：<br/>
尝试搜索 Graph 安全警报：

- 在搜索栏中键入 `sourcetype="amdl:securitygraph:alert"` 来获取所有通过 graph 安全 API 显示的警报。 在右侧，您将看到 Azure Monitor 日志的顶级属性，其中 Graph 安全警报位于属性栏下方。<br/>
- 在左窗格中，您将看到所选的字段和感兴趣的字段。 您可以使用所选的字段来创建仪表板或 Splunk 警报，您还可以通过右键单击字段添加或删除所选的字段。  
> **注意：** 如下面的搜索查询所示，您可以根据需要限制您的搜索。 在示例中，我们按照 Azure 安全中心的高严重性警报对 Graph 安全警报进行筛选。 我们也使用了 `eventDatetime`、`severity`、`status` 和 `provider` 作为要显示的选定字段。 有关更多高级搜索词，请参阅 [splunk 搜索教程](http://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial)。

 ![splunk_search_query](../concepts/images/splunk_search_query.png)
> 搜索查询： `sourcetype="amdl:securitygraph:alert" "properties.vendorInformation.provider"=ASC "properties.severity"=High | rename properties.eventDataTime as eventDateTime properties.severity as severity properties.vendorInformation.provider as provider properties.status as status`

Splunk 还允许通过屏幕右上角的“另存为”菜单选项对搜索结果进行多种操作。 您可以根据您的搜索筛选器创建报表、仪表板面板或警报。
下面是基于以前查询的事件流仪表板示例：您可以对每个事件添加深化链接，进一步访问 Microsoft Graph 网站上的详细信息。 请参阅 [Splunk 深化文档](http://docs.splunk.com/Documentation/Splunk/7.1.2/Viz/DrilldownIntro)。

 ![splunk_search_results](../concepts/images/splunk_search_results.png)

或者您也可以创建仪表板作为时间线图表：

 ![splunk_search_timeline](../concepts/images/splunk_search_timeline.png)

您可以参考 [Splunk 搜索与报表教程](http://docs.splunk.com/Documentation/Splunk/7.1.2/SearchTutorial/WelcometotheSearchTutorial)获得更多信息。