---
title: Azure AD 访问评论-beta 更新
description: 您可以使用 Azure AD 访问评论来配置一次性或定期访问审核，以证明用户访问权限的证明。 本文档提供第二版 Api 的服务。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 44bdd534aeb36ad85133fe1ab26006150328e926
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000829"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审查

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>本文档包含适用于 Microsoft 365 组的 access 检查 Api 的最新受支持版本。 有关对其他资源的评论，请参阅 [access 审阅 api](accessreviews-root.md)。
>
>目前，Microsoft Graph Api 仅支持对组成员身份的访问权限审查。

您可以使用 [AZURE AD 访问评论](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) 来配置一次性或定期访问审核，以证明用户访问权限的证明。

组成员身份和应用程序访问的访问审核的典型客户方案包括：

- 客户可以通过对应用程序和组成员身份的访问权限审查来查看和验证来宾用户访问权限。 审阅者可以使用提供的见解来有效决定来宾是否应继续访问。

- 客户可以查看和验证员工对应用程序和组成员身份的访问权限，并进行访问审核。

- 客户可以将访问审核控件收集到与您的组织相关的程序中，以跟踪对合规性或风险敏感的应用程序的审查。

还有一种相关功能，客户可以查看和验证分配给 Azure AD 角色（如全局管理员或 Azure 订阅角色）的管理用户的角色分配。  此功能包含在 [AZURE AD 特权标识管理](privilegedidentitymanagement-root.md)中。

请注意，"访问审阅" 功能（包括 API）包含在 Azure AD Premium P2 中。  在其中创建访问审核的租户必须具有有效的已购买或试用版 Azure AD Premium P2 或 EMS E5 订阅。


## <a name="methods"></a>方法

下表列出了可用于与访问评审相关的资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[列出 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-list.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 集合 | 列出每个 `accessReviewScheduleDefinition` 。 不包括 `accessReviewInstance` 清单中的关联实例。 |
|[获取 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 获取 `accessReviewScheduleDefinition` 具有指定 id 的。 |
|[创建 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | 新建 `accessReviewScheduleDefinition`。 |
|[删除 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | 无。 | 删除 `accessReviewScheduleDefinition` 具有指定 ID 的。 |
|[更新 accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | 无。 | 使用指定的 ID 更新的属性 `accessReviewScheduleDefinition` 。 |
|[列出 accessReviewInstance](../api/accessreviewinstance-list.md) | [accessReviewInstance](accessreviewinstance.md) 集合 | 列出了每个 `accessReviewInstance` 特定的 `accessReviewScheduleDefinition` 。 不包括 `accessReviewInstanceDecisionItem` 清单中的关联的 s。 |
|[获取 accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | 返回 `accessReviewInstance` 的 `accessReviewScheduleDefinition` 。 不包括 `accessReviewInstanceDecisionItem` 对象中的关联 s。 |
|[列出 accessReviewInstances 待审批](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [accessReviewInstance](accessreviewinstance.md) 集合。 | 获取 `accessReviewInstance` 分配给呼叫用户的所有。 |
|[发送 accessReviewInstance 提醒](../api/accessreviewinstance-sendreminder.md) | 无。 | 将提醒发送给的审阅人 `accessReviewInstance` 。 |
|[停止 accessReviewInstance](../api/accessreviewinstance-stop.md) | 无。 | 手动停止 `accessReviewInstance` 。 |
|[接受建议](../api/accessreviewinstance-acceptrecommendations.md) | 无。 | 允许呼叫用户接受针对特定的审阅者的每个 NotReviewed 的决策建议 `accessReviewInstanceDecisionItem` `accessReviewInstance` 。 |
|[应用决策](../api/accessreviewinstance-applydecisions.md) | 无。 | 在上手动应用决定 `accessReviewInstance` 。 |
|[列出 accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合 | 列出了每个 `accessReviewInstanceDecisionItem` 特定的 `accessReviewInstance` 。 |
|[列出 accessReviewInstanceDecisionItems 待审批](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) 集合。 | 获取 `accessReviewInstanceDecisionItems` 特定用户的所有分配给呼叫用户的 `accessReviewInstance` 。 |
|[更新 accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | 无。 | 对于 `accessReviewInstanceDecisionItems` 呼叫用户分配有审阅者的任何人，呼叫用户可以通过修补决策对象来记录决策。 |

## <a name="role-and-application-permission-authorization-checks"></a>角色和应用程序权限授权检查

调用用户需要使用以下目录角色来管理访问评审。 请注意，目前仅通过 Microsoft Graph Api 支持对组进行的访问审阅。

| 操作 | 应用程序权限 | 呼叫用户的必需目录角色 |
|:------------------|:------------|:--------------------------------------------|
| 读取 | AccessReview 或 AccessReview。所有 | 全局管理员、全局读取器、安全管理员、安全读者或用户管理员 |
| 创建、更新或删除 | AccessReview.ReadWrite.All | 全局管理员或用户管理员 |

此外，为访问审核分配的审阅者的用户可以管理他们的决策，而无需在目录角色中进行管理。

## <a name="see-also"></a>另请参阅

- [管理员如何管理使用 Azure AD 访问评论的用户访问](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员如何管理使用 Azure AD 访问审查的来宾访问](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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


