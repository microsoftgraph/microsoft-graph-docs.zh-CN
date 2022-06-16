---
title: Microsoft Graph 中的用户
description: 使用 Microsoft Graph 访问与组织中的登录用户上下文相关的关系、文档、联系人和首选项。
author: dkershaw10
ms.localizationpriority: high
ms.prod: users
ms.custom: scenarios:getting-started
ms.openlocfilehash: 03a9e667a665363c4d36ca9c576c1472f66726fe
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095046"
---
# <a name="overview-of-users-in-microsoft-graph"></a>Microsoft Graph 中用户的概述

用户是 Microsoft Graph 中 Azure Active Directory (Azure AD) 工作或学校用户帐户或 Microsoft 帐户的表示形式。 Microsoft Graph 中的 **用户** 资源是一个中心，可以从这里访问与用户相关的关系和资源。

> [!VIDEO https://www.youtube-nocookie.com/embed/TUMPipN3UFI]

## <a name="develop-user-centric-applications"></a>开发以用户为中心的应用程序

你可使用 Microsoft Graph 访问与登录用户上下文相关的关系、文档、联系人和首选项。 **用户** 资源提供了无需执行其他调用即可访问和操作用户资源的简单方法，可查找特定的身份验证信息，并直接对其他 Microsoft Graph 资源发出查询。

若要访问用户的信息和数据，你需要[以用户身份进行访问](auth-v2-user.md)。 验证应用程序并获得[管理员同意](permissions-reference.md)，即可使用和更新与用户关联的更广泛的实体。

### <a name="manage-your-organization"></a>管理组织

在组织中创建新用户或更新现有用户的资源和关系。 可使用 Microsoft Graph 执行以下用户管理任务： 

- 创建或删除 Azure AD 组织中的用户。
- 列出用户的组成员资格并确定用户是否为组的成员。
- 列出向某用户报告的用户和向某用户分配经理。
- 上传或检索用户的照片。

### <a name="work-with-calendars-and-tasks"></a>使用日历和任务

可查看、查询和更新与某用户关联的用户日历和日历组，包括：

- 在用户日历上列出和创建事件。
- 查看分配给用户的任务。
- 为一组用户查找空闲的会议时间。
- 获取用户日历上设置的提醒列表。

### <a name="administer-mail-and-handle-contacts"></a>管理邮件和处理联系人

可配置用户邮件设置和联系人列表，并代表用户发送邮件，包括：

- 列出邮件消息和发送新邮件。
- 创建和列出用户联系人，并组织文件夹中的联系人。
- 检索并更新邮箱文件夹和设置。

### <a name="enrich-your-app-with-user-insights"></a>利用用户见解丰富应用

通过推广最近使用的文档或热门文档以及与用户关联的联系人，最大限度地提高应用程序的关联性。可以使用 Microsoft Graph 来：

- 返回用户最近查看和修改的文档。
- 返回有关用户活动的文档和网站。
- 列出通过电子邮件或 OneDrive for Business 与用户共享的文档。

## <a name="api-reference"></a>API 参考

在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的用户 API](/graph/api/resources/users?view=graph-rest-1.0&preserve-view=true)
- [Microsoft Graph beta 中的用户 API](/graph/api/resources/users?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>后续步骤

- 了解有关如何[使用用户](/graph/api/resources/users)的详细信息。
- 从 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)的 **用户** 资源中探索自己的数据。
- [代表用户](auth-v2-user.md)或[作为管理员同意的守护程序或服务](auth-v2-service.md)使用 Microsoft Graph 进行身份验证。
- 为使用 [Azure AD API](/graph/api/resources/azure-ad-overview) 的用户设置访问控制和策略。
- 审阅应用访问用户数据所需的[权限](permissions-reference.md)。
