---
title: Azure Active Directory 同意请求
description: 使用 Azure AD 许可请求管理尝试访问需要管理员同意的应用的用户的请求工作流。
ms.localizationpriority: medium
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: abac5b526601ad4aec522be707e24c210f1f8f3a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442862"
---
# <a name="azure-active-directory-consent-requests"></a>Azure Active Directory 同意请求

命名空间：microsoft.graph

Azure Active Directory (Azure AD) 许可请求可帮助你管理尝试访问需要管理员批准的应用的用户的请求工作流。

若要允许用户请求对未经授权的应用程序的访问权限或管理员同意，请先启用同意请求工作流。 

>[!NOTE]
>当前 API 仅限于配置工作流和读取请求列表。 目前，没有任何方法可用于以编程方式批准或拒绝请求。 但是，请求的内容可用于重新创建可用于授予管理员同意和批准请求的 URL。

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]

同意请求资源类型包括：

* [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)：指定可以为整个租户创建和管理应用同意请求的策略。 每个租户有一个 **adminConsentRequestPolicy** 。
* [appConsentRequest](../resources/appconsentrequest.md)：一个请求，表示特定应用程序的 **userConsentRequest** 对象的集合。
* [userConsentRequest](../resources/userconsentrequest.md)：用户创建的请求，用于使用需要管理员许可才能访问的应用。
* [appConsentRequestScope](../resources/appconsentrequestscope.md)：一个资源，其中包含为应用程序请求的动态权限范围的详细信息。  

## <a name="methods"></a>方法

下表列出了可用于与同意请求资源交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md) | [adminConsentRequestPolicy](adminconsentrequestpolicy.md) 集合 | 读取 [adminConsentRequestPolicy](adminconsentrequestpolicy.md) 的属性。 |
|[更新 adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md) | [adminConsentRequestPolicy](adminconsentrequestpolicy.md) 集合 | 设置 [adminConsentRequestPolicy](adminconsentrequestpolicy.md) 的配置。 |
|[列出 appConsentRequests ](../api/appconsentapprovalroute-list-appconsentrequests.md) | [appConsentRequest](appconsentrequest.md) 集合 | 检索 [appConsentRequest](appconsentrequest.md) 对象的集合。 |
|[获取 appConsentRequests ](../api/appconsentrequest-get.md) | [appConsentRequest](appconsentrequest.md) 集合 | 读 [取 appConsentRequest](appconsentrequest.md) 对象。 |
|[appConsentRequest：filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md) | [appConsentRequests](../resources/appconsentrequest.md) 集合 | 读取当前用户是审阅者且用户同意请求`InProgress`的状态为的 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性。 |
|[获取 userConsentRequest ](../api/userconsentrequest-get.md) | [userConsentRequest](userconsentrequest.md) 集合 | 读取 [appConsentRequest](userconsentrequest.md) 的 [userConsentRequest](appconsentrequest.md) 对象。 |
|[列出 userConsentRequests ](../api/appconsentrequest-list-userconsentrequests.md) | [userConsentRequest](userconsentrequest.md) 集合 | 检索 [appConsentRequest](appconsentrequest.md) 的 [userConsentRequest](userconsentrequest.md) 对象的集合。 |
|[userConsentRequest：filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md) | [appConsentRequests](../resources/userconsentrequest.md) 集合 | 读取当前用户是审阅者的 [userConsentRequest](../resources/userconsentrequest.md) 对象的属性。 |

## <a name="role-and-delegated-permission-authorization-checks"></a>角色和委派权限授权检查

调用用户需要以下目录角色来管理请求工作流或读取请求列表。

| Operation | 委派权限 | 调用用户所需的目录角色 |
|:------------------|:------------|:--------------------------------------------|
| 读取 | ConsentRequest.Read.All、ConsentRequest.ReadWrite.All | 全局管理员、全局阅读器、云应用管理员和应用程序管理员 |

## <a name="see-also"></a>另请参阅

- [配置管理员同意工作流 (预览) ](/azure/active-directory/manage-apps/configure-admin-consent-workflow?preserve-view=true)


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
