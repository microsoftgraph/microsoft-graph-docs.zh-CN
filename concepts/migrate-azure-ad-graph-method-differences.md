---
title: Azure AD 和 Microsoft Graph 之间的方法差异
description: 介绍 Azure Active Directory (Azure AD) Graph API 和 Microsoft Graph API (REST) 之间的方法差异。
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 577167a306c98ba51c1ba13d9240570df202f083
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46872913"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph 之间的方法差异

本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

许多 Azure AD Graph 方法也已更改。  如果 **未** 在此列表中显示方法，则该方法在 Microsoft Graph 的 v1.0 [版本](/graph/api/overview?view=graph-rest-1.0) 中可用，与 Azure AD Graph 中的名称完全相同。

|Azure AD Graph <br> (1.6) 方法 |Microsoft Graph<br> (资源/方法) |备注|
|---|---|---|
| getAvailableExtensionProperties | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; [directoryObjects/getAvailableExtensionProperties](/graph/api/directoryobject-getavailableextensionproperties?view=graph-rest-1.0) |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> v1.0 1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | beta &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| isMemberOf | &nbsp; - &nbsp; _未计划_beta <br> 1.0 版 &nbsp; - &nbsp; _未计划_ | 请改用 [checkMemberGroups](/graph/api/user-checkmembergroups?view=graph-rest-1.0) 。 |
| restore | &nbsp; - &nbsp; [ &nbsp; (应用程序、 &nbsp; 用户 &nbsp; 和 &nbsp; 组) ](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)的 beta 还原<br> &nbsp; - &nbsp; [ &nbsp; (应用程序、 &nbsp; 用户 &nbsp; 和 &nbsp; 组](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0)的1.0 版还原)  | 您还可以查看已删除的应用程序、用户和组，并永久删除它们。 |

## <a name="next-steps"></a>后续步骤

- 了解如何在 Azure AD Graph 和 Microsoft Graph 之间检查您的应用程序中的 [API 差异](migrate-azure-ad-graph-audit-api-use.md) 。
- 再次查看 [检查表](migrate-azure-ad-graph-planning-checklist.md) 。
