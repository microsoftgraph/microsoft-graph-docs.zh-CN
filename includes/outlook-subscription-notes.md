---
author: angelgolfer-ms
ms.localizationpriority: high
ms.prod: outlook
ms.topic: include
ms.openlocfilehash: f790fd4357bfe63ad364fff30a7de0c69d94dfe0
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337893"
---
<!-- markdownlint-disable MD041-->
创建和管理（获取、更新和删除）订阅需要资源的读取范围。 例如，若要获取有关邮件的更改通知，应用需要 Mail.Read 权限。 Outlook 更改通知支持委派和应用程序权限范围。 请注意以下限制：

- 委托的权限仅支持订阅已登录用户的邮箱内文件夹中的项。 例如，不能使用委托的权限 Calendars.Read 来订阅另一个用户邮箱中的事件。
- 订阅 _共享或委托_ 文件夹中 Outlook 联系人、事件或邮件的更改通知：

  - 使用相应的应用程序权限订阅租户内 _任何_ 用户的文件夹或邮箱中项目的更改。
  - 切勿使用 Outlook 共享权限（Contacts.Read.Shared、Calendars.Read.Shared、Mail.Read.Shared 及其相应的读写权限），因为它们 **不** 支持订阅对共享或委托文件夹中的项的更改通知。