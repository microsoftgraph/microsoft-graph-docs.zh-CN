---
title: Access 审阅 API 概述
description: 使用访问评审 API 以编程方式查看对 Azure AD 资源的访问权限，以确保正确的标识有权访问正确的资源。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 929eaeaf259b3f6f8db163ba7cec1a99fad17e7b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437077"
---
# <a name="overview-of-the-access-reviews-api"></a>Access 审阅 API 概述

[Azure Active Directory (Azure AD) 访问评审](/azure/active-directory/governance/access-reviews-overview) 是 Azure AD 标识治理的一项功能，有助于确保正确的标识 (或主体) 有权访问组织中正确的资源。 此评审可以使用 Microsoft Graph 中 [的访问评审 API](/graph/api/resources/accessreviewsv2-overview) 以编程方式实现。

## <a name="participants-in-an-access-review"></a>访问评审中的参与者

访问评审是关于证明或重新认证主体对资源的持续访问。 主体可以是单个用户、组或应用程序。  

可以查看其访问权限的资源包括组、特权角色 (包括 Azure AD 角色和 Azure 资源角色) 、访问包和应用程序。

访问评审中的审阅者或证明者可能包括以下用户或用户组：

+ 用户 (来宾用户或成员) 查看自己的访问权限，并证明他们需要继续访问。
+ 另一个用户，例如，安全管理员角色中的管理员，查看其他主体的访问权限。
+ 用户的经理证明其直接报告需要持续访问。
+ 组的成员。
+ 组所有者，包括可能符合特定条件的所有者。
+ 应用程序所有者。

## <a name="building-blocks-of-the-access-review-api"></a>访问评审 API 的构建基块

访问评审 API 是逻辑结构化的，由以下构建基块组成。  

### <a name="1-access-reviews-schedule-definition"></a>1. 访问评审计划定义

这是包含访问评审及其实例设置的逻辑蓝图。 这些设置包括：

+ 正在访问的资源。
+ 访问资源的主体。
+ 证明主体需要保持对资源的访问权限的审阅者。
+ 访问评审的频率。
+ 多阶段访问评审) 的访问评审 (阶段。
+ 如果未记录决策，则应用的默认决策。

### <a name="2-access-review-instance"></a>2. 访问评审实例

表示审阅者针对其做出决策的单个评审活动或事件。 访问评审定义可能具有多个实例，如定期评审中的情况一样。 一次性评审只有一个实例。 对于多阶段访问评审，每个实例最多包含三个阶段。

### <a name="3-decision-item-recorded-for-a-review"></a>3. 记录供审阅的决策项

表示审阅者对实例做出的决定，包括时间戳和决策理由。 每个评审实例的决策数与正在审查的主体数相同。 如果没有做出任何决定，即审阅者尚未对评审作出答复，则实例将没有决策对象。

可以为每个决策项提供系统生成的建议决策。 这些基于正在审查其访问权限的主体的最后一个登录日期。 此功能使审阅者能够查看组织中处于休眠状态的帐户，并建议对主体的持续访问应用决策。

访问评审还支持审核对每个访问评审实例所做的决策，也可以下载用于脱机审核的决定。

## <a name="scope-of-calling-the-access-reviews-api"></a>调用访问评审 API 的范围

访问评审 API 支持 [委派](/graph/auth-v2-user) 和 [应用程序](/graph/auth-v2-service) 上下文。

在委托 (用户) 上下文中，应用程序代表用户调用访问评审 API。 典型方案包括：

+ 管理员使用脚本创建、读取或更新访问评审。
+ 资源所有者使用应用或脚本为其拥有的资源创建访问评审。
+ 管理员会自动收集一个或多个访问评审的所有决策。

在应用程序上下文中，应用程序在没有登录用户的情况下调用访问评审 API。 典型的方案是定期收集所有访问评审决策的计划后台脚本。

## <a name="next-steps"></a>后续步骤 

+ [使用访问评审 API](/graph/api/resources/accessreviewsv2-overview)
+ [详细了解 Azure AD 访问评审](/azure/active-directory/governance/access-reviews-overview)
+ 请尝试以下教程来管理访问评审：
    + [使用访问评审 API 查看对安全组的访问权限](tutorial-accessreviews-securitygroup.md)
    + [使用访问评审 API 查看对 Microsoft 365 组的来宾访问权限](tutorial-accessreviews-M365group.md)