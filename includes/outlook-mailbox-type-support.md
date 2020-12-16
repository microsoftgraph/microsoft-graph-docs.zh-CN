---
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.topic: include
ms.openlocfilehash: 94f5606f6bdf5382d35eab5864cb7ea76a1be702
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44894935"
---
<!-- markdownlint-disable MD041-->

Microsoft Graph API 支持访问用户 _主_ 邮箱和 [共享邮箱](https://support.office.com/article/open-and-use-a-shared-mailbox-in-outlook-d94a8e9e-21f1-4240-808b-de9c9c088afd)中的数据。 这些数据可以是日历、邮件或个人联系人，存储在 Exchange Online（作为 Microsoft 365 的一部分）云端的邮箱中或[混合部署](/graph/hybrid-rest-support)中的 Exchange 本地邮箱中。

此 API _不_ 支持访问就地存档邮箱（不在 [Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-archiving-service-description/archive-features#archive-mailbox) 和 [Exchange Server](https://docs.microsoft.com/Exchange/policy-and-compliance/in-place-archiving/in-place-archiving?view=exchserver-2019) 上）。