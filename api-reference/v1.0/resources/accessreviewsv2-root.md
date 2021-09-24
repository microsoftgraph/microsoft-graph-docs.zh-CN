---
title: Azure AD 访问审查
description: 使用 Azure AD 访问评审配置一次性或定期访问评审，以证明用户对 Azure AD 资源的访问权限。
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 2d1b72b557c5825b72cbf827609933bdc97edcfa
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59507429"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审查

命名空间：microsoft.graph

使用 [Azure AD 访问评审](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) 配置一次性或定期访问评审，以证明用户访问 Azure AD 资源的权利。 这些 Azure AD 资源包括组、服务主体、访问包和特权角色。

访问评审的典型客户方案包括：

- 客户可以通过组成员身份查看和认证来宾用户对组的访问权限。 审阅者可以使用提供的见解来有效决定是否应让来宾继续访问。
- 客户可以审阅并认证员工对 Azure AD 资源的访问权限。
- 客户可以审阅和审核对 Azure AD 特权角色的分配。 这支持组织管理特权访问。

访问评审功能（包括 API）仅在用户或 EMS E5 订阅的有效购买或试用Azure AD Premium P2可用。

## <a name="methods"></a>Methods

下表列出了可用于与访问评审相关资源进行交互的方法。

| 方法           | 返回类型    |Description|
|:---------------|:--------|:----------|
|**计划定义**| | |
|[列出 accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|获取 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象及其属性的列表。|
|[创建 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|创建新的 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。|
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|读取 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的属性和关系。|
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|更新 [accessReviewScheduleDefinition 对象](../resources/accessreviewscheduledefinition.md) 的属性。|
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md)|无|删除 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。|
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|返回调用用户是任何实例的审阅者的所有定义。|
|**实例**| | |
|[列出 accessReviewInstances](../api/accessreviewinstance-list.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。|
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。|
|[stop](../api/accessreviewinstance-stop.md)|无|手动停止 accessReviewInstance。|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|无|向 accessReviewInstance 的审阅者发送提醒。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|无|将实例上的所有决策项重置为 `notReviewed`|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|无|手动对 accessReviewInstance 应用决策。|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|无| 允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|无|在一次调用中查看主体或资源的批次。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回调用用户是审阅者的定义上的所有实例对象。|
|**实例决策项**| | |
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|获取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象及其属性的列表。|
|[获取 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。|
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|更新 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。|
|[accessReviewInstanceDecisionItem：filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|返回调用用户是其审阅者的决策项。|


## <a name="role-and-application-permission-authorization-checks"></a>角色和应用程序权限授权检查

以下 [Azure AD](/azure/active-directory/roles/permissions-reference) 角色是呼叫用户管理访问评审所需的。

| 操作 | 应用程序权限 | 呼叫用户的必需目录角色 |
|:------------------|:------------|:--------------------------------------------|
| 读取 | AccessReview.Read.All 或 AccessReview.ReadWrite.All | 全局管理员、全局读取者、安全管理员、安全读者或用户管理员 |
| 创建、更新或删除 | AccessReview.ReadWrite.All | 全局管理员或用户管理员 |

此外，作为访问评审的分配审阅者的用户可以管理其决策，而无需担任目录角色。

## <a name="see-also"></a>另请参阅

- [了解如何](/graph/accessreviews-overview) 使用访问评审 API 查看对 Azure AD 资源的访问权限的教程
- [管理员如何使用 Azure AD 访问评审管理用户访问](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员如何使用 Azure AD 访问评审管理来宾访问](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)