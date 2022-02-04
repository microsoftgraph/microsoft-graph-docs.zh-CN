---
title: Microsoft Graph 数据连接策略和许可
description: 介绍支持的策略以及如何为组织分配 ISV 访问 SKU。
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
---

# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Microsoft Graph 数据连接策略和计费

Microsoft Graph 数据连接使用 [Azure 托管应用程序](/azure/managed-applications/overview)，允许你在 Azure 环境中创建和部署解决方案。 托管应用程序允许你支持某些 Azure 策略，让客户能够更加信心十足并舒适地使用你的应用程序。

## <a name="policies"></a>策略

对于使用 Microsoft 365 数据构建的 Azure 托管应用程序，支持使用以下 Azure 策略：

- [Azure 存储和 ADLS Gen 2 必需策略](/azure/storage/common/policy-reference)
- [ADLS Gen1 必需策略](/azure/data-lake-store/policy-reference)

> [!NOTE]
> Azure Data Lake Store Gen 1 和 Gen 2 使用不同的策略，因为 ADLS Gen 2 实施 Azure 存储。

在 Azure 应用市场发布过程中选择任何策略时，将为应用程序的所有安装检查并实施策略合规性状态。 在数据请求过程中，将向数据审批者显示合规的所有选定策略。 任何策略合规性违规行为将导致管道运行失败并停止数据提取。

## <a name="billing-for-microsoft-graph-data-connect"></a>Microsoft Graph 数据连接计费

账单将与你正在使用的 Azure 数据工厂的 Azure 订阅相关联。 此新计费模型的价格基于正在访问的 Microsoft Graph 对象的数量来确定。 有关计费的详细信息，请参阅[定价页面](https://azure.microsoft.com/pricing/details/graph-data-connect/)。

不会收费的目录对象包括：

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>另请参阅

- [Azure 存储策略](/azure/storage/common/policy-reference)
- [Microsoft Graph 数据连接计费](https://azure.microsoft.com/pricing/details/graph-data-connect/)
- [Azure 托管应用程序](/azure/managed-applications/overview)
- [用户选择和筛选](data-connect-filtering.md)
- [数据连接常见问题解答](data-connect-faq.md)
