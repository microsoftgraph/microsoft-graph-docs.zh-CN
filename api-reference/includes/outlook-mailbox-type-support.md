---
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.topic: include
ms.openlocfilehash: 93e1ebadf88a319b164e58b0a909d3d596dcd69a9de10f56bd4c549ddf771922
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230465"
---
<!-- markdownlint-disable MD041-->

Microsoft Graph API 支持访问用户 _主_ 邮箱和 [共享邮箱](https://support.office.com/article/open-and-use-a-shared-mailbox-in-outlook-d94a8e9e-21f1-4240-808b-de9c9c088afd)中的数据。 这些数据可以是日历、邮件或个人联系人，存储在 Exchange Online（作为 Microsoft 365 的一部分）云端的邮箱中或[混合部署](/graph/hybrid-rest-support)中的 Exchange 本地邮箱中。

此 API _不_ 支持访问就地存档邮箱（不在 [Exchange Online](/office365/servicedescriptions/exchange-online-archiving-service-description/archive-features#archive-mailbox) 和 [Exchange Server](/Exchange/policy-and-compliance/in-place-archiving/in-place-archiving?view=exchserver-2019) 上）。