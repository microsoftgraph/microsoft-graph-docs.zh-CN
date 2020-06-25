---
title: Azure AD 和 Microsoft Graph 之间的方法差异
description: 介绍 Azure Active Directory （Azure AD） Graph API 和 Microsoft Graph API （REST）之间的方法差异。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8179dcc797086e26d4351d17d7a5675b5d012722
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863717"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph 之间的方法差异

本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

许多 Azure AD Graph 方法也已更改。  如果**未**在此列表中显示方法，则该方法在 Microsoft Graph 的 v1.0[版本](/graph/api/overview?view=graph-rest-1.0)中可用，与 Azure AD Graph 中的名称完全相同。

|Azure AD Graph <br>（v. 1.6）方法 |Microsoft Graph<br>（资源/方法）|备注|
|---|---|---|
| getAvailableExtensionProperties | beta &nbsp; - &nbsp; _不可用_ <br> v1.0 1.0 &nbsp; - &nbsp; _不可用_ |  |
| getObjectsByObjectId | beta &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-beta) <br> v1.0 1.0 &nbsp; - &nbsp; [directoryObjects/getByIds](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) | |
| invalidateAllRefreshTokens | beta &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [revokeSignInSessions](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) | |
| isMemberOf | &nbsp; - &nbsp; _未计划_beta <br> 1.0 版 &nbsp; - &nbsp; _未计划_ | 请改用 checkMemberGroups。 |
| restore | beta &nbsp; - &nbsp; [还原 &nbsp; （应用程序、 &nbsp; 用户 &nbsp; 和 &nbsp; 组）](/graph/api/directory-deleteditems-restore?view=graph-rest-beta)<br> 1.0 版 &nbsp; - &nbsp; [还原 &nbsp; （应用程序、 &nbsp; 用户 &nbsp; 和 &nbsp; 组）](/graph/api/directory-deleteditems-restore?view=graph-rest-1.0) | 您还可以查看已删除的应用程序、用户和组，并永久删除它们。 |

## <a name="next-steps"></a>后续步骤

- 了解如何在 Azure AD Graph 和 Microsoft Graph 之间检查您的应用程序中的[API 差异](migrate-azure-ad-graph-audit-api-use.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
