---
title: riskDetection 资源类型
description: 风险检测
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6dad1999a6b0cea913f02bb1a072fa501a241157
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061102"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

命名空间：microsoft.graph

表示有关Azure AD租户中检测到的风险的信息。 

Azure AD根据各种信号和机器学习持续评估[用户风险](riskyuser.md)、应用或用户[登录](signin.md)风险。 此 API 提供对Azure AD环境中的所有风险检测的编程访问。

有关风险事件的详细信息，请[参阅Azure Active Directory标识保护](/azure/active-directory/identity-protection/overview-identity-protection)。

>[!NOTE]
> 1. 必须具有Azure AD Premium P1或 P2 许可证才能使用风险检测 API。
> 2. 风险检测数据的可用性受[Azure AD数据保留策略](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)的约束。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskDetections](../api/riskdetection-list.md)|[riskDetection](../resources/riskdetection.md) 集合|获取 [riskDetection](../resources/riskdetection.md) 对象及其属性的列表。|
|[获取 riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|读取 [riskDetection](../resources/riskdetection.md) 对象的属性和关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|活动|activityType|指示检测到的风险链接到的活动类型。 可取值为：`signin`、`user`、`unknownFutureValue`。|
|activityDateTime|DateTimeOffset|发生风险活动的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示： `2014-01-01T00:00:00Z`|
|additionalInfo|String|与 JSON 格式的风险检测相关联的其他信息。 例如，`"[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"`。 additionalInfo JSON 字符串中可能的键为：`userAgent`、`alertUrl`、、`relatedUserAgent``relatedEventTimeInUtc`、`deviceInformation`、`relatedLocation`、`requestId`、`correlationId`、`lastActivityTimeInUtc`、`malwareName`、、`clientLocation`、、、`clientIp`。 `riskReasons` <br/>有关 riskReasons 和可能值的详细信息，请参阅 [riskReasons 值](#riskreasons-values)。 |
|correlationId|String|与风险检测关联的登录的相关 ID。 如果风险检测未与登录关联，则此属性 `null` 。|
|detectedDateTime|DateTimeOffset|检测到风险的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示： `2014-01-01T00:00:00Z`|
|detectionTimingType|riskDetectionTimingType|检测到的风险的计时 (实时/脱机) 。 可取值为：`notDefined`、`realtime`、`nearRealtime`、`offline`、`unknownFutureValue`。|
|id|String|风险检测的唯一 ID。 继承自 [实体](../resources/entity.md)|
|ipAddress|String|提供发生风险的客户端的 IP 地址。|
|lastUpdatedDateTime|DateTimeOffset|上次更新风险检测的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示： `2014-01-01T00:00:00Z`|
|location|[signInLocation](../resources/signinlocation.md)|登录位置。|
|requestId|String|与风险检测关联的登录的请求 ID。 如果风险检测未与登录关联，则此属性为 null。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskEventType|字符串|检测到的风险事件的类型。 可能的值是`unlikelyTravel`，`anonymizedIPAddress`、、`unfamiliarFeatures``maliciousIPAddress`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials``investigationsThreatIntelligence`、`adminConfirmedUserCompromised``generic`、`mcasSuspiciousInboxManipulationRules``newCountry``anomalousToken``impossibleTravel``passwordSpray``suspiciousBrowser``riskyIPAddress``tokenIssuerAnomaly``suspiciousInboxForwarding`和。`unknownFutureValue` 如果风险检测是高级检测，将显示 `generic`。 <br/>有关每个值的详细信息，请参阅 [riskEventType 值](#riskeventtype-values)。|
|riskLevel|riskLevel|检测到的风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|检测到的风险用户或登录的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|source|String|风险检测的来源。 例如，`activeDirectory`。 |
|tokenIssuerType|tokenIssuerType|指示检测到的登录风险的令牌颁发者类型。 可取值为：`AzureAD`、`ADFederationServices`、`UnknownFutureValue`。|
|userDisplayName|String|用户的用户主体名称 (UPN)。 |
|userId|String|用户的唯一 ID。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。|

### <a name="riskeventtype-values"></a>riskEventType 值

| 名称 | UI 显示名称 | 说明 |
|--|--|--|
| unlikelyTravel | 非典型旅行 | 标识两个来自地理遥远位置的登录，根据过去的行为，其中至少有一个位置可能对用户来说也是非典型的。  |
| anonymizedIPAddress | 匿名 IP 地址 | 指示来自匿名 IP 地址的登录，例如，使用匿名浏览器或 VPN。 |
| maliciousIPAddress | 恶意 IP 地址 | 指示来自恶意 IP 地址的登录。 由于从 IP 地址或其他 IP 信誉源收到的凭据无效，IP 地址因失败率高而被视为恶意。 |
| unfamiliarFeatures | 不熟悉的登录属性 | 指示具有与过去登录属性相差的特征的登录。 |
| malwareInfectedIPAddress | 恶意软件链接的 IP 地址 | 指示来自已感染恶意软件的 IP 地址的登录。 已弃用并且不再为新检测生成。 |
| suspiciousIPAddress | 恶意 IP 地址 | 标识登录时已知为恶意的 IP 地址的登录名。 |
| leakedCredentials | 泄露的凭据 | 指示用户的有效凭据已泄露。 这种共享通常通过在深色 Web 上公开发布、粘贴网站或在黑市上交易和销售凭据来完成。 当 Microsoft 泄露的凭据服务从深色 Web、粘贴站点或其他源获取用户凭据时，会根据Azure AD用户当前的有效凭据检查这些凭据以查找有效的匹配项。 |
| investigationsThreatIntelligence | Azure AD威胁情报 | 指示针对给定用户的异常或与基于 Microsoft 内部和外部威胁情报源的已知攻击模式一致的登录活动。 |
| 通用 | 检测到其他风险 | 指示用户未启用标识保护。 |
| adminConfirmedUserCompromised | 管理员确认用户遭到入侵 | 指示管理员已 [确认用户已遭入侵](../api/riskyuser-confirmcompromised.md)。 |
| passwordSpray | 密码喷射 | 指示使用通用密码以统一暴力方式攻击多个用户名以获取未经授权的访问权限。 |
| anomalousToken | 异常令牌 | 指示令牌中有异常特征，例如异常令牌生存期或从不熟悉位置播放的令牌。 |
| tokenIssuerAnomaly | 令牌颁发者异常 | 指示关联 SAML 令牌的 SAML 令牌颁发者可能遭到入侵。 令牌中包含的声明异常或匹配已知的攻击者模式。 |
| suspiciousBrowser | 可疑浏览器 | 同一浏览器中来自不同国家的多个租户之间的可疑登录活动。 |
| impossibleTravel | 不可能旅行 | 由 Microsoft Defender for Cloud Apps (MDCA) 发现。 标识一个或多个会话 (两个用户活动，) 在比用户从第一个位置到第二个位置所用的时间短的时间段内从地理上遥远的位置出发，指示另一个用户使用相同的凭据。 | 
| newCountry | 新国家/地区 | 此检测由Microsoft Cloud App Security (MCAS) 发现。 登录发生在给定用户最近未访问或从未访问过的位置。 |
| riskyIPAddress | 来自匿名 IP 地址的活动 | 此检测由Microsoft Cloud App Security (MCAS) 发现。 用户在已标识为匿名代理 IP 地址的 IP 地址中处于活动状态。 |
| mcasSuspiciousInboxManipulationRules | 可疑的收件箱操作规则 | 由 Microsoft Defender for Cloud Apps (MDCA) 发现。 标识可疑的电子邮件转发规则，例如，如果用户创建了一个收件箱规则，该规则将所有电子邮件的副本转发到外部地址。|
| suspiciousInboxForwarding | 可疑的收件箱转发 | 此检测由Microsoft Cloud App Security (MCAS) 发现。 它查找可疑的电子邮件转发规则，例如，如果用户创建了一个收件箱规则，该规则将所有电子邮件的副本转发到外部地址。 |
| unknownFutureValue | 不适用 | 可变枚举 sentinel 值。 请勿使用。 |

### <a name="riskreasons-values"></a>riskReasons 值

| riskEventType | 值 | UI 显示字符串 |
|--|--|--|
| `investigationsThreatIntelligence` | `suspiciousIP` | 此登录来自可疑 IP 地址 |
| `investigationsThreatIntelligence` | `passwordSpray` | 此用户帐户遭到密码喷射攻击。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.riskDetection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "String (identifier)",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```
