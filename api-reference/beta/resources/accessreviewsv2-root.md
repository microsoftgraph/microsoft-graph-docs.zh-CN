---
title: Azure AD 访问审查
description: 可以使用 Azure AD 访问评审来配置一次性或定期访问评审，以证明用户的访问权限。 本文档提供第 2 版 API。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: facc1cd9f51d9e638b01fa0bcf5efce5f846e727
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579716"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审查

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


可以使用 [Azure AD 访问评审](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) 来配置一次性或定期访问评审，以证明用户的访问权限。

访问组成员身份和应用程序访问评审的典型客户方案包括：

- 客户可以通过使用访问评审来查看和认证来宾用户访问权，访问应用程序和组成员身份。 审阅者可以使用提供的见解来有效决定是否应让来宾继续访问。

- 客户可以通过访问评审查看并认证员工对应用程序和组成员身份的访问权限。

- 客户可以将访问控制收集到与组织相关的程序中，以跟踪合规性或风险敏感型应用程序的相关审查。

客户还可以查看和认证分配给 Azure AD 角色（如全局管理员或 Azure 订阅角色）的管理用户的角色分配的相关功能。  此功能包含在 Azure [AD](privilegedidentitymanagement-root.md)Privileged Identity Management 中。

请注意，访问评审功能（包括 API）包含在 Azure AD 高级版 P2 中。  创建访问评审的租户必须拥有有效的已购买或试用 Azure AD 高级版 P2 或 EMS E5 订阅。


## <a name="methods"></a>方法

下表列出了可用于与访问评审相关资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 `accessReviewScheduleDefinition` 。 不在一览 `accessReviewInstance` 中包括关联的实例。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取 `accessReviewScheduleDefinition` 具有指定 ID 的 。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 新建 `accessReviewScheduleDefinition`。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除 `accessReviewScheduleDefinition` 具有指定 ID 的 。 |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 更新具有指定 `accessReviewScheduleDefinition` ID 的属性。 |
|[列出 accessReviewInstance](../api/accessreviewinstance-list.md) | [accessReviewInstance](accessreviewinstance.md) 集合 | 列出 `accessReviewInstance` 每个特定 `accessReviewScheduleDefinition` 。 不在一览 `accessReviewInstanceDecisionItem` 中包括关联的 。 |
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | 返回 `accessReviewInstance` `accessReviewScheduleDefinition` 。 对象中不包括关联的 `accessReviewInstanceDecisionItem` 。 |
|[列出 accessReviewInstances 待审批](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance](accessreviewinstance.md) 集合。 | 获取 `accessReviewInstance` 分配给呼叫用户的所有资源。 |
|[发送 accessReviewInstance 提醒](../api/accessreviewinstance-sendreminder.md) | 无。 | 向 的审阅者发送提醒 `accessReviewInstance` 。 |
|[停止访问ReviewInstance](../api/accessreviewinstance-stop.md) | 无。 | 手动停止 `accessReviewInstance` 。 |
|[接受建议](../api/accessreviewinstance-acceptrecommendations.md) | 无。 | 允许调用用户接受针对每个 NotReviewed 的决策建议，即他们是 `accessReviewInstanceDecisionItem` 特定 的审阅者 `accessReviewInstance` 。 |
|[应用决策](../api/accessreviewinstance-applydecisions.md) | 无。 | 手动对 应用决策 `accessReviewInstance` 。 |
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 列出 `accessReviewInstanceDecisionItem` 每个特定 `accessReviewInstance` 。 |
|[列出 accessReviewInstanceDecisionItems 待审批](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取 `accessReviewInstanceDecisionItems` 分配给特定 呼叫用户的所有 `accessReviewInstance` 。 |
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于为呼叫用户分配审阅者的任何用户，调用用户可以通过 `accessReviewInstanceDecisionItems` 修补决策对象来记录决策。 |

## <a name="role-and-application-permission-authorization-checks"></a>角色和应用程序权限授权检查

呼叫用户需要以下目录角色才能管理访问评审。 

| Operation | 应用程序权限 | 呼叫用户的必需目录角色 |
|:------------------|:------------|:--------------------------------------------|
| 阅读 | AccessReview.Read.All 或 AccessReview.ReadWrite.All | 全局管理员、全局读取者、安全管理员、安全读者或用户管理员 |
| 创建、更新或删除 | AccessReview.ReadWrite.All | 全局管理员或用户管理员 |

此外，作为访问评审的分配审阅者的用户可以管理其决策，而无需担任目录角色。

## <a name="see-also"></a>另请参阅

- [管理员如何使用 Azure AD 访问评审管理用户访问](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员如何使用 Azure AD 访问评审管理来宾访问](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


