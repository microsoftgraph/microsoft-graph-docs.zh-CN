---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac605e93603cb39491fd980e78a9b0f0026541eb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492200"
---
# <a name="update-authorizationpolicy"></a>更新 authorizationPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新[authorizationPolicy](../resources/authorizationpolicy.md)对象的属性。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy。读身份验证|
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | Policy。读身份验证|

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | 持有者 {token} |
| Content-type | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|  
|displayName|String| 此策略的显示名称。 |  
|说明|String| 此策略的说明。 |  
|guestUserRoleId|Guid| 表示应向来宾用户授予的角色的角色 templateId。 若要查找可用角色模板的列表，请参阅[List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) 。 目前只有受支持的角色是用户（a0b1b346-4d3e-4e8b-98f8-753987be4970）、来宾用户（10dae51f-b6af-4016-8d66-8c2a99b929b3）和受限制的来宾用户（2af84b1e-32c8-42b7-82bc-daa82404023b）。 | 
|enabledPreviewFeatures|集合（string）| 租户上启用了专用预览的功能列表。 | 
|blockMsolPowerShell|Boolean| 若要禁用 MSOL PowerShell 的使用，请将此属性设置为 `true` 。 设置为 `true` 将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。 这不会影响 Azure AD Connect 或 Microsoft Graph。 | 

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a>示例1：更新或设置租户的来宾用户访问级别

#### <a name="request"></a>请求

下面展示了示例请求。 在此示例中，将来宾访问级别修改为受限制的来宾用户。

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a>示例2：在租户上为预览启用新功能

#### <a name="request"></a>请求

下面展示了示例请求。

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a>示例3：阻止租户中的 MSOL PowerShell

#### <a name="request"></a>请求

下面展示了示例请求。

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "blockMsolPowerShell": true
}

```
#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
