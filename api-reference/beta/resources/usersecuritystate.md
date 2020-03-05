---
title: Logonip 资源类型
description: " > **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 67e5c7d2feb76346d754f582e34b5afe39af3d32
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519510"
---
# <a name="usersecuritystate-resource-type"></a>Logonip 资源类型

命名空间： microsoft. graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关用户帐户的状态信息。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|aadUserId|String|AAD 用户对象标识符（GUID）-表示物理/多帐户用户实体。|
|帐户|String|用户帐户的帐户名（不包含 Active Directory 域或 DNS 域）-（也`mailNickName`称为）。|
|domainName|String|用户帐户的 NetBIOS/Active Directory 域（即，域 \ 帐户格式）。|
|emailRole|emailRole|对于与电子邮件相关的警报-用户帐户的电子邮件 "role"。 可取值为：`unknown`、`sender`、`recipient`。|
|isVpn|布尔|指示用户是否通过 VPN 登录。|
|logonDateTime|DateTimeOffset|登录发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|logonId|String|用户登录 ID。|
|Usersecuritystate|String|发出登录请求的 IP 地址。|
|logonLocation|String|与用户登录事件关联的此用户的位置（按 IP 地址映射）。|
|logonType|logonType|用户登录的方法。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|字符串|用户的 Active Directory （本地）安全标识符（SID）。|
|riskScore|String|提供程序生成/计算的风险分数的用户帐户。 建议的值范围为0-1，这相当于一个百分比。|
|userAccountType|userAccountSecurityType|每个 Windows 定义的用户帐户类型（组成员身份）。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|userPrincipalName|String|用户登录名-internet 格式：（用户帐户名称） @ （用户帐户 DNS 域名）。|

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
