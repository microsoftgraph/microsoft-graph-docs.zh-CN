---
title: userSecurityState 资源类型
description: 包含有关用户帐户的有状态信息。
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 7bf0f249fd46ebff8b90d32159d47dd63c6682b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134274"
---
# <a name="usersecuritystate-resource-type"></a>userSecurityState 资源类型

命名空间：microsoft.graph

包含有关用户帐户的有状态信息。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|aadUserId|String|AAD 用户对象标识符 (GUID) - 表示物理/多帐户用户实体。|
|accountName|String|没有 Active Directory 域 (DNS 域的用户帐户名 -)  (也称为 `mailNickName`) 。|
|domainName|String|用户帐户的 NetBIOS/Active Directory 域 (，即域\帐户格式) 。|
|emailRole|emailRole|对于电子邮件相关警报 - 用户帐户的电子邮件"角色"。 可取值为：`unknown`、`sender`、`recipient`。|
|isVpn|布尔值|指示用户是否通过 VPN 登录。|
|logonDateTime|DateTimeOffset|登录发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。|
|logonId|String|用户登录 ID。|
|logonIp|String|IP 地址 源自登录请求。|
|logonLocation|String|位置 (IP 地址映射) 与此用户登录事件关联的位置。|
|logonType|logonType|用户登录方法。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|String|Active Directory (本地) 安全标识符 (SID) 的 SID。|
|riskScore|String|提供程序生成/计算用户帐户的风险评分。 建议的值范围为 0-1，等于百分比。|
|userAccountType|userAccountSecurityType|根据用户定义 (组) 用户帐户Windows类型。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|userPrincipalName|String|用户登录名 - Internet 格式： (用户帐户名) @ (用户帐户 DNS 域名) 。|

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
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

