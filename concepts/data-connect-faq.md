---
title: Microsoft Graph 数据连接常见问题解答
description: 获取可帮助你利用 Microsoft Graph 数据连接的相关提示。
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 7d8001c0517b38fdee910e609e76f5891e84ba03
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629685"
---
# <a name="microsoft-graph-data-connect-frequently-asked-questions"></a>Microsoft Graph 数据连接常见问题解答

借助 Microsoft Graph 数据连接，开发人员可为客户创建应用程序，用以提供对其大规模的 Microsoft Graph 数据集的受管访问。 本文提供了可帮助你利用数据连接功能的提示。 有关 Microsoft Graph 数据连接的简介，请参阅[概述](data-connect-concept-overview.md)文章。

## <a name="is-microsoft-graph-data-connect-right-for-me"></a>Microsoft Graph 数据连接是否适合我？

数据连接和 Microsoft Graph API 可以完全不同的方式访问相同的基础数据。 数据连接旨在批量提取大量数据，而 Microsoft Graph API 更适合于实时访问分散的数据集。 在某些情况下，将两者组合使用可能极具意义。 例如，可以使用数据连接来对去年的电子邮件数据进行初步提取，再使用 Microsoft Graph API 实时动态分析不断变化的电子邮件。 数据连接和 Microsoft Graph API 是针对不同工作的不同工具。 有必要思考哪种访问方法最适合你的场景。

## <a name="will-there-be-any-initial-overhead"></a>是否会有任何初始开销？

数据连接专用于批量提取大量数据，因此在提取数据之前可能会产生一些开销。 此开销大约为 45 分钟，这意味着无论数据量如何，所有管道至少都将花费这么长时间。 数据量庞大时，这一成本可忽略不计；但是如果你的场景无法承受这么长的时间，Microsoft Graph API 可提供更好的方法。

## <a name="how-much-do-i-have-to-pay-for-microsoft-graph-data-connect"></a>我需要为 Microsoft Graph 数据连接支付多少费用？

Microsoft Graph 数据连接消耗费用按月以“即付即用”方式计费。 Microsoft Graph 数据连接计费单位为 1000 个对象倍数，其，1 个对象映射到 Microsoft 365 中实体的 1 个单独实例。 例如，1 封电子邮件 =1 个对象，1 个文件 =1 个对象，1 条 Teams 聊天消息 = 1 个对象等等。 根据通过连接器提取的每 1,000 个对象计数，使用统一费率计算费用。 从以下数据集中提取对象无需支付任何费用：

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport。

迄今为止，Microsoft Graph 数据连接对象的价格是每提取的 1000 个对象 0.375 美元。

## <a name="is-it-possible-for-my-data-to-stay-within-the-organizations-subscription-with-microsoft-graph-data-connect"></a>使用 Microsoft Graph 数据连接，我的数据是否可保留在组织的订阅内？

数据连接管道由 Azure 数据工厂进行安排，后者是一项在 Azure 订阅中运行的数据集成服务。 Azure 订阅[与 Microsoft 365 租户一对一关联](/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)。 这样的话，数据一开始必须传输到关联的 Azure 订阅。 在进一步最小化和聚合后，数据可在其他位置使用。

如果想要构建供其他人用来提取其 Microsoft 365 数据的应用，可将应用打包为 [Azure 托管应用](/azure/managed-applications/overview)，再将其发布到 Azure 市场。 之后，其他人可在其自己的 Azure 订阅中部署你的应用，而该应用也能访问其租户中的数据。

## <a name="are-service-principals-required-with-microsoft-graph-data-connect"></a>使用 Microsoft Graph 数据连接时，是否要求使用服务主体？

创建数据工厂管道时，必须向 Microsoft 365 链接的服务提供服务主体。 在 Azure 中，服务主体是指代表应用程序/服务（与用户相反）的一个安全标识。 数据连接在获得授权可访问 Microsoft 365 数据时，会使用此服务主体作为其标识。

如果创建供其他人在其租户中使用的 Azure 托管应用程序，仍需为要使用的应用提供服务主体。 该服务主体将存在于你的（发布者的）租户中。 但是如果该应用需要其他服务主体，你的客户（安装者）将在其自己的租户中自行创建。 例如，数据工厂管道将可能需要访问 Azure 中的存储资源。 客户会创建服务主体，该主体有权存储帐户供管道使用。

## <a name="how-can-i-check-for-pending-privileged-access-management-requests"></a>如何检查待处理的 Privileged Access Management 请求？

Privileged Access Management (PAM) 请求必须得到管理员的批准，然后数据连接才可复制你的数据。 PAM 是 Microsoft 365 中向数据管道授予数据访问权限的机制。 首次触发管道时，它将等待 Microsoft 365 管理员（或指定的代理人）批准访问请求。 虽然管道状态显示“**正在进行中**”，但基础复制活动的状态将为 **ConsentPending**，直到获得批准，如以下屏幕截图所示。

![具有 ConsentPending 状态的管道运行状态窗格屏幕截图](images/data-connect-tips.png)

在开发期间，最好确保你的管道运行不一直处于 **ConsentPending** 状态，尤其是在更改管道之后。 例如，如果向架构额外添加了一个字段，则下一次管道运行将发出一个新的 PAM 请求，而该请求必须获得批准。 不要浪费时间等待一个需要你来批准的管道。

## <a name="how-can-i-approve-pam-requests-via-microsoft-365-admin-portal"></a>如何通过 Microsoft 365 管理门户审批 PAM 请求？

数据连接文档介绍了如何使用 PowerShell 和 PAM UX 来审批 PAM 请求。 要通过 PAM UX 进行审批，请访问 [Microsoft 365 管理门户](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/Settings/PrivilegedAccess)中的 PAM 界面。 该门户让你能够以简单、快捷的方式查看和审批/拒绝/撤消 PAM 请求。 可访问“**设置**” > “**服务和加载项**” > “**Microsoft Graph 数据连接**”，在 Microsoft Graph 数据连接加载项中查找指向它的链接。

## <a name="can-i-have-a-second-user-to-approve-pam-requests"></a>是否可让另一名用户审批 PAM 请求？

运行管道并触发 PAM 请求，该请求会附加到拥有该管道所用服务主体的用户帐户上。 但即使该帐户属于你设置的审批者组，你也不能用它来审批 PAM 请求，因为不允许自我审批。 如果尝试此操作，你将在 PAM 门户中获得一个错误消息：“请求者和审批者是同一人。 不允许自我审批。” 在开发时，你将必须在审批请求的管理员之外再拥有一个帐户。 提交者和审批者都必须具有有效的 Exchange Online 帐户。

## <a name="can-i-deduplicate-emails-when-needed"></a>能否在必要时删除重复的电子邮件？

从 `Message` 数据集中提取电子邮件时，通常同一封电子邮件有多个 JSON 对象。 这些重复项存在的原因是在向多名用户发送电子邮件时，每个收件人的邮箱中都有该电子邮件的副本。 由于数据集是从每个邮箱中提取的，因此它将包含所有用户的所有副本。 在某些情况下，可能有必要保留每个副本；但在其他情况下，可能必须删除重复项。
可根据邮件的 `internetMessageId` 删除导出的 JSON 对象中的重复项：具有相同 `internetMessageId` 的两封邮件是同一实例的重复副本。 由于重复项可存在于不同的 blob 中，因此必须删除所有 blob 中的重复项，而不是分别删除每个 blob 中的重复项。

## <a name="can-i-use-puser-field-to-determine-the-relevant-user"></a>能否使用 puser 字段来确定相关用户？

提取的数据包含一些在使用相应的 Microsoft Graph API 时不存在的属性。 具体而言，`puser` 在确定用户数据提取的位置时非常有用。 如果不同邮箱中具有同一电子邮件的两个副本，可使用 `puser` 字段来确定副本来自哪个邮箱。 `puser` 字段还对 `Manager` 数据集之类的数据集很有用。 导出的 JSON 将包含管理器相关信息，但只有当你知道它们是谁的管理器时，这才有用。 `puser` 字段将指出 JSON 对象对应于哪个管理器。

## <a name="is-a-mix-of-users-with-and-without-workplace-analytics-licenses-supported"></a>是否支持混合拥有和不拥有工作区分析许可证的用户？

如今，我们要求用户列表中的所有用户都拥有工作区分析许可证，或者用户列表中的所有用户都没有工作区分析许可证。 遗憾的是，我们不支持混合的用户列表，即有些用户拥有工作区分析许可证，而有些用户没有工作区分析许可证。 这是因为如果用户列表中的用户拥有工作区分析许可证，则数据连接不需要额外收费，而如果客户没有工作区分析许可证，则将使用此处详述的消耗计费向客户收费。 如果当前存在违反你的用例的情况，请告知我们，我们可在此查看是否有机会帮助解决这种情况。

## <a name="is-hybrid-mode-tenant-setup-supported"></a>是否支持混合模式租户设置？

如果你的 Microsoft 365 设置有一些用户在 Exchange Online 中，而一些用户在 Exchange 本地，则位于 Exchange 本地的用户将不受支持。 遗憾的是，当前对 Exchange 本地用户不支持数据连接。

## <a name="are-resource-accounts-supported"></a>是否支持资源帐户？

我们目前不支持从资源帐户访问邮件或事件。 我们将在未来添加对此功能的支持。

## <a name="i-am-seeing-multiple-files-per-adf-pipeline-run-but-sometimes-just-1-file-per-run-why-is-this-happening"></a>我看到每个 ADF 管道运行有多个文件，但有时每个运行只有 1 个文件。 这是什么原因？

Microsoft Graph 数据连接会获取每个管道运行的用户列表，然后跨并行运行的多个作业分发数据集提取和策展。 对于每个并行运行，都会在你定义的数据接收器中生成 1 个输出文件。 对于某些情况，如果用户列表较小，则可能会将其映射到 1 个提取和策展作业，在这些情况下，数据接收器中只会生成 1 个输出文件。

## <a name="how-is-billing-computed-with-the-count-of-objects-is-not-a-round-number"></a>如何使用对象计数而不是舍入数字计算计费？

出于计费目的，Microsoft Graph 数据连接会将提取的对象计数进位到最接近的 1000。 例如，如果你提取了 125 个对象或它们提取了 999 个对象，则将收取 1000 个对象的费用。 同样，如果你提取的对象数在 1001 到 2000 之间，则将收取 2000 个对象的费用。

## <a name="my-microsoft-365-copy-data-activity-is-always-failing-when-initialized-via-azure-synapse-why-is-this-happening"></a>通过 Azure Synapse 初始化时，Microsoft 365 复制数据活动始终失败。 这是什么原因？

目前，我们不支持通过 Azure Synapse 初始化 Microsoft 365 复制数据活动。 我们正在努力添加 Azure Synapse 初始化活动的集成，并将在完成此操作后更新我们的文档。
