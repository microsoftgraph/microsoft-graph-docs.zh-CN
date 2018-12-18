---
title: Microsoft Graph 数据连接（预览）入门
description: 'Office 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。 '
author: ajacks-msft
ms.openlocfilehash: 1cd8d5734b0fd8b48df8a49fe0a833583c21148d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312080"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a>Microsoft Graph 数据连接（预览）入门

Office 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。 

1. 通过 Microsoft 365 管理门户的“服务和加载项”页同意选择使用 Microsoft Graph 数据连接。**** 这样即允许了对 Microsoft Azure 的数据移动请求（即保持对数据的完全控制，但允许 Azure 资源访问它）。 在提供对特定管道的批准前，无法迁移任何数据。
2. 在 Office 365 订阅中设置审批者组。 确保审批者组不为空。 仅此组中的用户可以批准数据移动请求。

可参阅 [Microsoft Graph 数据连接培训模块](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)，来获取详细的分步说明。

## <a name="next-steps"></a>后续步骤

恭喜！ 现在你即可开始使用 Azure 工具生成智能应用程序。 可参阅 [Microsoft Graph 数据连接 GitHub 存储库](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki)来获取示例应用程序和更多文档。 
