---
title: Azure AD Graph 和 Microsoft Graph
description: 介绍 AZURE ACTIVE DIRECTORY (AZURE AD) GRAPH API 和 Microsoft Graph API (REST) 。
author: dkershaw10
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: a9b9bdd59441f804a6a7314db3a1ae0a44d4cba7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077612"
---
# <a name="method-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph 和 Microsoft Graph

本文是步骤 *1：查看迁移应用的* 过程的 API [差异的一部分](migrate-azure-ad-graph-planning-checklist.md)。

一些Azure Active Directory (Azure AD) Graph方法也发生了更改。  如果此方法未 **在此** 列表中显示，则它已在 [v1.0](/graph/api/overview)版本的 Microsoft Graph 中可用，其名称与 Azure AD Graph 中的名称完全相同。

|Azure AD Graph <br> (v1.6) 方法 |Microsoft Graph<br> (资源/方法) |备注|
|---|---|---|
| getAvailableExtensionProperties | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids) | |
| invalidateAllRefreshTokens | beta &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta&preserve-view=true) <br> v1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions) | |
| isMemberOf | beta &nbsp; - &nbsp; _未计划_ <br> v1.0 &nbsp; - &nbsp; _未计划_ | 请[改为使用 checkMemberGroups。](/graph/api/user-checkmembergroups) |
| restore | beta &nbsp; - &nbsp; [restore &nbsp; (applications， &nbsp; users， and groups &nbsp; &nbsp;) ](/graph/api/directory-deleteditems-restore?view=graph-rest-beta&preserve-view=true)<br> v1.0 &nbsp; - &nbsp; [还原 &nbsp; (&nbsp; 应用程序、用户 &nbsp; &nbsp; 和组) ](/graph/api/directory-deleteditems-restore) | 还可以查看已删除的应用程序、用户和组，并永久删除它们。 |

## <a name="next-steps"></a>后续步骤

- 了解如何检查[应用与](migrate-azure-ad-graph-audit-api-use.md)Microsoft graph 之间的 API Azure AD Graph差异。
- 再次查看 [检查](migrate-azure-ad-graph-planning-checklist.md) 表。
