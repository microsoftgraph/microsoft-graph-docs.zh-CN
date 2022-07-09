---
title: Azure AD 访问审查
description: 可以使用 Azure AD 访问评审来配置一次性或定期访问评审，以证明用户的访问权限。 本文档提供第二版本的 API。
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 24dd74c3baa54807a78ce338504be89a31043b77
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697143"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审查

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

使用 [Azure AD 访问评审](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) 配置一次性或定期访问评审，以证明用户访问 Azure AD 资源的权限。 这些 Azure AD 资源包括组、服务主体、访问包和特权角色。

访问评审的典型客户方案包括：

- 客户可以通过组成员身份查看和认证来宾用户对组的访问权限。 审阅者可以使用提供的见解来有效地确定来宾是否应继续访问。
- 客户可以查看和认证员工对 Azure AD 资源的访问权限。
- 客户可以查看和审核 Azure AD 特权角色的分配。 这支持组织管理特权访问。

请注意，访问评审功能（包括 API）包含在Azure AD Premium P2中。  创建访问评审的租户必须具有有效的购买或试用Azure AD Premium P2或 EMS E5 订阅。 有关许可证要求的详细信息，请 [参阅 Access 评审许可证要求](/azure/active-directory/governance/access-reviews-overview#license-requirements)。

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]

## <a name="methods"></a>方法

下表列出了可用于与访问评审相关的资源交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|**计划定义**| | |
|[列表定义](../api/accessreviewset-list-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 获取 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象及其属性的列表。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取 accessReviewScheduleDefinition 对象及其属性。 |
|[创建定义](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 创建新的 accessReviewScheduleDefinition。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除 accessReviewScheduleDefinition。 |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定的标识符更新 accessReviewScheduleDefinition 的属性。 |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|检索调用用户是一个或多个实例的审阅者的所有定义。|
|**实例**| | |
|[列出实例](../api/accessreviewscheduledefinition-list-instances.md) | [accessReviewInstance](accessreviewinstance.md) 集合 | 获取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象及其属性的列表。 |
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | 读取 [accessReviewInstance](../resources/accessreviewinstance.md) 对象的属性和关系。 |
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | 无。 | 向 accessReviewInstance 的审阅者发送提醒。 |
|[stop](../api/accessreviewinstance-stop.md) | 无。 | 手动停止 accessReviewInstance。 |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | 无。 | 允许调用用户接受针对每个 NotReviewed accessReviewInstanceDecisionItem 的决策建议，即他们是特定 accessReviewInstance 的审阅者。 |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | 无。 | 在 accessReviewInstance 上手动应用决策。 |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|无|在一次调用中查看主体或资源的批处理。|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|无|将实例上的所有决策项重置为 `notReviewed`。|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[accessReviewInstance](../resources/accessreviewinstance.md) 集合|返回给定 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 上的所有实例，调用用户是一个或多个决策的审阅者。|
|**实例决策项**| | |
|[列出决策](../api/accessreviewinstance-list-decisions.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 获取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象及其属性的列表。|
|[获取 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。|
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于向调用用户分配审阅者的任何 accessReviewInstanceDecisionItems，调用用户可以通过修补决策对象来记录决策。 |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合|检索所有 [accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) 对象，其中调用使用是给定 [accessReviewInstance](accessreviewinstance.md) 的审阅者。|
|[listPendingApproval](../api/accessreviewinstancedecisionitem-listpendingapproval.md) (已弃用)  | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取分配给调用用户的所有 accessReviewInstanceDecisionItems，以获取特定 accessReviewInstance。 此方法已被弃用，并替换为 [accessReviewInstanceDecisionItem：filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)。 |
|**历史记录定义**| | |
|[列出 historyDefinitions](../api/accessreviewset-list-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 集合|获取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象及其属性的列表。|
|[创建 historyDefinitions](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|创建新的 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象。|
|[获取 accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|读取 [accessReviewHistoryDefinition](accessreviewhistorydefinition.md) 对象的属性和关系。|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|为可用于检索审阅历史记录数据的实例生成 URI。|
|[列出实例](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|检索 [accessReviewHistoryInstance](accessreviewhistoryinstance.md) 对象及其属性的列表。|
|**策略**| | |
|[获取 accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|读取 [accessReviewPolicy](../resources/accessreviewpolicy.md) 对象的属性和关系。|
|[更新 accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|更新 [accessReviewPolicy 对象的](../resources/accessreviewpolicy.md) 属性。|
|[列出待批准的定义](../api/accessreviewscheduledefinition-filterbycurrentuser.md) (已弃用) |[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 集合|检索调用用户是一个或多个实例的审阅者的所有定义。 此方法已被弃用并替换为 [accessReviewScheduleDefinition：filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)。|
|[列出挂起的AccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) (已弃用)  | [accessReviewInstance](accessreviewinstance.md) 集合。 | 获取分配给调用用户的所有挂起的 accessReviewInstance 资源。 此方法已被弃用并替换为 [accessReviewInstance：filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)。 |

## <a name="role-and-application-permission-authorization-checks"></a>角色和应用程序权限授权检查

调用用户需要以下 [Azure AD 角色](/azure/active-directory/roles/permissions-reference) 来管理访问评审。

| 操作 | 应用程序权限 | 调用用户所需的目录角色 |
|:------------------|:------------|:--------------------------------------------|
| 读取 | AccessReview.Read.All 或 AccessReview.ReadWrite.All | 全局管理员、全局读取者、安全管理员、安全读取者或用户管理员 |
| 创建、更新或删除 | AccessReview.ReadWrite.All | 全局管理员或用户管理员 |

此外，作为访问评审的分配审阅者用户可以管理其决策，而无需担任目录角色。

## <a name="see-also"></a>另请参阅

- [教程](/graph/accessreviews-overview) ，了解如何使用访问评审 API 来评审对 Azure AD 资源的访问权限
- [管理员如何使用 Azure AD 访问评审管理用户访问权限](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
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

