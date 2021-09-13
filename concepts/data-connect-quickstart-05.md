---
ms.localizationpriority: medium
ms.openlocfilehash: c36ed01a3d913a487864bfa2b77c13c707d0299f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289528"
---
<!-- markdownlint-disable MD002 MD041 -->

下一步是使用 Azure 数据工厂创建管道，以使用 Microsoft 365 将数据从 Azure 存储 帐户提取Microsoft Graph 数据连接。

## <a name="create-an-azure-data-factory-pipeline"></a>创建 Azure 数据工厂管道

1. 打开浏览器并转到 Azure [门户](https://portal.azure.com/)。

1. 使用具有 Azure 和租户 **全局** 管理员权限Microsoft 365登录。

1. 在边栏导航上，选择 **"创建资源"。**

1. 查找"**数据工厂**"资源类型，然后使用以下值创建它，然后选择"创建 **"。**

    1. **订阅**：选择 Azure 订阅
    2. **资源组**：GraphDataConnect
    3. **区域**：选取与你的客户区域Microsoft 365 Azure 区域
    4. **名称**：dfM365toBlobStorage
    5. **版本**： V2

        ![显示成功在 Azure 门户中新建 Azure 数据工厂服务的屏幕截图。](images/data-connect-adf-create.png)

    6. 在 **"Git 配置"** 选项卡中，确保配置 Git 或选择选项"_稍后配置 Git"。_

1. 创建 Azure 数据工厂资源后，选择"作者和 **监视器** "磁贴以启动 Azure 数据工厂全屏编辑器。

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。 用户单击"作者和监视器"按钮。](images/data-connect-adf-auth-and-mon.png)

1. 通过从左侧 **导航****中选择**"概述"，从"管理"体验切换到"管理"体验。

1. 默认情况下，Azure 数据工厂将使用自动解析区域集成运行时。 由于连接要求源和目标以及集成运行时存在于同一 Microsoft 365 区域，因此建议您创建一个包含固定区域的新集成运行时。

    1. 选择 **"集成运行时**  >  **""新建"。**
    2. 选择 **"Azure，自托管"，** 然后选择"继续 **"。**
    3. 选择 **"Azure** 用于网络环境"，然后选择"继续 **"。**

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。 用户正在为网络环境选择 Azure 选项。](images/data-connect-adf-network.png)

    4. 使用以下详细信息在最终屏幕上完成表单，然后选择"创建 **"。**

        - **名称**：集成运行时的名称
        - **说明**：输入说明
        - **区域**：选择与你的区域Microsoft 365区域
        - **虚拟网络配置 (预览) ：** 已禁用

1. 从左侧 **导航中选择** "管理 **"** 体验切换到"作者"体验。
1. 通过选择加号图标，然后通过管道 创建新 **管道**。

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。 用户正在创建新管道。](images/data-connect-adf-pipeline-create.png)

    - 将 **"复制数据"** 活动从 **"移动和转换"** 部分拖到设计图面上。

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。 用户将复制数据活动拖动到屏幕右侧编辑器中。](images/data-connect-adf-pipeline-copy-data.png)

    - 在设计器中选择活动。
    - 选择" **常规"** 选项卡，并指定其名称和说明。

      - **名称**：CopyFromM365toBlobStorage
      - **说明**：您需要的说明。

    - 在设计器下面的活动编辑器窗格中，选择"源 **"** 选项卡，然后选择"新建 **"。**
    - 找到数据集 **Office 365，** 选择它，然后选择"继续 **"** 按钮。

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。 用户选择 UI 中的Office 365数据集，然后选择"继续"按钮。](images/data-connect-adf-pipeline-dataset.png)

    - 设计器将 **更新"源**"选项卡，Microsoft 365连接器设置。
    - 选择" **源** 数据集"字段旁边的" **打开"** 选项。
    - 在表设置中，选择"连接 **"** 选项卡，然后选择" **新建"** 按钮。
    - 在出现的对话框中，分别在"服务主体 **ID"** 和"服务主体密钥"字段中输入之前创建的 Azure AD应用程序的应用程序 ID 和密码 **ID，** 然后选择"创建 **"。**
    - 通过"集成运行时"下拉列表选择 **之前在 连接中创建的集成** 运行时。

        ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。 用户使用服务主体密钥配置集成运行时。](images/data-connect-adf-linked-service.png)

    - 创建连接Microsoft 365，对于 **"表**"字段，选择"BasicDataSet_v0"。 **Message_v0**。
    - 从 **Office365Table** 切换到 **管道>源**。 对 Date 筛选器 **使用以下值**。

      - **列名称**：CreatedDateTime
      - **开始时间 (UTC) ：** 选择当前日期之前的某个时间
      - **UTC (结束) ：** 选择当前日期
      - 选择 **"输出列** "部分 _中的"导入架构_ "。

    - 选择管道 **选项卡中的** "复制数据活动"，然后选择" **接收"** 选项卡。

      - 选择"**新建"** 按钮，选择 **"Azure Blob 存储"，** 然后选择"继续 **"** 按钮。
      - 选择 **"** 二进制"作为数据的格式，然后选择"继续 **"** 按钮。
      - 为数据集指定名称 **M365JsonFile，** 如果尚未存在，则创建新的链接服务。

    - 在表中，选择"连接 **"** 选项卡，然后选择"新建 **"。**
    - 在对话框中设置以下值，然后选择"完成 **"。**

        - **身份验证方法**：服务主体
        - **Azure 订阅**：全选
        - **存储帐户名称**： mgdcm365datastore
          - 这是本练习前面创建的存储帐户。
        - **租户**：输入 Azure 租户的 ID
        - **服务主体 ID：** 输入之前创建的 Azure AD 应用程序的 ID
        - **服务主体密钥**：输入你之前创建的 Azure AD 应用程序的哈希密钥

    - 在"文件 **路径"字段旁边**，选择"浏览 **"。**
    - 选择之前创建的存储容器的名称。

      ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图。 用户在接收器属性中配置容器和文件路径。](images/data-connect-adf-sa-fp-config.png)

1. 创建管道后，选择设计器 **顶部的** "全部验证"按钮。

1. 在验证 (并修复在) 发现的所有问题后，选择设计器顶部的"全部发布"按钮。 

## <a name="run-the-azure-data-factory-pipeline"></a>运行 Azure 数据工厂管道

创建管道后，现在可以运行它了。

> [!NOTE]
> 可能需要几分钟时间才能显示同意请求，并且整个过程 (开始、请求同意以及批准完成管道运行) 后，需要 40 分钟以上的时间。

1. 在 Azure 数据工厂设计器中，打开管道后，选择"添加触发器 **>"现在触发"。**

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图，显示如何在管道中激活触发器。](images/data-connect-adf-run-trigger.png)

1. 启动作业后，从边栏菜单中选择"监视器"以查看当前正在运行的作业。

1. 在左侧导航栏上，找到" **管道运行** "选项卡并选择它。 选择管道 **名称列下的** 管道以查看活动 **运行**。 此管道将显示为 _"正在进行"。_

    ![Screenshot showing the Azure portal UI for Data Factory， it is showing the pipeline runs list.](images/data-connect-adf-pipeline-runs.png)

1. 进入"活动运行 **"** 视图后，转到位于页面底部的"活动运行"部分。

1. 将鼠标悬停在 **活动名称上方** ，然后选择切换选项。 此时将打开" **详细信息"** 选项卡。

    ![显示数据工厂活动运行的 Azure 门户 UI 的屏幕截图，用户选择活动名称中的 google 以打开详细信息选项卡。](images/data-connect-adf-pipeline-details.png)

1. 在 **"详细信息** "屏幕中，查找管道活动的状态，如下图所示。 在这种情况下，你可以看到它的状态为 **RequestingConsent**。

    ![显示数据工厂服务的 Azure 门户 UI 的屏幕截图，其中请求的加载状态设置为"RequestingConsent"。](images/data-connect-adf-wait-for-approval.png)

1. 此时，活动运行在内部暂停，直到有人通过管理员或 PowerShell Microsoft 365 管理中心同意请求。
