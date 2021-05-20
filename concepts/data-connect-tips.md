---
title: Microsoft Graph 数据连接的相关使用提示
description: 获取可帮助你利用 Microsoft Graph 数据连接的相关提示。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: d9a87c629a80bc94c57e77bd0f2c0b1e7438c935
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547602"
---
# <a name="tips-for-using-microsoft-graph-data-connect"></a>Microsoft Graph 数据连接的相关使用提示

借助 Microsoft Graph 数据连接，开发人员可为客户创建应用程序，用以提供对其大规模的 Microsoft Graph 数据库的受管理的访问服务。 本文提供了可帮助你使用数据连接功能的提示。 有关 Microsoft Graph 数据连接的简介，请参阅[概述](data-connect-concept-overview.md)文章。

## <a name="is-microsoft-graph-data-connect-right-for-you"></a>Microsoft Graph 数据连接是否适合你？

数据连接和 Microsoft Graph API 可以完全不同的方式访问相同的基础数据。 数据连接旨在批量提取大量数据，而 Microsoft Graph API 更适合于实时访问分散的数据集。 在某些情况下，将两者组合使用可能极具意义。 例如，可以使用数据连接来对去年的电子邮件数据进行初步提取，再使用 Microsoft Graph API 实时动态分析不断变化地电子邮件。 数据连接和 Microsoft Graph API 是针对不同工作的不同工具。 有必要思考哪种访问方法最适合你的场景。

## <a name="expect-an-initial-overhead"></a>预估初始开销

数据连接专用于批量提取大量数据，因此在提取数据之前可能会产生一些开销。 此开销大约为 45 分钟，这意味着无论数据量如何，所有管道至少都将花费这么长时间。 数据量庞大时，这一成本可忽略不计；但是如果你的场景无法承受这么长的时间，Microsoft Graph API 可提供更好的方法。

## <a name="data-must-stay-within-the-organizations-subscription"></a>数据必须保留在组织的订阅中。

数据连接管道由 Azure 数据工厂进行安排，后者是一项在 Azure 订阅中运行的数据集成服务。 Azure 订阅[与 Microsoft 365 租户一对一关联](/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)。 这样的话，数据一开始必须传输到关联的 Azure 订阅。 在进一步最小化和聚合后，数据可在其他位置使用。

如果想要构建供其他人用来提取其 Microsoft 365 数据的应用，可将应用打包为 [Azure 托管应用](/azure/managed-applications/overview)，再将其发布到 Azure 市场。 之后，其他人可在其自己的 Azure 订阅中部署你的应用，而该应用也能访问其租户中的数据。 

## <a name="use-of-service-principals"></a>服务主体的使用

创建数据工厂管道时，必须向 Microsoft 365 链接的服务提供服务主体。 在 Azure 中，服务主体是指代表应用程序/服务（与用户相反）的一个安全标识。 数据连接在获得授权可访问 Microsoft 365 数据时，会使用此服务主体作为其标识。
如果创建供其他人在其租户中使用的 Azure 托管应用程序，仍需为要使用的应用提供服务主体。 该服务主体将存在于你的（发布者的）租户中。 但是如果该应用需要其他服务主体，你的客户（安装者）将在其自己的租户中自行创建。 例如，数据工厂管道将可能需要访问 Azure 中的存储资源。 客户会创建服务主体，该主体有权存储帐户供管道使用。

## <a name="check-for-pending-privileged-access-management-requests"></a>检查待处理的 Privileged Access Management 请求

Privileged Access Management (PAM) 请求必须得到管理员的批准，然后数据连接才可复制你的数据。 PAM 是 Microsoft 365 中向数据管道授予数据访问权限的机制。 首次触发管道时，它将等待 Microsoft 365 管理员（或指定的代理人）批准访问请求。 虽然管道状态显示“**正在进行中**”，但基础复制活动的状态将为 **ConsentPending**，直到获得批准，如以下屏幕截图所示。

![具有 ConsentPending 状态的管道运行状态窗格屏幕截图](images/data-connect-tips.png)

在开发期间，最好确保你的管道运行不一直处于 **ConsentPending** 状态，尤其是在更改管道之后。 例如，如果向架构额外添加了一个字段，则下一次管道运行将发出一个新的 PAM 请求，而该请求必须获得批准。 不要浪费时间等待一个需要你来批准的管道。

## <a name="approve-pam-requests-via-microsoft-365-admin-portal"></a>通过 Microsoft 365 管理门户审批 PAM 请求

数据连接文档介绍了如何使用 PowerShell 和 PAM UX 来审批 PAM 请求。 要通过 PAM UX 进行审批，请访问 [Microsoft 365 管理门户](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/Settings/PrivilegedAccess)中的 PAM 界面。 该门户让你能够以简单、快捷的方式查看和审批/拒绝/撤消 PAM 请求。 可访问“**设置**” > “**服务和加载项**” > “**Microsoft Graph 数据连接**”，在 Microsoft Graph 数据连接加载项中查找指向它的链接。

## <a name="use-a-second-user-to-approve-pam-requests"></a>使用另一名用户来审批 PAM 请求

运行管道并触发 PAM 请求，该请求会附加到拥有该管道所用服务主体的用户帐户上。 但即使该帐户属于你设置的审批者组，你也不能用它来审批 PAM 请求，因为不允许自我审批。 如果尝试此操作，你将在 PAM 门户中获得一个错误消息：“请求者和审批者是同一人。 不允许自我审批。” 在开发时，你将必须在审批请求的管理员之外再拥有一个帐户。 提交者和审批者都必须具有有效的 Exchange Online 帐户。

## <a name="deduplicate-emails-when-needed"></a>必要时删除重复的电子邮件

从 `Message` 数据集中提取电子邮件时，通常同一封电子邮件有多个 JSON 对象。 这些重复项存在的原因是在向多名用户发送电子邮件时，每个收件人的邮箱中都有该电子邮件的副本。 由于数据集是从每个邮箱中提取的，因此它将包含所有用户的所有副本。 在某些情况下，可能有必要保留每个副本；但在其他情况下，可能必须删除重复项。
可根据邮件的 `internetMessageId` 删除导出的 JSON 对象中的重复项：具有相同 `internetMessageId` 的两封邮件是同一实例的重复副本。 由于重复项可存在于不同的 blob 中，因此必须删除所有 blob 中的重复项，而不是分别删除每个 blob 中的重复项。

## <a name="use-puser-field-to-determine-the-relevant-user"></a>使用 puser 字段来确定相关用户

提取的数据包含一些在使用相应的 Microsoft Graph API 时不存在的属性。 具体而言，`puser` 在确定用户数据提取的位置时非常有用。 如果不同邮箱中具有同一电子邮件的两个副本，可使用 `puser` 字段来确定副本来自哪个邮箱。
`puser` 字段还对 `Manager` 数据集之类的数据集很有用。 导出的 JSON 将包含管理器相关信息，但只有当你知道它们是谁的管理器时，这才有用。 `puser` 字段将指出 JSON 对象对应于哪个管理器。

## <a name="next-steps"></a>后续步骤

联系 [Microsoft 365 开发人员平台意见论坛](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph)提交功能请求。