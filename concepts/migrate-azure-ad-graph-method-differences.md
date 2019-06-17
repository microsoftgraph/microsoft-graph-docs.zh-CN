---
title: Azure AD 和 Microsoft Graph 之间的方法差异
description: 介绍 Azure Active Directory (Azure AD) Graph API 和 Microsoft Graph API (REST) 之间的方法差异。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8ab5723c4fc25115f7c505099f19c847618f404
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990370"
---
# <a name="method-differences-between-azure-ad-and-microsoft-graph"></a>Azure AD 和 Microsoft Graph 之间的方法差异

本文是*第1步: 查看*[迁移应用程序](migrate-azure-ad-graph-planning-checklist.md)的 API 差异的过程的一部分。

许多 Azure AD Graph 方法也已更改。  如果未在此列表中显示方法, 则该方法在 Microsoft Graph 的 v1.0[版本](/graph/api/overview?view=graph-rest-1.0)中可用, 与 Azure AD Graph 中的名称完全相同。

|Azure AD Graph <br>(v. 1.6) 方法 |Microsoft Graph<br>(资源/方法)|Comments|
|---|---|---|
| addKey | beta 版-_尚不可用_ <br> v1.0-_尚不可用_ | 已计划, 但尚不可用。 | 
| addPassword | beta-addPassword <br> v1.0-_尚不可用_ | |
| getAvailableExtensionProperties | beta-_未计划_ <br> v1.0-_未计划_ | 当前未计划;可以根据需求进行再视。 |
| getObjectsByObjectId | &nbsp;-beta&nbsp;目录/getByIds <br> v1.0-directory/getByIds | |
| invalidateAllRefreshTokens | beta-revokeSignInSessions <br> v1.0-revokeSignInSessions | |
| isMemberOf | beta-_未计划_ <br> v1.0-_未计划_ | 请改用 checkMemberGroups。 |
| removeKey | beta 版-_尚不可用_ <br> v1.0-_尚不可用_ | 已计划, 但尚不可用。 | 
| removePassword | beta-removePassword <br> v1.0-_尚不可用_ | |
| restore | &nbsp;-beta&nbsp;还原&nbsp;(应用程序&nbsp;、用户&nbsp;和&nbsp;组)<br> &nbsp;-1.0&nbsp;版还原&nbsp;(用户&nbsp;和&nbsp;组) | 您还可以查看已删除的应用程序、用户和组, 并永久删除它们。 |

## <a name="next-steps"></a>后续步骤

- 了解如何在 Azure AD Graph 和 Microsoft Graph 之间检查您的应用程序中的[API 差异](migrate-azure-ad-graph-audit-api-use.md)。
- 浏览[Microsoft Graph](/graph/overview)概念和实践。
- 使用[Graph 浏览器](https://aka.ms/ge)试用 Microsoft Graph。
