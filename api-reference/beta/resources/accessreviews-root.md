---
title: Azure AD 访问审查
description: 您可以使用 Azure AD 访问评论来配置一次性或定期访问审核，以证明用户访问权限的证明。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 9a46ff3b5bd1d3df24b59335a3ab8bb1c269a7f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024575"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审查

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以使用 [AZURE AD 访问评论](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) 来配置一次性或定期访问审核，以证明用户访问权限的证明。

组成员身份和应用程序访问的访问审核的典型客户方案包括：

- 客户可以通过对应用程序和组成员身份的访问权限审查来查看和验证来宾用户访问权限。 审阅者可以使用提供的见解来有效决定来宾是否应继续访问。

- 客户可以查看和验证员工对应用程序和组成员身份的访问权限，并进行访问审核。

- 客户可以将访问审核控件收集到与您的组织相关的程序中，以跟踪对合规性或风险敏感的应用程序的审查。

还有一种相关功能，客户可以查看和验证分配给 Azure AD 角色（如全局管理员或 Azure 订阅角色）的管理用户的角色分配。  此功能包含在 [AZURE AD 特权标识管理](privilegedidentitymanagement-root.md)中。

请注意，"访问审阅" 功能（包括 API）包含在 Azure AD Premium P2 中。  在其中创建访问审核的租户必须具有有效的已购买或试用版 Azure AD Premium P2 或 EMS E5 订阅。
在创建访问审核、程序或程序控制之前，管理员必须先拥有载入，才能准备 [programControlType](programcontroltype.md) 和 [businessFlowTemplate](businessflowtemplate.md) 资源。 组织可以在 azure ad 角色或 Azure 订阅角色（azure ad PIM）的访问查看的情况下集成到 Azure AD 访问评论。


## <a name="methods"></a>方法

下表列出了可用于与访问评审相关的资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取具有特定 ID 的访问评审。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新的 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[列出 accessReviews](../api/accessreview-list.md) |    [accessReview](accessreview.md) 集合 |    列出 businessFlowTemplate 的 accessReviews。 |
|[列出 accessReview 审阅者](../api/accessreview-listreviewers.md) |      [userIdentity](useridentity.md) 集合| 获取 accessReview 的审阅者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   向 accessReview 添加审阅者。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   从 accessReview 中删除审阅者。 |
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md) 集合| 获取 accessReview 的决策。|
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md) 集合| 作为审阅者，请 accessReview 的决策。|
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) |        无。   |   向 accessReview 的审阅者发送提醒。 |
|[停止 accessReview](../api/accessreview-stop.md) |     无。   |   停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) |     无。   |   在进行中的 accessReview 中重置决策。|
|[应用 accessReview 决策](../api/accessreview-apply.md) |     无。   |   从已完成的 accessReview 应用决策。|
|[列出 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md) 集合| 获取适用于访问评审的业务流模板。|
|[创建程序](../api/program-create.md) |   [主程序](program.md)   |   创建新程序。|
|[删除程序](../api/program-delete.md) |   无。   |   删除程序。|
|[列出程序](../api/program-list.md) |  [程序](program.md) 集|   获取所有程序的集合。|
|[列出程序的 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md) 集合| 获取程序的控件的集合。|
|[更新程序](../api/program-update.md) |   [主程序](program.md)|  更新程序。|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   将 programControl 添加到程序中。|
|[删除 programControl](../api/programcontrol-delete.md) |     无。   |   从程序中删除 programControl。|
|[列出 programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md) 集合| 列出租户中所有程序之间的控件。|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md) 集合| 列出程序控制类型。 |

## <a name="role-and-application-permission-authorization-checks"></a>角色和应用程序权限授权检查

调用用户需要使用以下目录角色来管理访问评审、程序和控件。

| 目标资源 | 操作 | 应用程序权限 | 呼叫用户的必需目录角色 |
|:----------------|:------------------|:------------|:--------------------------------------------|
|Azure AD 角色的[accessReview](accessreview.md) | 阅读 | AccessReview 或 AccessReview。所有 | 全局管理员、安全管理员、安全读者或特权角色管理员 |
|Azure AD 角色的[accessReview](accessreview.md) | 创建、更新或删除 | AccessReview.ReadWrite.All | 全局管理员或特权角色管理员 |
|组或应用的[accessReview](accessreview.md) | 阅读 | AccessReview、AccessReview、成员身份或 AccessReview。 | 全局管理员、安全管理员、安全读者或用户管理员 |
|组或应用的[accessReview](accessreview.md) | 创建、更新或删除 | AccessReview 或 AccessReview 的所有成员 | 全局管理员或用户管理员 |
| [程序](program.md) 和 [programControl](programcontrol.md)| 阅读 | ProgramControl 或 ProgramControl。所有 |  全局管理员、安全管理员、安全读者或用户管理员 |
| [程序](program.md) 和 [programControl](programcontrol.md) | 创建、更新或删除 | ProgramControl.ReadWrite.All | 全局管理员或用户管理员 |

此外，为访问审核分配的审阅者的用户可以管理他们的决策，而无需在目录角色中进行管理。

## <a name="see-also"></a>另请参阅

- [管理员如何管理使用 Azure AD 访问评论的用户访问](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员如何管理使用 Azure AD 访问审查的来宾访问](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [管理员如何管理 Azure AD 访问评论的程序和控件](/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


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


