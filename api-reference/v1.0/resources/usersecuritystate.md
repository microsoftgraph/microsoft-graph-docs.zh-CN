---
title: Logonip 资源类型
description: 包含有关用户帐户的状态信息。
author: krbain
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ae085791cb60aa6d5071332ead86033861a6305a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015370"
---
# <a name="usersecuritystate-resource-type"></a>Logonip 资源类型

命名空间：microsoft.graph

包含有关用户帐户的状态信息。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|aadUserId|String|AAD User 对象标识符 (GUID) -表示物理/多帐户用户实体。|
|帐户|String|用户帐户的帐户名 (没有 Active Directory 域或 DNS 域)  (也称为 `mailNickName`) 。|
|domainName|String|用户帐户的 NetBIOS/Active Directory 域 (即 "域 \ 帐户" 格式) 。|
|emailRole|emailRole|对于与电子邮件相关的警报-用户帐户的电子邮件 "role"。 可取值为：`unknown`、`sender`、`recipient`。|
|isVpn|Boolean|指示用户是否通过 VPN 登录。|
|logonDateTime|DateTimeOffset|登录发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|logonId|String|用户登录 ID。|
|Usersecuritystate|String|发出登录请求的 IP 地址。|
|logonLocation|String|与此用户的用户登录事件关联的 IP 地址映射)  (位置。|
|logonType|logonType|用户登录的方法。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|String|Active Directory (用户 (SID) 的本地) 安全标识符。|
|riskScore|String|提供程序生成/计算的风险分数的用户帐户。 建议的值范围为0-1，这相当于一个百分比。|
|userAccountType|userAccountSecurityType|每个 Windows 定义 (组成员身份) 的用户帐户类型。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|userPrincipalName|String|用户登录名-internet 格式： (用户帐户名) @ (用户帐户 DNS 域名) 。|

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

