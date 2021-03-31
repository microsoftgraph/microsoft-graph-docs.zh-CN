---
title: Azure AD 访问评审 - 旧版
description: 可以使用 Azure AD 访问评审来配置一次性或定期访问评审，以证明用户的访问权限。 本文档提供旧版 API。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 498769a0ea3362186b4991bcc6f18ef2bcd532f4
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469342"
---
# <a name="azure-ad-access-reviews-for-resources-excluding-groups"></a>Azure AD 访问评审 (组和组除外) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

可以使用 [Azure AD 访问评审](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) 来配置一次性或定期访问评审，以证明用户的访问权限。

访问组成员身份和应用程序访问评审的典型客户方案包括：

- 客户可以通过使用访问评审来查看和认证来宾用户访问权，访问应用程序和组成员身份。 审阅者可以使用提供的见解来有效决定是否应让来宾继续访问。

- 客户可以通过访问评审查看并认证员工对应用程序和组成员身份的访问权限。

- 客户可以将访问控制收集到与组织相关的程序中，以跟踪合规性或风险敏感型应用程序的相关审查。

客户还可以查看和认证分配给 Azure AD 角色（如全局管理员或 Azure 订阅角色）的管理用户的角色分配的相关功能。  此功能包含在 Azure [AD Privileged Identity Management 中](privilegedidentitymanagement-root.md)。

请注意，访问评审功能（包括 API）包含在 Azure AD Premium P2 中。  创建访问评审的租户必须拥有有效的已购买或试用 Azure AD Premium P2 或 EMS E5 订阅。
在创建访问评审、计划或程序控制之前，管理员必须事先已载入才能准备 [programControlType](programcontroltype.md) 和 [businessFlowTemplate](businessflowtemplate.md) 资源。 组织可以载入 Azure AD 访问评审，或者，对于 Azure AD 角色或 Azure 订阅角色的访问评审，为 Azure AD PIM。


## <a name="methods"></a>方法

下表列出了可用于与访问评审相关资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取具有特定 ID 的访问评审。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新的 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[列出 accessReviews](../api/accessreview-list.md) |    [accessReview](accessreview.md) 集合 |    列出 businessFlowTemplate 的 accessReviews。 |
|[列出 accessReview 审阅者](../api/accessreview-listreviewers.md) |      [userIdentity](useridentity.md) 集合| 获取 accessReview 的审阅者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   将审阅者添加到 accessReview。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   从 accessReview 中删除审阅者。 |
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) 集合| 获取 accessReview 的决策。|
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) 集合| 作为审阅者，获取我在 accessReview 上的决定。|
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) |        无。   |   向 accessReview 的审阅者发送提醒。 |
|[Stop accessReview](../api/accessreview-stop.md) |     无。   |   停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) |     无。   |   重置进行中的 accessReview 中的决策。|
|[应用 accessReview 决策](../api/accessreview-apply.md) |     无。   |   从已完成的 accessReview 应用决策。|
|[列出 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md) 集合| 获取适用于访问评论的业务流程模板。|
|[创建程序](../api/program-create.md) |   [程序](program.md)   |   创建新程序。|
|[删除程序](../api/program-delete.md) |   无。   |   删除程序。|
|[列出程序](../api/program-list.md) |  [program](program.md) 集合|   获取所有程序的集合。|
|[列出程序的 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md) 集合| 获取程序控件的集合。|
|[更新程序](../api/program-update.md) |   [程序](program.md)|  更新程序。|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   将 programControl 添加到程序。|
|[删除 programControl](../api/programcontrol-delete.md) |     无。   |   从程序中删除 programControl。|
|[列出 programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md) 集合| 列出租户中所有程序控件。|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) 集合| 列出程序控件类型。 |

## <a name="role-and-application-permission-authorization-checks"></a>角色和应用程序权限授权检查

以下目录角色是呼叫用户管理访问评审、程序和控件所需的。

| 目标资源 | 操作 | 应用程序权限 | 呼叫用户的必需目录角色 |
|:----------------|:------------------|:------------|:--------------------------------------------|
|[accessReview](accessreview.md) of an Azure AD role | 阅读 | AccessReview.Read.All 或 AccessReview.ReadWrite.All | 全局管理员、全局读取者、安全管理员、安全读取者或特权角色管理员 |
|[accessReview](accessreview.md) of an Azure AD role | 创建、更新或删除 | AccessReview.ReadWrite.All | 全局管理员或特权角色管理员 |
|[accessReview](accessreview.md) of a group or app | 阅读 | AccessReview.Read.All、AccessReview.ReadWrite.Membership 或 AccessReview.ReadWrite.All | 全局管理员、全局读取者、安全管理员、安全读者或用户管理员 |
|[accessReview](accessreview.md) of a group or app | 创建、更新或删除 | AccessReview.ReadWrite.Membership 或 AccessReview.ReadWrite.All | 全局管理员或用户管理员 |
| [program](program.md) 和 [programControl](programcontrol.md)| 阅读 | ProgramControl.Read.All 或 ProgramControl.ReadWrite.All |  全局管理员、全局读取者、安全管理员、安全读者或用户管理员 |
| [program](program.md) 和 [programControl](programcontrol.md) | 创建、更新或删除 | ProgramControl.ReadWrite.All | 全局管理员或用户管理员 |

此外，作为访问评审的分配审阅者的用户可以管理其决策，而无需担任目录角色。

## <a name="see-also"></a>另请参阅

- [管理员如何使用 Azure AD 访问评审管理用户访问](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员如何使用 Azure AD 访问评审管理来宾访问](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [管理员如何管理 Azure AD 访问评审的计划和控制](/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


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


