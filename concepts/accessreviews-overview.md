---
title: 访问评审 API 概述
description: 访问评审 API 允许你以编程方式查看对 Azure AD 资源的访问权限。
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: b22fcf84e8303f10ad6d9f0f30cf0e508db5f103aee8430c35fb9981bcaec8c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154852"
---
# <a name="overview-of-the-access-reviews-api"></a>Access 审阅 API 概述

Microsoft[访问评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) Graph允许你以编程方式查看对 Azure AD 资源的访问权限。 这包括：
+ 创建、读取、更新和删除访问评审、访问评审设置和计划。
+ 调查过去的访问评审和审阅者做出的决策，包括 Azure AD 自动执行的步骤。

## <a name="scope-of-use"></a>使用范围

访问评审 API 既支持委托上下文又支持应用程序上下文。 在委派 (上下文中) ，应用程序代表用户调用访问评审 API。 典型方案包括：
+ 使用脚本创建、读取或更新访问评审的管理员。
+ 使用应用或脚本为自己拥有的资源创建访问评审的资源所有者。
+ 管理员会自动收集一个或多个访问评审的所有决策。
  
若要在用户环境中授权 (委派) ，请参阅代表 [用户获取访问权限](/graph/auth-v2-user)。

在应用程序上下文中，应用程序在没有登录用户的情况下调用访问评审 API。 典型方案是安排的后台脚本定期收集所有访问评审的决策。 若要在此上下文中授权你的应用，请参阅 [在没有用户的情况下获取访问权限](/graph/auth-v2-service)。

## <a name="building-blocks-of-an-access-review"></a>访问评审的构建基块

访问评审按逻辑进行构建，并包含以下构建基块：
+ **访问评审计划定义** - 包含访问评审及其实例设置的逻辑蓝图。 这些设置包括用于查看访问权限的资源，以及证明访问这些资源的审阅者。
+ **访问评审实例** - 表示审阅者依据做出决策的单个审阅活动。 访问评审定义可以具有多个实例，就像定期审阅中一样。 一次评审只有一个实例。
+ **记录用于审阅的决策项** - 表示审阅者对实例做出的决定，包括时间戳和决策理由。 每个审阅实例具有与所审阅用户数一样多的决策。 如果没有做出任何决策，即审阅者尚未对审阅做出响应，则实例将没有决策对象。

## <a name="next-steps"></a>后续步骤

请尝试以下教程来管理访问评审：

+ [使用组的访问评审 API 查看对安全组的访问权限](tutorial-accessreviews-securitygroup.md)
+ [使用组的访问评审 API 查看对具有来宾用户的所有Microsoft 365组的访问权限](tutorial-accessreviews-M365group.md)

## <a name="see-also"></a>另请参阅

+ [规划Azure Active Directory访问评审部署](/azure/active-directory/governance/deploy-access-reviews)
+ [创建对应用程序应用程序的组&评审](/azure/active-directory/governance/create-access-review)
+ [代表用户获取访问权限](/graph/auth-v2-user)
+ [不代表用户获取访问权限](/graph/auth-v2-service)
