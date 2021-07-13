---
title: 更新 mobileDeviceManagementPolicy
description: 更新移动设备管理对象的属性。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: ef94012247c011026b8c24a9219aa2d7c3228131
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401356"
---
# <a name="update-mobiledevicemanagementpolicy"></a>更新 mobileDeviceManagementPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [mobilityManagementPolicy 对象](../resources/mobilitymanagementpolicy.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.Read.All、Policy.ReadWrite.MobilityManagement|
|委派（个人 Microsoft 帐户） | 不支持。|
|应用程序 | 不支持。|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/mobileDeviceManagementPolicies/{id}
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的 JSON 表示形式。

在请求正文中，提供下面列出的应更新的字段的值。 **注意：** 不能将 `PATCH` 操作用于 `appliesTo` 其他属性。

|属性|类型|说明|
|:---|:---|:---|
|appliesTo|policyScope|确定此策略设置应用于的组。 可能的值是 `none` `all` `selected` **：、、重要：** `selected` 指定此属性时不能使用。 使用 [includedGroups](../api/mobiledevicemanagementpolicies-post-includedgroups.md) 添加特定组。 使用 `all` 将删除任何现有组。|
|complianceUrl|String|移动管理应用程序的合规性 URL|
|discoveryUrl|String|移动管理应用程序的发现 URL|
|termsOfUseUrl|String|移动管理应用程序的使用条款 URL|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_mobilitymanagementpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.mobilityManagementPolicy",
  "complianceUrl": "https://portal.uem.contoso.com/?portalAction=Compliance",
  "discoveryUrl": "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
  "termsOfUseUrl": "https://portal.uem.contoso.com/TermsofUse.aspx"
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
