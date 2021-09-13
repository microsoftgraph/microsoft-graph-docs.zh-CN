---
ms.localizationpriority: medium
ms.openlocfilehash: 9a98117bc0021e1f51054f35f8de74f1aeed17f7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289523"
---
<!-- markdownlint-disable MD002 MD041 -->

在此步骤中，你将创建一Azure 存储帐户，Microsoft Graph 数据连接从数据库中提取的数据Microsoft 365进一步处理。

1. 打开浏览器并转到 Azure [门户](https://portal.azure.com/)。

1. 使用具有 Azure 和租户 **全局** 管理员权限Microsoft 365登录。

1. 在边栏导航上，选择 **"创建资源"。**

1. 查找 **"存储帐户**"资源类型，然后使用以下值创建它，然后选择"审阅 +**创建"。**

    - **订阅**：选择 Azure 订阅
    - **资源组**：GraphDataConnect (或选择现有资源组) 
    - **存储帐户名称**： mgdcm365datastore
    - **区域**：选取与你的客户区域Microsoft 365 Azure 区域
    - **性能**：标准
    - **冗余：** 地理位置冗余存储 (GRS) 
    - **高级选项卡**：
      - **访问层**：热

1. 查看设置与上一步中显示的设置匹配，然后选择"创建 **"。**

1. 创建Azure 存储帐户后，向 Azure AD 应用程序授予之前创建的正确访问权限。

    1. 选择Azure 存储 **帐户**。
    2. 在边栏菜单上，选择访问控制 **(IAM)**。
    3. 选择" **添加** 项目"块 **中的** 角色分配按钮。
    4. 使用以下值查找之前选择的应用程序，以授予其存储 **Blob 数据** 参与者角色，然后选择"保存 **"。**

        - **角色**：存储 Blob 数据参与者
        - **向：** 用户、组或服务主体分配访问权限
        - **选择**：Microsoft Graph 数据连接数据 (之前创建的 Azure AD 应用程序的名称) 

        ![Screenshot showing the proper 角色分配 to the application for Microsoft Graph 数据连接 in the Azure 存储 account in the Azure portal.](images/data-connect-azure-storage-role.png)

1. 在 **mgdcm365datastore** 帐户Azure 存储容器。

    1. 选择 **mgdcm365datastore Azure 存储** 帐户。
    2. 在边栏菜单上，选择 **"Blob** 服务"部分下的"容器"。
    3. 选择 **页面顶部的"+容器**"按钮，然后使用以下值，然后选择"创建 **"。**

        - **名称**：m365mails
        - **公共访问级别**：专用 (匿名访问) 

        ![Screenshot showing the creation of a new container called m365mails in the 存储 account blob containers in the Azure portal.](images/data-connect-azure-storage-container.png)
