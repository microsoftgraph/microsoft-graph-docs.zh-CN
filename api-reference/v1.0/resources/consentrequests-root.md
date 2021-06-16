---
title: Azure Active Directory同意请求
description: 使用 Azure AD 同意请求来管理尝试访问需要管理员同意的应用的用户的请求工作流。
localization_priority: Normal
author: psignoret
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: e39a1c71064282f3422a3bc48e3d019a852dbb95
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971368"
---
# <a name="azure-active-directory-consent-requests"></a>Azure Active Directory同意请求

命名空间：microsoft.graph

Azure Active Directory (Azure AD) 请求可帮助你管理尝试访问需要管理员批准的应用的用户的请求工作流。

若要允许用户请求其未经授权应用程序的访问权限或管理员同意以向自己授予同意，请首先启用同意请求工作流。 

>[!NOTE]
>当前 API 仅限于配置工作流和读取请求列表。 目前，没有任何方法可用于以编程方式批准或拒绝请求。 但是，请求的内容可用于重新创建可用于授予管理员同意和批准请求的 URL。

同意请求资源类型包括：

* [adminConsentRequestPolicy：](../resources/adminconsentrequestpolicy.md)指定可在整个租户中创建和管理应用同意请求的策略。 每个租户只有一个 **adminConsentRequestPolicy。**
* [appConsentRequest：](../resources/appconsentrequest.md)表示特定应用程序的 **userConsentRequest** 对象集合的请求。
* [userConsentRequest：](../resources/userconsentrequest.md)用户创建以使用需要管理员同意才能访问的应用的请求。
* [appConsentRequestScope：](../resources/appconsentrequestscope.md)包含为应用程序请求的动态权限范围的详细信息的资源。  

## <a name="methods"></a>方法

下表列出了可用于与同意请求资源进行交互的方法。

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md) | [adminConsentRequestPolicy](adminconsentrequestpolicy.md) 集合 | 读取 [adminConsentRequestPolicy 的属性](adminconsentrequestpolicy.md)。 |
|[更新 adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md) | [adminConsentRequestPolicy](adminconsentrequestpolicy.md) 集合 | 设置 [adminConsentRequestPolicy 的配置](adminconsentrequestpolicy.md)。 |
|[列出 appConsentRequests ](../api/appconsentrequest-list.md) | [appConsentRequest](appconsentrequest.md) 集合 | 检索 [appConsentRequest 对象](appconsentrequest.md) 的集合。 |
|[获取 appConsentRequests ](../api/appconsentrequest-get.md) | [appConsentRequest](appconsentrequest.md) 集合 | 读取 [appConsentRequest](appconsentrequest.md) 对象。 |
|[appConsentRequest：filterByCurrentUser](../api/appconsentrequest-filterByCurrentUser.md) | [appConsentRequests](../resources/appconsentrequest.md) 集合 | 读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性，当前用户是这些对象的审阅者，并且用户同意请求的状态为 `InProgress` 。 |
|[获取 userConsentRequest ](../api/userconsentrequest-get.md) | [userConsentRequest](userconsentrequest.md) 集合 | 读取 [appConsentRequest](userconsentrequest.md) 的 [userConsentRequest 对象](appconsentrequest.md)。 |
|[列出 userConsentRequests ](../api/userconsentrequest-list.md) | [userConsentRequest](userconsentrequest.md) 集合 | 检索 [appConsentRequest 的 userConsentRequest](userconsentrequest.md) [对象的集合](appconsentrequest.md)。 |
|[userConsentRequest：filterByCurrentUser](../api/userconsentrequest-filterByCurrentUser.md) | [appConsentRequests](../resources/userconsentrequest.md) 集合 | 读取当前用户是审阅者的 [userConsentRequest](../resources/userconsentrequest.md) 对象的属性。 |

## <a name="role-and-delegated-permission-authorization-checks"></a>角色和委派权限授权检查

以下目录角色是呼叫用户管理请求工作流或读取请求列表所需的。

| 操作 | 委派权限 | 呼叫用户的必需目录角色 |
|:------------------|:------------|:--------------------------------------------|
| 读取 | ConsentRequest.Read.All、ConsentRequest.ReadWrite.All | 全局管理员、全局读者、云应用管理员和应用程序管理员 |

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
