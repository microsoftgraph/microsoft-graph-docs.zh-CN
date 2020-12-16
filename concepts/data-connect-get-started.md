---
title: Microsoft Graph 数据连接入门
description: 'Microsoft 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: f451da704c0fce255f37b61da7c7446145d8afd1
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897279"
---
# <a name="get-started-with-microsoft-graph-data-connect"></a>Microsoft Graph 数据连接入门

Microsoft 365 管理员必须先执行两个操作，以便管理员能够通过 Privileged Access Management (PAM) 控制数据移动，之后你才可以使用 Microsoft Graph 数据连接。 

1. 通过 Microsoft 365 管理门户的“服务和加载项”页同意选择使用 Microsoft Graph 数据连接。 这样即允许了对 Microsoft Azure 的数据移动请求（即保持对数据的完全控制，但允许 Azure 资源访问它）。 在提供对特定管道的批准前，无法迁移任何数据。
2. 在 Microsoft 365 订阅中设置已启用邮件的安全组或通讯组列表。 确保审批者组不为空。 仅此组中的用户可以批准数据移动请求。

## <a name="next-steps"></a>后续步骤

恭喜！ 现在你即可开始使用 Azure 工具生成智能应用程序。 可参阅 [Microsoft Graph 数据连接培训模块](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md)，来获取详细的分步说明。 要详细了解 Microsoft Graph 数据连接提供的功能，请参阅数据连接支持的[数据集、区域和接收器](data-connect-datasets.md)或[用户选择和筛选](data-connect-filtering.md)。
