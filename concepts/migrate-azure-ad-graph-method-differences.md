---
title: Azure AD 和 Microsoft Graph 之间的方法差异
description: 介绍 Azure Active Directory （Azure AD） Graph API 和 Microsoft Graph API （REST）之间的方法差异。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 00649e4f55a8bfcfd5354d2a75793447e3686109
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38656527"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph 之间的方法差异

本文是*第1步：查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

许多 Azure AD Graph 方法也已更改。  如果**未**在此列表中显示方法，则该方法在 Microsoft Graph 的 v1.0[版本](/graph/api/overview?view=graph-rest-1.0)中可用，与 Azure AD Graph 中的名称完全相同。

|Azure AD Graph <br>（v. 1.6）方法 |Microsoft Graph<br>（资源/方法）|备注|
|---|---|---|
| getAvailableExtensionProperties | beta 版-_不可用_ <br> v1.0-不可_用_ |  |
| getObjectsByObjectId | &nbsp;-beta&nbsp;目录/getByIds <br> v1.0-directory/getByIds | |
| invalidateAllRefreshTokens | beta-revokeSignInSessions <br> v1.0-revokeSignInSessions | |
| isMemberOf | beta-_未计划_ <br> v1.0-_未计划_ | 请改用 checkMemberGroups。 |
| restore | &nbsp;-beta&nbsp;还原&nbsp;（应用程序&nbsp;、用户&nbsp;和&nbsp;组）<br> &nbsp;-1.0&nbsp;版还原&nbsp;（用户&nbsp;和&nbsp;组） | 您还可以查看已删除的应用程序、用户和组，并永久删除它们。 |

## <a name="next-steps"></a>后续步骤

- 了解如何在 Azure AD Graph 和 Microsoft Graph 之间检查您的应用程序中的[API 差异](migrate-azure-ad-graph-audit-api-use.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
