---
title: Exchange Web 服务 (EWS) 与 Microsoft Graph 之间的身份验证差异
description: 介绍身份验证详细信息，以帮助你将 Exchange Web 服务 (EWS) 应用迁移到 Microsoft Graph。
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: be933068b459aabeb0d2a7aca083b0745fa3c97a
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549615"
---
# <a name="authentication-differences-between-exchange-web-services-ews-and-microsoft-graph"></a>Exchange Web 服务 (EWS) 与 Microsoft Graph 之间的身份验证差异

Exchange Web 服务 (EWS) 和 Microsoft Graph都使用 [Microsoft 标识平台 OAuth 2.0](/azure/active-directory/develop/active-directory-v2-protocols) 进行身份验证和授权。

> [!NOTE]
> EWS 目前还支持基本身份验证。 [基本身份验证已弃](/lifecycle/announcements/exchange-online-basic-auth-deprecated)用，并且正在跨Microsoft 365组织停用。 Microsoft Graph不支持基本身份验证，因此尚未迁移到 OAuth 2.0 的应用必须这样做才能访问 Microsoft Graph。

## <a name="permissions"></a>权限

EWS 和 Microsoft Graph提供两种类型的权限：委派和应用程序。 委派的权限位于经过身份验证的用户的上下文中。 向不代表用户操作的应用程序授予应用程序权限。

对于 EWS，应用程序有权访问用户有权访问 (的所有内容（如果) 委派权限或 EWS 可以使用应用程序权限) 访问 (的所有内容。 

EWS 具有全部或全无访问模型，并且没有用于限制邮箱中数据访问的粒度范围。 而 Microsoft Graph为Exchange Online邮箱中的特定功能提供精细的权限。 例如，可以允许应用程序只读取邮件，并且无法访问日历或联系人。 委派身份验证的有效权限是用户权限与已为应用程序许可的权限的交集。 对于应用程序身份验证，有效权限是管理员同意的权限集。

有关Exchange相关的 Microsoft Graph 权限的完整列表，请参阅：

- [邮件权限](permissions-reference.md#mail-permissions)
- [日历权限](permissions-reference.md#calendars-permissions)
- [个人联系人权限](permissions-reference.md#contacts-permissions)
- [任务权限](permissions-reference.md#tasks-permissions)

## <a name="impersonation"></a>模拟

[EWS 模拟](/exchange/client-developer/exchange-web-services/impersonation-and-ews-in-exchange) 为作为服务帐户运行以充当用户的 EWS 应用程序提供了一种机制。 这允许应用执行看似来自模拟用户的操作，例如发送电子邮件。

使用 Microsoft Graph，没有服务帐户。 而是直接向应用程序授予权限。 应用程序使用 [客户端凭据流](auth-v2-service.md) 及其自己的标识进行身份验证。 默认情况下，管理员同意授予对所有用户邮箱的访问权限，但管理员可以 [将应用限制为特定邮箱](auth-limit-mailbox-access.md) 。 在 Microsoft Graph中实现模拟的方法是使用应用访问策略和应用程序权限。
