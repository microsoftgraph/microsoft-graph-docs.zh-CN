---
title: riskDetection 资源类型
description: 风险检测
author: cloudhandler
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6b9cfd5ed1a170613563a18351132ef444d198d4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335925"
---
# <a name="riskdetection-resource-type"></a>riskDetection 资源类型

命名空间：microsoft.graph 表示有关租户中检测到Azure AD的信息。 

Azure AD根据[各种信号和](riskyuser.md)机器学习持续评估用户风险以及应用或[](signin.md)用户登录风险。 此 API 提供对环境中的所有风险检测的编程Azure AD访问。

有关风险事件详细信息，请参阅Azure Active Directory [Identity Protection](/azure/active-directory/identity-protection/overview-identity-protection)。

>[!NOTE]
>必须具有一个Azure AD Premium P1 P2 许可证才能使用风险检测 API。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 riskDetections](../api/riskdetection-list.md)|[riskDetection](../resources/riskdetection.md) 集合|获取 [riskDetection 对象](../resources/riskdetection.md) 及其属性的列表。|
|[获取 riskDetection](../api/riskdetection-get.md)|[riskDetection](../resources/riskdetection.md)|读取 [riskDetection](../resources/riskdetection.md) 对象的属性和关系。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|活动|activityType|指示检测到的风险链接到的活动类型。 可取值为：`signin`、`user`、`unknownFutureValue`。|
|activityDateTime|DateTimeOffset|发生有风险活动的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示： `2014-01-01T00:00:00Z`|
|additionalInfo|String|与 JSON 格式的风险检测相关的其他信息。 例如，`"[{\"Key\":\"userAgent\",\"Value\":\"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/68.0.3440.106 Safari/537.36\"}]"`。 additionalInfo JSON 字符串中的可能键是：、`userAgent``alertUrl``relatedEventTimeInUtc``relatedUserAgent``deviceInformation`、`relatedLocation`、`requestId`、、`correlationId`、。 `lastActivityTimeInUtc``malwareName``clientLocation``clientIp``riskReasons` <br/>有关 riskReasons 和可能值详细信息，请参阅 [riskReasons 值](#riskreasons-values)。 |
|correlationId|String|与风险检测关联的登录的相关 ID。 此属性表示 `null` 风险检测未与登录相关联。|
|detectedDateTime|DateTimeOffset|检测到风险的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示： `2014-01-01T00:00:00Z`|
|detectionTimingType|riskDetectionTimingType|实时/脱机 (检测到的风险) 。 可取值为：`notDefined`、`realtime`、`nearRealtime`、`offline`、`unknownFutureValue`。|
|id|String|风险检测的唯一 ID。 继承自 [实体](../resources/entity.md)|
|ipAddress|String|提供发生风险的客户端的 IP 地址。|
|lastUpdatedDateTime|DateTimeOffset|上次更新风险检测的日期和时间。 DateTimeOffset 表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示： `2014-01-01T00:00:00Z`|
|location|[signInLocation](../resources/signinlocation.md)|登录的位置。|
|requestId|String|与风险检测相关联的登录请求 ID。 如果风险检测未与登录相关联，则此属性为 null。|
|riskDetail|riskDetail|检测到的风险的详细信息。 可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。|
|riskEventType|String|检测到的风险事件的类型。 可能的值为 、`unlikelyTravel``malwareInfectedIPAddress``unfamiliarFeatures``anonymizedIPAddress``maliciousIPAddress`、、`suspiciousIPAddress`、、 `passwordSpray``impossibleTravel``adminConfirmedUserCompromised``newCountry``generic``anomalousToken``tokenIssuerAnomaly``investigationsThreatIntelligence``leakedCredentials``riskyIPAddress``mcasSuspiciousInboxManipulationRules``suspiciousBrowser``suspiciousInboxForwarding`和 。`unknownFutureValue` 如果风险检测是高级检测，将显示 `generic`。 <br/>有关每个值详细信息，请参阅 [riskEventType 值](#riskeventtype-values)。|
|riskLevel|riskLevel|检测到的风险级别。 可取值为：`low`、`medium`、`high`、`hidden`、`none`、`unknownFutureValue`。|
|riskState|riskState|检测到有风险的用户或登录的状态。 可取值为：`none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised` 或 `unknownFutureValue`。|
|source|字符串|风险检测的来源。 例如，`activeDirectory`。 |
|tokenIssuerType|tokenIssuerType|指示检测到的登录风险的令牌颁发者类型。 可取值为：`AzureAD`、`ADFederationServices`、`UnknownFutureValue`。|
|userDisplayName|String|用户的用户主体名称 (UPN)。 |
|userId|String|用户的唯一 ID。|
|userPrincipalName|String|用户的用户主体名称 (UPN)。|

### <a name="riskeventtype-values"></a>riskEventType 值

| 名称 | UI 显示名称 | 说明 |
|--|--|--|
| unlikelyTravel | 非典型旅行 | 标识两个源自地理位置较远的位置的登录，如果给定过去的行为，至少其中一个位置对于用户可能也是非典型位置。  |
| 匿名IPAddress | 匿名 IP 地址 | 指示从匿名 IP 地址登录，例如，使用匿名浏览器或 VPN。 |
| maliciousIPAddress | 恶意 IP 地址 | 指示从恶意 IP 地址登录。 由于从 IP 地址或其他 IP 信誉源收到的凭据无效，因此 IP 地址被视为恶意地址，但故障率较高。 |
| unfamiliarFeatures | 不熟悉的登录属性 | 指示特征偏离过去登录属性的登录。 |
| malwareInfectedIPAddress | 恶意软件链接的 IP 地址 | 指示从感染了恶意软件的 IP 地址登录。 已弃用并且不再生成用于新检测。 |
| suspiciousIPAddress | 恶意 IP 地址 | 标识登录时已知是恶意 IP 地址的登录名。 |
| leakedCredentials | 泄露的凭据 | 指示用户的有效凭据已被泄露。 这种共享通常通过公开发布在深色 Web 上、粘贴网站，或在黑市上交易和销售凭据完成。 当 Microsoft 泄露的凭据服务从深色 Web、粘贴网站或其他源获取用户凭据时，会针对 Azure AD 用户的当前有效凭据检查这些凭据以查找有效匹配。 |
| investigationsThreatIntelligence | Azure AD威胁智能 | 指示给定用户不常见的登录活动，或与基于 Microsoft 内部和外部威胁情报源的已知攻击模式一致的登录活动。 |
| generic | 检测到其他风险 | 指示用户未启用 Identity Protection。 |
| adminConfirmedUserComprom一 | 管理员确认用户遭到入侵 | 指示管理员已 [确认用户受到威胁](../api/riskyuser-confirmcompromised.md)。 |
| passwordSpray | 密码喷射 | 指示以统一暴力方式使用公用密码攻击多个用户名，以获得未经授权的访问。 |
| anomalousToken | 异常令牌 | 指示令牌中存在异常特征，例如异常令牌生存期或从不熟悉的位置播放的令牌。 |
| tokenIssuerAnomaly | 令牌颁发者异常 | 指示关联的 SAML 令牌的 SAML 令牌颁发者可能受到威胁。 令牌中包含的声明异常或匹配已知的攻击者模式。 |
| suspiciousBrowser | 可疑浏览器 | 同一浏览器中来自不同国家/地区的多个租户的可疑登录活动。 |
| impossibleTravel | 不可能旅行 | 由 Microsoft Defender for Cloud Apps (MDCA) 。 标识两个用户活动 (一个或多个会话) 源自地理位置较远的位置，其时间短于用户从第一个位置前往第二个位置的时间，这表示其他用户使用的是同一凭据。 | 
| newCountry | 新建国家/地区 | 此检测由 MCAS Microsoft Cloud App Security (发现) 。 登录发生在给定用户最近未访问或从未访问过的位置。 |
| riskyIPAddress | 来自匿名 IP 地址的活动 | 此检测由 MCAS Microsoft Cloud App Security (发现) 。 用户从标识为匿名代理 IP 地址的 IP 地址中处于活动状态。 |
| mcasSuspiciousInboxManipulationRules | 可疑的收件箱操作规则 | 由 Microsoft Defender for Cloud Apps (MDCA) 。 标识可疑电子邮件转发规则，例如，如果用户创建了一个收件箱规则，将所有电子邮件的副本转发到外部地址。|
| suspiciousInboxForwarding | 可疑的收件箱转发 | 此检测由 MCAS Microsoft Cloud App Security (发现) 。 它会查找可疑的电子邮件转发规则，例如，如果用户创建了一个收件箱规则，将所有电子邮件的副本转发到外部地址。 |
| unknownFutureValue | 不适用 | 可发展枚举 sentinel 值。 请勿使用。 |

### <a name="riskreasons-values"></a>riskReasons 值

| riskEventType | 值 | UI 显示字符串 |
|--|--|--|
| `investigationsThreatIntelligence` | `suspiciousIP` | 此登录来自可疑 IP 地址 |
| `investigationsThreatIntelligence` | `passwordSpray` | 此用户帐户受到密码加密的攻击。 |

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
