---
title: 访问评审 API 概述
description: 访问评审 API 允许你以编程方式查看对Azure AD的访问权限。 这有助于确保正确的标识具有对组织中正确资源的访问权限。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: e09914b7e52f3be2961d3a55dd308262442eb1b1
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335897"
---
# <a name="overview-of-the-access-reviews-api"></a>Access 审阅 API 概述

[Azure Active Directory (Azure AD) ](/azure/active-directory/governance/access-reviews-overview)访问评审是 Azure AD Identity Governance 的一项功能，它有助于确保 (或主体) 对组织中适当的资源具有适当的访问权限。 此评价可以使用 Microsoft Graph 中的访问评审 [API](/graph/api/resources/accessreviewsv2-overview) 以编程Graph。

## <a name="participants-in-an-access-review"></a>访问评审的参与者

访问评审用于证明或重新验证主体对资源的连续访问。 主体可以是单个用户、组或应用程序。  

可审阅其访问权限的资源包括组、特权角色 (包括 Azure AD 角色和 Azure 资源) 、访问包和应用程序。

访问评审中的审阅者或证明人可能包括以下用户或用户组：

+ 用户 (来宾用户或成员) 查看自己的访问权限并证明其需要持续访问。
+ 另一个用户（例如，安全管理员角色中的管理员）查看其他主体的访问权限。
+ 用户的经理证明其直接下属需要持续访问。
+ 组的成员。
+ 组所有者，包括可能满足特定条件的所有者。
+ 应用程序所有者。

## <a name="building-blocks-of-the-access-review-api"></a>访问评审 API 的构建基块

访问评审 API 在逻辑上构造，由以下构建基块组成。  

### <a name="1-access-reviews-schedule-definition"></a>1. 访问评审计划定义

这是包含访问评审及其实例设置的逻辑蓝图。 这些设置包括：

+ 要访问的资源。
+ 访问资源的主体。
+ 证明主体需要维护对资源的访问权限的审阅者。
+ 访问评审的频率。
+ 访问评审阶段 (多阶段访问评审) 。
+ 未记录决策时要应用的默认决策。

### <a name="2-access-review-instance"></a>2. 访问评审实例

代表审阅者依据做出决策的单个审阅活动或事件。 访问评审定义可以具有多个实例，就像定期审阅中一样。 一次评审只有一个实例。 对于多阶段访问评审，每个实例最多包含三个阶段。

### <a name="3-decision-item-recorded-for-a-review"></a>3. 记录用于审阅的决策项

表示审阅者对实例做出的决定，包括时间戳和决策的理由。 每个审阅实例具有与所审阅的主体数量一样多的决策。 如果没有做出任何决策，即审阅者尚未对审阅做出响应，则实例将没有决策对象。

可以针对每个决策项提供系统生成的推荐决策。 这些基于正在审查其访问权限的主体的上一次登录日期。 此功能使审阅者能够查看组织中休眠的帐户，并推荐有关主体继续访问的决策。

访问评审还支持审核在每个访问评审实例上做出的决策，这些决策也可以下载用于脱机审核。

## <a name="scope-of-calling-the-access-reviews-api"></a>调用访问评审 API 的范围

访问评审 API 既支持[委托上下文又支持](/graph/auth-v2-user)[应用程序](/graph/auth-v2-service)上下文。

在委派 (用户) 上下文中，应用程序代表用户调用访问评审 API。 典型方案包括：

+ 管理员使用脚本来创建、读取或更新访问评审。
+ 资源所有者使用应用或脚本来创建他们拥有的资源的访问评审。
+ 管理员会自动收集一个或多个访问评审的所有决策。

在应用程序上下文中，应用程序在没有登录用户的情况下调用访问评审 API。 典型方案是安排的后台脚本定期收集所有访问评审的决策。

## <a name="next-steps"></a>后续步骤 

+ [使用访问评审 API](/graph/api/resources/accessreviewsv2-overview)
+ [阅读有关Azure AD评论](/azure/active-directory/governance/access-reviews-overview)
+ 请尝试以下教程来管理访问评审：
    + [使用访问评审 API 查看对安全组的访问权限](tutorial-accessreviews-securitygroup.md)
    + [使用访问评审 API 查看来宾对组Microsoft 365访问](tutorial-accessreviews-M365group.md)