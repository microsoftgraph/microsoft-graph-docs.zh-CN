# <a name="usersecuritystate-resource-type"></a>userSecurityState 资源类型

包含有关用户帐户的状态信息。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|aadUserId|字符串|AAD 用户对象标识符 (GUID) - 表示物理/多帐户用户实体。|
|accountName|字符串|用户帐户的帐户名称（没有 Active Directory 域和 DNS 域）- (也称为 `mailNickName`)。|
|domainName|字符串|用户帐户的 NetBIOS/Active Directory 域 （即域\帐户格式）。|
|emailRole|emailRole|与电子邮件相关的通知 - 用户帐户的电子邮件“角色”。 可取值为：`unknown`、`sender`、`recipient`。|
|isVpn|布尔值|指示用户是否通过 VPN 登录。|
|logonDateTime|DateTimeOffset|登录发生的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。|
|logonId|字符串|用户登录 ID。|
|logonIp|字符串|登录请求源自的 IP 地址。|
|logonLocation|字符串|此用户与用户登录事件关联的位置（通过 IP 地址映射）。|
|logonType|logonType|用户登录的方法。 可取值为：`unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|字符串|用户的 Active Directory （本地）安全标识符 (SID)。|
|riskScore|字符串|提供程序生成/计算的用户帐户风险评分。 建议值的范围为 0-1，相当于百分比。|
|userAccountType|userAccountSecurityType|用户帐户类型 （组成员身份），依照 Windows 定义。 可取值为：`unknown`、`standard`、`power`、`administrator`。|
|userPrincipalName|字符串|用户登录名 - 互联网格式：（用户帐户名）@（用户帐户 DNS 域名）。|

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
