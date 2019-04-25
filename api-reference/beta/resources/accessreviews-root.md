---
title: Azure AD 访问审查
description: 您可以使用 Azure AD 访问评论来配置一次性或定期访问审核, 以证明用户访问权限的证明。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 212af4ad8519f7ec54fb56ceffee0a0d4de16027
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544114"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审查

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

您可以使用[Azure AD 访问评论](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview)来配置一次性或定期访问审核, 以证明用户访问权限的证明。

组成员身份和应用程序访问的访问审核的典型客户方案包括:
   
- 客户可以通过对应用程序和组成员身份的访问权限审查来查看和验证来宾用户访问权限。 审阅者可以使用提供的见解来有效决定来宾是否应继续访问。
      
- 客户可以查看和验证员工对应用程序和组成员身份的访问权限, 并进行访问审核。
   
- 客户可以将访问审核控件收集到与您的组织相关的程序中, 以跟踪对合规性或风险敏感的应用程序的审查。

还有一种相关功能, 客户可以查看和验证分配给 Azure AD 角色 (如全局管理员或 azure 订阅角色) 的管理用户的角色分配。  此功能包含在[Azure AD 特权标识管理](privilegedidentitymanagement-root.md)中。

请注意, "访问审阅" 功能 (包括 API) 包含在 Azure AD Premium P2 中。 

## <a name="methods"></a>方法

下面是 Azure AD access 检查提供的方法的列表。  

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取具有特定 id 的访问评审。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新的 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[列出 accessReview 审阅者](../api/accessreview-listreviewers.md) |      [userIdentity](useridentity.md)集合| 获取 accessReview 的审阅者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   向 accessReview 添加审阅者。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   从 accessReview 中删除审阅者。 |
|[列出 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)集合| 获取 accessReview 的决策。|
|[列出我的 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)集合| 作为审阅者, 请 accessReview 的决策。|
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) |        无。   |   向 accessReview 的审阅者发送提醒。 |
|[停止 accessReview](../api/accessreview-stop.md) |     无。   |   停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) |     无。   |   在进行中的 accessReview 中重置决策。|
|[应用 accessReview 决策](../api/accessreview-apply.md) |     无。   |   从已完成的 accessReview 应用决策。|
|[列出 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md)集合| 获取适用于访问评审的业务流模板。|
|[创建程序](../api/program-create.md) |   [主程序](program.md)   |   创建新程序。|
|[删除程序](../api/program-delete.md) |   无。   |   删除程序。|
|[列出程序](../api/program-list.md) |  [程序](program.md)集|   获取所有程序的集合。|
|[列出程序的 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md)集合| 获取程序的控件的集合。|
|[更新程序](../api/program-update.md) |   [主程序](program.md)|  更新程序。|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   将 programControl 添加到程序中。|
|[删除 programControl](../api/programcontrol-delete.md) |     无。   |   从程序中删除 programControl。|
|[列出 programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md)集合| 列出租户中所有程序之间的控件。|
|[列出 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)集合| 列出程序控制类型。 |


## <a name="see-also"></a>另请参阅

- [管理员如何管理使用 Azure AD 访问评论的用户访问](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员如何管理使用 Azure AD 访问审查的来宾访问](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [管理员如何管理 Azure AD 访问评论的程序和控件](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviews-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
