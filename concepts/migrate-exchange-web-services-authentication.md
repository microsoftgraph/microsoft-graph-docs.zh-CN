---
title: Web 服务 Exchange EWS (和 Microsoft) 之间的身份验证Graph
description: 介绍身份验证详细信息，以帮助您将 Exchange Web 服务 (EWS) 迁移到 Microsoft Graph。
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 120efa7e2fc4c34b973831131d8fb2c435c2c432
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516551"
---
# <a name="authentication-differences-between-exchange-web-services-ews-and-microsoft-graph"></a>Web 服务 Exchange EWS (和 Microsoft) 之间的身份验证Graph

Exchange EWS (EWS) 和 Microsoft Graph都使用 [Microsoft 标识平台 OAuth 2.0](/azure/active-directory/develop/active-directory-v2-protocols) 进行身份验证和授权。

> [!NOTE]
> EWS 当前还支持基本身份验证。 [基本身份验证已弃用，](/lifecycle/announcements/exchange-online-basic-auth-deprecated)并且正在跨组织Microsoft 365停用。 Microsoft Graph不支持基本身份验证，因此尚未迁移到 OAuth 2.0 的应用必须这样做，以访问 Microsoft Graph。

## <a name="permissions"></a>权限

EWS 和 Microsoft Graph提供两种类型的权限：委派权限和应用程序权限。 委派权限在经过身份验证的用户上下文中。 应用程序权限授予不代表用户的应用程序。

使用 EWS，应用程序可以访问用户有权访问 (（如果为委派权限) ）或 EWS 可以使用应用程序权限 (访问) 的所有内容。

Microsoft Graph 为邮箱中的特定功能提供Exchange Online权限。 例如，可以允许应用程序仅读取邮件，并且无法访问日历或联系人。 委派身份验证的有效权限是用户的权限与应用程序已同意的权限的交集。 对于应用程序身份验证，有效权限是管理员同意的一组权限。

有关与 Microsoft Exchange权限Graph列表，请参阅：

- [邮件权限](permissions-reference.md#mail-permissions)
- [日历权限](permissions-reference.md#calendars-permissions)
- [个人联系人权限](permissions-reference.md#contacts-permissions)
- [任务权限](permissions-reference.md#tasks-permissions)

## <a name="impersonation"></a>模拟

[EWS 模拟](/exchange/client-developer/exchange-web-services/impersonation-and-ews-in-exchange) 为作为服务帐户运行的 EWS 应用程序提供了一种充当用户的机制。 这允许应用执行看似来自模拟用户的操作，例如发送电子邮件。

使用 Microsoft Graph，没有服务帐户。 相反，直接向应用程序授予权限。 应用程序使用具有其自己的 [标识的客户端](auth-v2-service.md) 凭据流进行身份验证。 默认情况下，管理员同意授予对所有用户邮箱的访问权限，但管理员可以将应用限制为 [特定](auth-limit-mailbox-access.md) 邮箱。
