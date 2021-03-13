---
title: Azure AD 和 Microsoft Graph 的方法差异
description: 介绍 Azure Active Directory (Azure AD) Graph API 和 Microsoft Graph API (REST) 。
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 95acfccc83fee798d5b06d78bbf10f02c128a640
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760670"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph 的方法差异

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

一些 Azure AD Graph 方法也发生了更改。  如果方法 **未在此** 列表中显示，则它在 [v1.0](/graph/api/overview?view=graph-rest-1.0) 版本的 Microsoft Graph 中已经可用，其名称与 Azure AD Graph 中的名称完全相同。

|Azure AD Graph <br> (v1.6) 方法 |Microsoft Graph<br> (资源/方法) |Comments|
|---|---|---|
| getAvailableExtensionProperties | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | beta &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| isMemberOf | beta &nbsp; - &nbsp; _未计划_ <br> v1.0 &nbsp; - &nbsp; _未计划_ | 请[改为使用 checkMemberGroups。](/graph/api/user-checkmembergroups?view=graph-rest-1.0) |
| restore | beta &nbsp; - &nbsp; [restore &nbsp; (applications， &nbsp; users， &nbsp; and groups &nbsp;) ](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> v1.0 &nbsp; - &nbsp; [还原 &nbsp; (应用程序 &nbsp; 、用户 &nbsp; &nbsp; 和组) ](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | 还可以查看已删除的应用程序、用户和组，并永久删除它们。 |

## <a name="next-steps"></a>后续步骤

- 了解如何检查 [Azure](migrate-azure-ad-graph-audit-api-use.md) AD Graph 和 Microsoft Graph 之间的应用中的 API 差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。
