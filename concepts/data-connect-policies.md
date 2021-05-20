---
title: Microsoft Graph 数据连接策略和许可
description: 介绍支持的策略以及如何为组织分配 ISV 访问 SKU。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: c9529c500ff2e086a3a1185a56b9db397f0ace49
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547616"
---
# <a name="microsoft-graph-data-connect-policies-and-licensing"></a>Microsoft Graph 数据连接策略和许可

Microsoft Graph 数据连接使用 [Azure 托管应用程序](/azure/managed-applications/overview)，允许你在客户的 Azure 环境中创建和部署解决方案。 托管应用程序允许你支持某些 Azure 策略，让客户能够更加信心十足并舒适地使用你的应用程序。 此外，你必须为安装你的应用程序的一个或多个组织向 Microsoft 购买和申请许可证，以便允许应用程序通过数据连接访问数据。

## <a name="policies"></a>策略

对于使用 Microsoft 365 数据构建的 Azure 托管应用程序，支持使用以下 Azure 策略：

- [ADLS Gen1 加密必需策略](/azure/azure-policy/scripts/enforce-datalakestore-encryption)

在 Azure 应用市场发布过程中选择任何策略时，将为应用程序的所有安装检查并实施策略合规性状态。 在数据请求过程中，将向数据审批者显示合规的所有选定策略。 任何策略合规性违规行为将导致管道运行失败并停止数据提取。

如果想要请求为其他策略提供支持，请在 [Microsoft 365 开发人员平台创意论坛](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)上告知我们。

## <a name="licensing"></a>许可

作为 Workplace Analytics 许可的一部分，Microsoft Graph 数据连接当前已可用。该许可证每月按用户提供。 具有 Workplace Analytics 的组织可以通过授予和管理对其数据的大规模访问来扩展对 Microsoft 365数据的见解。 若要了解详细信息，包括如何购买，请访问 [Workplace Analytics 产品页面](https://products.office.com/business/workplace-analytics)。

自 2021 年 2 月 1 日 起，Microsoft Graph 数据连接将为所有客户过渡至 Azure Billing。 账单将与你正在使用的 Azure 数据工厂的 Azure 订阅相关联。 此新计费模型的价格基于正在访问的 Microsoft Graph 对象的数量来确定。

虽然此新计费功能仍为预览版本，但价格已确定为每 1,000 个 Microsoft Graph 对象 $0.375。 例如，如果访问对象总计 10,000 个，你将收到 $3.75 的 Azure 账单。 预览期结束时，费用将改为每 1,000 个 Microsoft Graph 对象 $0.75。 上述费率将适用于 Exchange 邮件和 Teams 聊天对象，其中包括：BasicDataSet_v0.Contact、 BasicDataSet_v0.Event、 BasicDataSet_v0.Message、 BasicDataSet_v0.SentItem、 BasicDataSet_v0.MailFolder 和 BasicDataSet_v0.CalendarView。

目录对象的对象将不会收费，其中包括：BasicDataSet_v0.User、 BasicDataSet_v0.MailboxSettings、BasicDataSet_v0.Manager 和 BasicDataSet_v0.DirectReport。

## <a name="next-steps"></a>后续步骤
如果想要请求为其他策略或数据集提供支持，请在 [Microsoft 365 开发人员平台创意论坛](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)上告知我们。 若要详细了解 Workplace Analytics，包括如何购买，请访问 [Workplace Analytics 产品页面](https://products.office.com/business/workplace-analytics)。