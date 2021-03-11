---
title: userSecurityState 资源类型
description: 包含有关用户帐户的有状态信息。
localization_priority: Normal
author: jpettere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edd3f3eeb4e8efffde9abd4a8fb53a8a5ddb9ea3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722256"
---
# <a name="usersecuritystate-resource-type"></a>userSecurityState 资源类型

命名空间：microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关用户帐户的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|aadUserId|String|AAD 用户对象标识符 (GUID) - 表示物理/多帐户用户实体。|
|accountName|String|没有 Active Directory 域或 DNS 域 (用户帐户的帐户) - (也称为 `mailNickName`) 。|
|domainName|String|用户帐户的 NetBIOS/Active Directory (，即域\帐户) 。|
|emailRole|emailRole|对于电子邮件相关警报 - 用户帐户的电子邮件"角色"。 可取值为：`unknown`、`sender`、`recipient`。|
|isVpn|布尔值|指示用户是否通过 VPN 登录。|
|logonDateTime|DateTimeOffset|登录发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|logonId|String|用户登录 ID。|
|logonIp|String|IP 地址源自的登录请求。|
|logonLocation|String|位置 (与此) 登录事件关联的 IP 地址映射。|
|logonType|logonType|用户登录方法。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|String|Active Directory (本地) 安全标识符 (SID) 用户的 SID。|
|riskScore|String|用户帐户的提供程序生成/计算的风险评分。 建议的值范围为 0-1，等于百分比。|
|userAccountType|userAccountSecurityType|用户帐户类型 (Windows 定义) 组成员身份类型。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|userPrincipalName|String|用户登录名 - internet 格式： (用户帐户名称) @ (用户帐户 DNS 域名) 。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


