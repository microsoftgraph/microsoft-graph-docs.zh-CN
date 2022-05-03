---
title: Microsoft Graph 数据连接策略和计费
description: 介绍支持哪些策略以及数据连接计费模型。
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 83c285d94a060f5e66c76e27ab041a04c4da8d7a
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176584"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Microsoft Graph 数据连接策略和计费

Microsoft Graph 数据连接使用 [Azure 托管应用程序](/azure/managed-applications/overview)，允许你在 Azure 环境中创建和部署解决方案。 托管应用程序允许你支持某些 Azure 策略，让客户能够更加信心十足并舒适地使用你的应用程序。

## <a name="policies"></a>策略

对于使用 Microsoft 365 数据构建的 Azure 托管应用程序，支持使用以下 Azure 策略：

- [Azure Policy Azure 存储的内置定义](/azure/storage/common/policy-reference)
- [Azure Data Lake Storage Gen2](/azure/storage/blobs/data-lake-storage-introduction) 简介
- [Azure Policy Azure Data Lake Storage Gen1 的内置定义](/azure/data-lake-store/policy-reference)

> [!NOTE]
> Azure Data Lake Storage Gen1 和 Gen2 使用不同的策略，因为 Azure Data Lake Storage Gen2 实现 Azure 存储。

在 Azure 应用市场发布过程中选择任何策略时，将为应用程序的所有安装检查并实施策略合规性状态。 在数据请求过程中，将向数据审批者显示合规的所有选定策略。 任何策略合规性违规行为将导致管道运行失败并停止数据提取。

## <a name="billing"></a>计费

账单将与你正在使用的 Azure 数据工厂的 Azure 订阅相关联。 此新计费模型的价格基于正在访问的 Microsoft Graph 对象的数量来确定。 有关计费的详细信息，请参阅[定价页面](https://azure.microsoft.com/pricing/details/graph-data-connect/)。

不收费的目录对象如下所示：

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>另请参阅

- [用户选择和筛选](data-connect-filtering.md)
- [数据连接常见问题解答](data-connect-faq.md)
