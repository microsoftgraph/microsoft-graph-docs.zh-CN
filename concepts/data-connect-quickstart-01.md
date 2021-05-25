<!-- markdownlint-disable MD002 MD041 -->

Microsoft Graph Data 连接通过智能Graph大规模访问丰富数据来增强 Microsoft Graph 的事务模型。 此数据涵盖工作人员如何在企业内的所有应用程序和服务中进行通信、协作Microsoft 365。 对于大数据和机器学习，连接，你可以开发用于分析、智能和业务流程优化的应用程序，Microsoft 365 Azure 中。 通过这样集成，你将能够利用 Azure 中丰富的计算和存储套件，同时符合行业标准并保持数据安全。

![此图说明了将数据Microsoft 365 Azure 云中以及输出数据之间应用的数据控件。](images/data-connect-mgdc-capabilities.png)

Microsoft Graph Data 连接 使用 Azure 数据工厂Microsoft 365数据以可配置的间隔将数据复制到应用程序存储。 它还提供了一组工具来简化向用户传递此Microsoft Azure，从而让你可以访问最适用的开发和托管工具。 数据连接还授予更精细的控制和许可模型：你可以管理数据、查看谁在访问数据以及请求实体的特定属性。 这将增强 Microsoft Graph模型，从而授予或拒绝应用程序访问整个实体。

可以使用数据连接为组织启用机器学习方案。 在这些方案中，可以创建向利益干系人提供有价值信息的应用程序，培训机器学习模型，甚至根据获取的大量数据执行预测。

## <a name="get-started"></a>入门

在本教程中，你将创建你的第一个 Microsoft Graph Data 连接 应用程序。 很让人兴奋，对不对？ 我们也认为！ 若要开始，你首先需要设置一些内容。

### <a name="prerequisites"></a>先决条件

若要完成此实验，你将需要以下订阅或许可证。

1. **Microsoft 365租赁**
  
   - 如果没有，则通过注册 (开发人员计划) 一个免费Microsoft 365[应用程序](https://developer.microsoft.com/microsoft-365/dev-program)。
   - 多个Microsoft 365接收的电子邮件的用户。
   - 访问至少两个满足以下要求的帐户：
      - 必须分配 **有全局** 管理员角色。
      - 必须具有对管理Microsoft 365的访问权限。

1. **Microsoft Azure 订阅**
  
   - 如果没有，可在 Azure 网站中 (一 [) 免费订阅](https://azure.microsoft.com/free/)。
   - 用于登录的帐户必须被授予全局管理员角色。 
   - Azure 订阅必须与 Microsoft 365 租户在同一租户中，因为 Graph Data 连接 将仅将数据导出到同一租户中的 Azure 订阅，而不是跨租户。
   - 你的Microsoft 365和 Azure 租户必须在同一Microsoft Azure Active Directory租户中。

1. 请确保你已安装[Visual Studio](https://visualstudio.microsoft.com/vs/)计算机上。

> [!NOTE]
> 此实验中使用的屏幕截图和示例来自一个Microsoft 365测试租户，该租户包含来自测试用户的示例电子邮件。 可以使用自己的租户Microsoft 365执行相同的步骤。 不会将数据写入Microsoft 365。 电子邮件数据的副本从 Microsoft 365 租户中的所有用户中提取，并复制到 Azure Blob 存储 帐户，你可以控制谁有权访问 Azure Blob 存储 内的数据。
