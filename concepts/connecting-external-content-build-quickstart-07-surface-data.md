---
ms.localizationpriority: medium
ms.openlocfilehash: 04ba810183228e3834069d9bfa620fe3c71fdb12
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59289514"
---
<!-- markdownlint-disable MD002 MD025 MD041 -->

创建垂直搜索和结果类型以自定义 必应 中的 Microsoft SharePoint、Microsoft Office 和 Microsoft 搜索 中的搜索结果，以便用户更轻松地找到他们有权查看的信息。

## <a name="create-a-vertical"></a>创建垂直

若要在组织级别创建和启用垂直搜索，请Microsoft 365 管理中心全局管理员角色并执行以下操作[](https://admin.microsoft.com/)：

1. 转到 **"设置**  >  **搜索&**  >  **自定义"。**
2. 转到 **"垂直** "，然后单击" **添加"** 按钮。
3. 提供以下详细信息：
  * **将垂直名称：** 设备部件。

   !["命名垂直"部分屏幕截图](images/connectors-images/build11.png)

  * **内容源**：使用应用创建的连接器。  (部件清单) 

   !["内容源"部分屏幕截图](images/connectors-images/build12.png)

  * **添加查询：** 保留为空。

   !["添加查询"部分屏幕截图](images/connectors-images/build13.png)

  * **筛选器**：保留为空。

   !["筛选器"部分屏幕截图](images/connectors-images/build14.png)

## <a name="create-a-result-type"></a>创建结果类型

创建结果类型：

1. 转到 **"设置**  >  **搜索&**  >  **自定义"。**
2. 转到结果 **类型选项卡，** 然后单击"添加 **"** 按钮。
3. 提供以下详细信息：

  * **名称**：设备部件

   !["命名结果类型"部分屏幕截图](images/connectors-images/build15.png)

  * **内容源**：在应用中创建的连接器。

   !["选择内容源"部分屏幕截图](images/connectors-images/build16.png)

  * **规则**：无

   !["设置规则"部分屏幕截图](images/connectors-images/build17.png)

  * 将 [ 上result-type.js内容](https://github.com/microsoftgraph/msgraph-search-connector-sample/blob/master/result-type.json) 粘贴到布局设计器文本框中。

   !["设计布局"部分屏幕截图](images/connectors-images/build18.png)
