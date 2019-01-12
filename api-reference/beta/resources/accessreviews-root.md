---
title: Azure AD 访问审阅
description: 您可以使用 Azure AD 访问 reviews （英文） 配置的用户的访问权限的审计一次性或定期访问审阅。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 24571e8d83d6d321ba2bf20d9beae9ba6487e286
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975349"
---
# <a name="azure-ad-access-reviews"></a>Azure AD 访问审阅

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

您可以使用[Azure AD access 会检查](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview)配置一次性或定期访问审阅的审计的用户的访问权限。

访问的典型客户方案审阅的组成员身份和应用程序访问：
   
- 客户可以查看并使用其访问应用程序的访问评论和组的成员身份证明来宾用户访问。 审阅者可以使用提供高效地确定是否应可持续来宾访问见解。
      
- 客户可以检查和验证员工访问应用程序和组成员身份与 access 评论。
   
- 客户可以收集到相关的组织跟踪审阅合规性或风险敏感应用程序的程序中访问审阅控件。

此外，还有以便客户能够查看并保证管理用户的角色分配到 Azure AD 角色，如全局管理员或 Azure 订阅角色分配的相关的功能。  [Azure AD 特权身份管理](privilegedidentitymanagement-root.md)包含此功能。

请注意，将访问审阅功能，包括 API，包括在 Azure AD Premium P2。 

## <a name="methods"></a>方法

下面是所提供的 Azure AD 的方法列表访问 reviews （英文）。  

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   获取与特定 id 访问审阅。 |
|[创建 accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   创建新 accessReview。 |
|[删除 accessReview](../api/accessreview-delete.md) | 无。   | 删除 accessReview。 |
|[更新 accessReview](../api/accessreview-update.md) | [accessReview](accessreview.md) | 更新 accessReview。 |
|[列表 accessReview 审阅者](../api/accessreview-listreviewers.md) |      [userIdentity](useridentity.md)集合| 要获取 accessReview 审阅的者。 |
|[添加 accessReview 审阅者](../api/accessreview-addreviewer.md) |      无。   |   将审阅者添加到 accessReview。 |
|[删除 accessReview 审阅者](../api/accessreview-removereviewer.md) | 无。  |   删除 accessReview 审阅者。 |
|[列表 accessReview 决策](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)集合| 获取 accessReview 的决策。|
|[列出我 accessReview 决策](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)集合| 审阅者，以获取 accessReview 我决策。|
|[发送 accessReview 提醒](../api/accessreview-sendreminder.md) |        无。   |   向审阅者的 accessReview 发送提醒。 |
|[停止 accessReview](../api/accessreview-stop.md) |     无。   |   停止 accessReview。 |
|[重置 accessReview 决策](../api/accessreview-reset.md) |     无。   |   重置正在进行 accessReview 决策。|
|[应用 accessReview 决策](../api/accessreview-apply.md) |     无。   |   应用已完成 accessReview 从的决策。|
|[列表 businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md)集合| 获取业务流程模板相应访问 reviews （英文）。|
|[创建程序](../api/program-create.md) |   [程序](program.md)   |   创建一个新的程序。|
|[删除程序](../api/program-delete.md) |   无。   |   删除一个程序。|
|[列表程序](../api/program-list.md) |  [程序](program.md)集|   获取所有的程序的集合。|
|[对程序的列表 programControls](../api/program-listcontrols.md) |      [programControl](programcontrol.md)集合| 获取一个程序的控件的集合。|
|[更新程序](../api/program-update.md) |   [程序](program.md)|  更新程序。|
|[创建 programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   添加到程序 programControl。|
|[删除 programControl](../api/programcontrol-delete.md) |     无。   |   从某个程序中删除 programControl。|
|[列表 programControls](../api/programcontrol-list.md) | [programControl](programcontrol.md)集合| 在租户中的所有程序列表控件中。|
|[列表 programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)集合| 列出程序控件类型。 |


## <a name="see-also"></a>另请参阅

- [管理员可以如何管理 Azure AD 访问用户访问审阅](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [管理员可以如何管理与 Azure AD 访问来宾访问审阅](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [如何，管理员可以管理程序和控件的 Azure AD 访问 reviews （英文）](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
