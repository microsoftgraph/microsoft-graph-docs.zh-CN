---
title: Azure AD 访问审查
description: 使用Azure AD访问评审来配置一次性或定期访问评审，以证明用户对资源的访问权限Azure AD审核。
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 1e69482507020fb2902472fcbd7dcfa96639c343
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337178"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审查

命名空间：microsoft.graph

使用[Azure AD访问](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview)评审来配置一次性或定期访问评审，以证明用户访问Azure AD权限。 这些资源Azure AD组、服务主体、访问包和特权角色。

访问评审的典型客户方案包括：

- 客户可以通过组成员身份查看和认证来宾用户对组的访问权限。 审阅者可以使用提供的见解来有效决定是否应让来宾继续访问。
- 客户可以审阅并认证员工对Azure AD的访问权限。
- 客户可以审阅和审核分配Azure AD特权角色。 这支持组织管理特权访问。

访问评审功能（包括 API）仅在用户或 EMS E5 订阅的有效购买或试用Azure AD Premium P2可用。 有关许可证要求详细信息，请参阅 [访问评审许可证要求](/azure/active-directory/governance/access-reviews-overview#license-requirements)。

## <a name="methods"></a>Methods

下表列出了可用于与访问评审相关资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|**计划定义**| | |
|[列表定义](../api/accessreviewset-list-definitions.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|获取 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象及其属性的列表。|
|[创建定义](../api/accessreviewset-post-definitions.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|创建新的 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。|
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|读取 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的属性和关系。|
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|更新 [accessReviewScheduleDefinition 对象](../resources/accessreviewscheduledefinition.md) 的属性。|
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md)|无|删除 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。|
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|返回调用用户是任何实例的审阅者的所有定义。|
|**实例**| | |
|[列出实例](../api/accessreviewscheduledefinition-list-instances.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。|
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。|
|[stop](../api/accessreviewinstance-stop.md)|无|手动停止 accessReviewInstance。|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|无|向 accessReviewInstance 的审阅者发送提醒。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|无|将实例上的所有决策项重置为 `notReviewed`|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|无|手动对 accessReviewInstance 应用决策。|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|无| 允许调用用户接受他们作为特定 accessReviewInstance 审阅者的每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议。|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|无|在一次调用中查看主体或资源的批次。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回调用用户是审阅者的定义上的所有实例对象。|
|**实例决策项**| | |
|[列出决策](../api/accessreviewinstance-list-decisions.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|获取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象及其属性的列表。|
|[获取 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。|
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|更新 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。|
|[accessReviewInstanceDecisionItem：filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|返回调用用户是其审阅者的决策项。|
|**历史记录定义**| | |
|[列出 historyDefinitions](../api/accessreviewset-list-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 集合|获取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象及其属性的列表。|
|[创建 historyDefinitions](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|创建新的 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象。|
|[获取 accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|读取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象的属性和关系。|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|为可用于检索审阅历史记录数据的实例生成 URI。|
|[列出实例](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|检索 [accessReviewHistoryInstance](accessreviewhistoryinstance.md) 对象及其属性的列表。|

## <a name="role-and-application-permission-authorization-checks"></a>角色和应用程序权限授权检查

呼叫[Azure AD](/azure/active-directory/roles/permissions-reference)需要以下角色才能管理访问评审。

| 操作 | 应用程序权限 | 呼叫用户的必需目录角色 |
|:------------------|:------------|:--------------------------------------------|
| Read | AccessReview.Read.All 或 AccessReview.ReadWrite.All | 全局管理员、全局读取者、安全管理员、安全读者或用户管理员 |
| 创建、更新或删除 | AccessReview.ReadWrite.All | 全局管理员或用户管理员 |

此外，作为访问评审的分配审阅者的用户可以管理其决策，而无需担任目录角色。

## <a name="see-also"></a>另请参阅

- [了解如何](/graph/accessreviews-overview)使用访问评审 API 查看对访问Azure AD教程
- [管理员如何使用访问评审Azure AD用户访问](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员如何使用访问评审管理Azure AD访问](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)