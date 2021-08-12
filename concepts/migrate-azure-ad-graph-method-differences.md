---
title: Azure AD 和 Microsoft Graph
description: 介绍 Azure AD Azure Active Directory (API 和 Microsoft) Graph API Graph REST (方法) 。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: a8ab3022b55d8d6117157ca216e4a1bc9f6d461da02b8b44a2cea39d5ebd6b9e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54163533"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

一些 Azure AD Graph方法也发生了更改。  如果方法未 **在此** 列表中显示，则它已在 [v1.0](/graph/api/overview?view=graph-rest-1.0)版本的 Microsoft Graph 中可用，其名称与 Azure AD Graph。

|Azure AD Graph <br> (v1.6) 方法 |Microsoft Graph<br> (资源/方法) |备注|
|---|---|---|
| getAvailableExtensionProperties | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | beta &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| isMemberOf | beta &nbsp; - &nbsp; _未计划_ <br> v1.0 &nbsp; - &nbsp; _未计划_ | 请[改为使用 checkMemberGroups。](/graph/api/user-checkmembergroups?view=graph-rest-1.0) |
| restore | beta &nbsp; - &nbsp; [restore &nbsp; (applications， &nbsp; users， &nbsp; and groups &nbsp;) ](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> v1.0 &nbsp; - &nbsp; [还原 &nbsp; (应用程序 &nbsp; 、用户 &nbsp; &nbsp; 和组) ](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | 还可以查看已删除的应用程序、用户和组，并永久删除它们。 |

## <a name="next-steps"></a>后续步骤

- 了解如何检查[Azure](migrate-azure-ad-graph-audit-api-use.md) AD Graph 和 Microsoft graph 之间的应用中的 API 差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。
