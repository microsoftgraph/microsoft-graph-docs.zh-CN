---
ms.localizationpriority: medium
ms.openlocfilehash: f0ba3bbafa065bce8bb29fa760704df691bd5d79
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289522"
---
<!-- markdownlint-disable MD002 MD041 -->

Microsoft Graph 数据连接通过智能方式大规模访问丰富数据，增强了 Microsoft Graph 的事务性模型。 这些数据涵盖员工如何在 Microsoft 365 中的所有应用程序和服务之间进行沟通、协作和管理时间。 数据连接是大数据和机器学习的理想选择，让你能够通过将 Microsoft 365 数据扩展到 Azure 来开发用于分析、智能和业务流程优化的应用程序。 通过以这种方式集成，你将能够利用 Azure 中的大量计算、存储套件，同时保持符合行业标准并确保数据安全。

![此图说明了将数据Microsoft 365 Azure 云中以及输出数据之间应用的数据控件。](images/data-connect-mgdc-capabilities.png)

Microsoft Graph 数据连接使用 Azure 数据工厂以可配置的时间间隔将 Microsoft 365 数据复制到应用程序的存储中。 它还提供了一组工具来简化向 Microsoft Azure 传送此数据的过程，让你可以访问最适用的开发和托管工具。 数据连接还授权更精细的控制和同意模型：你可以管理数据，查看谁正在访问数据以及请求实体的特定属性。 这增强了 Microsoft Graph 模型，其授予或拒绝应用程序对整个实体的访问权限。

可以使用数据连接为组织启用机器学习方案。 在这些方案中，你可以创建应用程序来为利益干系人提供宝贵信息、训练机器学习模型，甚至根据采集的大量数据进行预测。

## <a name="get-started"></a>开始行动

在本教程中，你将创建第一个Microsoft Graph 数据连接应用程序。 很让人兴奋，对不对？ 我们也认为！ 若要开始，你首先需要设置一些内容。

### <a name="prerequisites"></a>先决条件

若要完成此实验，你将需要以下订阅或许可证。

1. **Microsoft 365租赁**

   - 如果没有，则通过注册 (开发人员计划) 一个免费Microsoft 365[应用程序](https://developer.microsoft.com/microsoft-365/dev-program)。
   - 多个Microsoft 365接收的电子邮件的用户。
   - 访问至少两个满足以下要求的帐户：
      - 必须分配 **有全局** 管理员角色。
      - 必须具有对 Microsoft 365 管理 中心的访问权限。

1. **Microsoft Azure 订阅**

   - 如果没有，可在 Azure 网站中 (一 [) 免费订阅](https://azure.microsoft.com/free/)。
   - 用于登录的帐户必须被授予全局管理员角色。 
   - Azure 订阅必须与 Microsoft 365 租户在同一租户中，因为 Graph Data 连接 将仅将数据导出到同一租户中的 Azure 订阅，而不是跨租户。
   - 你的Microsoft 365和 Azure 租户必须在同一Microsoft Azure Active Directory租户中。

1. 请确保你已安装[Visual Studio](https://visualstudio.microsoft.com/vs/)计算机上。

> [!NOTE]
> 此实验中使用的屏幕截图和示例来自一个Microsoft 365测试租户，该租户包含来自测试用户的示例电子邮件。 可以使用自己的租户Microsoft 365执行相同的步骤。 不会将数据写入Microsoft 365。 电子邮件数据的副本从 Microsoft 365 租户中的所有用户中提取，并复制到 Azure Blob 存储 帐户，你可以控制谁有权访问 Azure Blob 存储 内的数据。
