---
title: tiIndicator 资源类型
description: 威胁智能 (TI) 指标表示用于标识恶意活动的数据。 如果您的组织使用威胁指示器 (通过生成自己的、从开放源源获取、与合作伙伴组织或社区共享, 或购买数据源), 则通常需要在各种安全性中使用这些指示器用于匹配日志数据的工具。 Graph security tiIndicators 实体允许您将威胁指示器上载到 Microsoft 安全工具, 以执行允许、阻止或警报等操作。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: fd86dc4da572c17e35afe939977b65ff99bd30be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582849"
---
# <a name="tiindicator-resource-type"></a>tiIndicator 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

威胁智能 (TI) 指标表示用于标识恶意活动的数据。 如果您的组织使用威胁指示器, 可以通过生成自己的、从开放源源中获取它们、与合作伙伴组织或社区共享, 也可以通过购买数据源进行通信, 因此您可能需要在各种安全性中使用这些指示器用于匹配日志数据的工具。 microsoft Graph Security API **tiIndicators**实体允许您将威胁指示器上载到 Microsoft 安全工具, 以执行允许、阻止或警报等操作。

通过**tiIndicators**上载的威胁指示器将与 Microsoft 威胁情报结合使用, 以为您的组织提供自定义安全解决方案。 使用**tiIndicators**实体时, 您可以指定要通过**targetProduct**属性使用指示器的 Microsoft 安全解决方案, 并指定安全解决方案应对其执行的操作 (允许、阻止或警告)。通过**action**属性应用指示器。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 tiIndicator](../api/tiindicator-get.md) | [tiIndicator](tiindicator.md) | 读取 tiIndicator 对象的属性和关系。 |
| [创建 tiIndicator](../api/tiindicators-post.md) | [tiIndicator](tiindicator.md) | 通过发布到 tiIndicators 集合创建新的 tiIndicator。 |
| [列出 tiIndicator](../api/tiindicators-list.md) | [tiIndicator](tiindicator.md)集合 | 获取 tiIndicator 对象集合。 |
| [更新](../api/tiindicator-update.md) | [tiIndicator](tiindicator.md) | 更新 tiIndicator 对象。 |
| [删除](../api/tiindicator-delete.md) | 无 | 删除 tiIndicator 对象。 |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|无| 删除多个 tiIndicator 对象。|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|无| 通过`externalId`属性删除多个 tiIndicator 对象。|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|[tiIndicator](tiindicator.md)集合|通过发布 tiIndicators 集合创建新的 tiIndicators。|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|[tiIndicator](tiindicator.md)集合| 更新多个 tiIndicator 对象。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|action|string| 在 targetProduct 安全工具中匹配指标时要应用的操作。 可取值为：`unknown`、`allow`、`block`、`alert`。 **必需。**|
|activityGroupNames|String collection|负责威胁指示器所涵盖的恶意活动的各方的网络威胁智能名称。|
|additionalInformation|String|可以放置其他 tiIndicator 属性中未涵盖的指标中的额外数据的 "容器" 区域。 放置在 additionalInformation 中的数据通常不会被 targetProduct 安全工具使用。|
|azureTenantId|String| 当指标为引入时由系统进行标记。 提交客户端的 Azure Active Directory 租户 id。 **必需。**|
|confidence|Int32|一个整数, 表示对指示器中的数据准确标识恶意行为的可信度。 可接受的值为0– 100, 100 的值为最高。|
|说明|String| 由指示器表示的威胁的简短说明 (100 个字符或更少)。 **必需。**|
|diamondModel|[diamondModel](#diamondmodel-values)|此指示器所在的菱形模型的面积。 可取值为：`unknown`、`adversary`、`capability`、`infrastructure` 或 `victim`。|
|expirationDateTime|DateTimeOffset| 指示指示器过期时间的日期/时间字符串。 所有指标都必须具有到期日期, 以避免系统中的陈旧指示器持久化。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。 **必需。**|
|externalId|String| 将指示器与指示器提供程序的系统 (例如外键) 相结合的标识号。 |
|id|字符串|当指标为引入时由系统创建。 生成的 GUID/唯一标识符。 只读。|
|ingestedDateTime|DateTimeOffset| 当指标为引入时由系统进行标记。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|isActive|Boolean| 用于停用系统中的指示器。 默认情况下, 提交的任何指示器都设置为活动状态。 但是, 提供程序可能会将此设置为 "False" 的现有指示器提交到系统中停用指示器。|
|killChain|[killChain](#killchain-values)集合|一个 JSON 字符串数组, 用于描述此指示器针对终止链上的哪个点或点。 有关确切值, 请参阅下面的 "killChain 值"。 |
|knownFalsePositives|String|指示符可能导致误报的情况。 这应该是可读的文本。|
|lastReportedDateTime|DateTimeOffset|上次发现指示器的时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|malwareFamilyNames|String collection|与指示器关联的恶意软件系列名称 (如果存在)。 如果所有可能都可以通过 Windows Defender 安全智能[威胁百科全书](https://www.microsoft.com/wdsi/threats)找到, microsoft 将首选 microsoft 恶意软件系列名称。|
|passiveOnly|Boolean |确定该指示符是否应触发对最终用户可见的事件。 如果设置为 "true", 则安全工具将不会通知最终用户已发生 "命中"。 通常情况下, 这通常被视为审核或静默模式, 安全产品只需记录已发生的匹配项, 但不会执行该操作。 默认值为 false。 |
|度|Int32| 一个整数, 表示由指示器中的数据标识的恶意行为的严重程度。 可接受的值为0– 5, 其中5为最严重, 0 表示根本不严重。 默认值为3。 |
|tags|String 集合|存储任意标记/关键字的字符串的 JSON 数组。 |
|targetProduct|String|一个字符串值, 表示应应用指标的单个安全产品。 可接受的值`Azure Sentinel`为:。 **必需**|
|threatType|[threatType](#threattype-values)| 每个指示器都必须具有有效的指示器威胁类型。 可取值为：`Botnet`、`C2`、`CryptoMining`、`Darknet`、`DDoS`、`MaliciousUrl`、`Malware`、`Phishing`、`Proxy`、`PUA`、`WatchList`。 **必需。** |
|tlpLevel|[tlpLevel](#tlplevel-values)| 指标的流量灯协议值。 可取值为：`unknown`、`white`、`green`、`amber` 或 `red`。 **必需。**|

### <a name="indicator-observables---email"></a>指标 observable-电子邮件

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|emailEncoding|String|电子邮件中使用的文本编码的类型。|
|emailLanguage|String|电子邮件的语言。|
|emailRecipient|String|收件人电子邮件地址。|
|emailSenderAddress|String|attacker& # 124; 牺牲品的电子邮件地址。|
|emailSenderName|String|attacker& # 124; 牺牲品的显示名称。|
|emailSourceDomain|String|电子邮件中使用的域。|
|emailSourceIpAddress|String|电子邮件的源 IP 地址。|
|emailSubject|String|电子邮件的主题行。|
|emailXMailer|String|在电子邮件中使用的邮件散播值。|

### <a name="indicator-observables---file"></a>指标 observable-文件

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|编译文件时的日期/时间。 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|fileCreatedDateTime|DateTimeOffset| 创建文件时的日期/时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|fileHashType|string| 存储在 fileHashValue 中的哈希的类型。 可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash` 或 `ctph`。|
|fileHashValue|String| 文件哈希值。|
|fileMutexName|String| 在基于文件的检测中使用的 Mutex 名称。|
|fileName|String|如果该标记是基于文件的, 则为该文件的名称。 可以用逗号分隔多个文件名。 |
|filePacker|String|用于生成相关文件的 packer。|
|路径|String|指示受损的文件路径。 可以是 Windows 或 * nix 样式路径。|
|fileSize|Int64|文件大小 (以字节为单位)。|
|类型|String| 文件类型的文本说明。 例如, "Word Document" 或 "Binary"。|

### <a name="indicator-observables---network"></a>指标 observable-网络

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|domainName|String|与此指标关联的域名称。 应为 topleveldomain 的格式 (例如, baddomain.domain.net)|
|networkCidrBlock|String| 此指示器中引用的网络的 CIDR 块表示法表示形式。 仅在无法识别源和目标时使用。 |
|networkDestinationAsn|Int32|指示器中引用的网络的目标自治系统标识符。|
|networkDestinationCidrBlock|String|此指标中目标网络的 CIDR 块表示法表示形式。|
|networkDestinationIPv4|String|IPv4 IP 地址目标。|
|networkDestinationIPv6|String|IPv6 IP 地址目标。|
|networkDestinationPort|Int32|TCP 端口目标。|
|networkIPv4|String| IPv4 IP 地址。 仅在无法识别源和目标时使用。 |
|networkIPv6|String| IPv6 IP 地址。 仅在无法识别源和目标时使用。 |
|networkPort|Int32| TCP 端口。 仅在无法识别源和目标时使用。 |
|networkProtocol|Int32|IPv4 标头中的协议字段的十进制表示形式。|
|networkSourceAsn|Int32|指示器中引用的网络的源自治系统标识符。|
|networkSourceCidrBlock|String|此指示器中源网络的 CIDR 块表示法表示形式|
|networkSourceIPv4|String|IPv4 IP 地址源。|
|networkSourceIPv6|String|IPv6 IP 地址源。|
|networkSourcePort|Int32|TCP 端口源。|
|url|String|统一资源定位器。 此 URL 必须符合 RFC 1738。|
|userAgent|String|来自 web 请求的用户代理字符串, 可能表明已泄露。|

### <a name="diamondmodel-values"></a>diamondModel 值

有关此模型的信息, 请参阅[菱形模型](http://diamondmodel.org)。

| 值 | 说明 |
|:-------|:------------|
|对手|该指示器描述了敌人。|
|性能|指示器是入侵者的一种功能。|
|基本|此指标介绍了入侵者的基础结构。|
|者|该指标描述敌人的牺牲品。|

### <a name="killchain-values"></a>killChain 值

| 值 | 说明 |
|:-------|:------------|
|Actions|Indcates 攻击者利用受危害的系统执行诸如分布式拒绝服务攻击之类的操作。|
|C2|表示操纵受损系统时所使用的控制通道。|
|Delivery|将攻击代码分发给受害者的过程 (例如, USB、电子邮件、网站)。|
|具备|利用漏洞的攻击代码 (例如, 代码执行)。|
|安装|在漏洞受到攻击后安装恶意软件。|
|侦测|指标是活动组收集信息以用于将来的攻击的证据。|
|Weaponization|将漏洞转换为攻击代码 (例如恶意软件)。|

### <a name="threattype-values"></a>threatType 值

| 值 | 说明 |
|:-------|:------------|
|僵尸网络| 指标对僵尸网络节点/成员进行了详细说明。|
|C2|指标对僵尸网络的命令 & 控件节点进行了详细说明。|
|CryptoMining|涉及此网络地址/URL 的流量是 CyrptoMining/资源滥用的指示。|
|Darknet|指标是 Darknet 节点/网络的指标。
|DDoS|与活动或即将到来的 DDoS 市场活动相关的指标。|
|MaliciousUrl|为恶意软件提供服务的 URL。|
|恶意软件|描述恶意文件的指示器。|
|网络钓鱼|与仿冒活动相关的指示器。|
|代理|指标是代理服务的指标。|
|PUA|可能有害的应用程序。|
|WatchList|这是在不能准确确定威胁或需要手动解释的情况下放置指示器的常规存储桶。 将数据提交到系统的合作伙伴通常不应使用此方法。|

### <a name="tlplevel-values"></a>tlpLevel 值

每个指示器在提交时还必须有流量轻型协议值。 此值表示给定指标的敏感度和共享作用域。

| 值 | 说明 |
|:-------|:------------|
|白色| 共享范围: 无限制。 指示器可以自由共享, 无需限制。|
|绿色| 共享作用域: 社区。 指标可与安全社区共享。|
|亮| 共享作用域: 受限。 这是指示器的默认设置, 并且仅将共享限制为 "需要已知" 为1的服务和实现威胁智能2的服务的服务和服务操作员, 这些客户端的系统表现出与指标一致的行为。|
|红色| 共享作用域: 个人。 这些指标仅可直接共享, 最好是人员。 通常情况下, TLP 红色指示器不会引入, 因为其预定义限制。 如果提交了 TLP 红色指示器, 则还应将 "PassiveOnly" 属性设置`True`为。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tiIndicator",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "string",
  "activityGroupNames": ["String"],
  "additionalInformation": "String",
  "azureTenantId": "String",
  "confidence": 1024,
  "description": "String",
  "diamondModel": "string",
  "domainName": "String",
  "emailEncoding": "String",
  "emailLanguage": "String",
  "emailRecipient": "String",
  "emailSenderAddress": "String",
  "emailSenderName": "String",
  "emailSourceDomain": "String",
  "emailSourceIpAddress": "String",
  "emailSubject": "String",
  "emailXMailer": "String",
  "expirationDateTime": "String (timestamp)",
  "externalId": "String",
  "fileCompileDateTime": "String (timestamp)",
  "fileCreatedDateTime": "String (timestamp)",
  "fileHashType": "string",
  "fileHashValue": "String",
  "fileMutexName": "String",
  "fileName": "String",
  "filePacker": "String",
  "filePath": "String",
  "fileSize": 1024,
  "fileType": "String",
  "id": "String (identifier)",
  "ingestedDateTime": "String (timestamp)",
  "isActive": true,
  "killChain": ["String"],
  "knownFalsePositives": "String",
  "lastReportedDateTime": "String (timestamp)",
  "malwareFamilyNames": ["String"],
  "networkCidrBlock": "String",
  "networkDestinationAsn": 1024,
  "networkDestinationCidrBlock": "String",
  "networkDestinationIPv4": "String",
  "networkDestinationIPv6": "String",
  "networkDestinationPort": 1024,
  "networkIPv4": "String",
  "networkIPv6": "String",
  "networkPort": 1024,
  "networkProtocol": 1024,
  "networkSourceAsn": 1024,
  "networkSourceCidrBlock": "String",
  "networkSourceIPv4": "String",
  "networkSourceIPv6": "String",
  "networkSourcePort": 1024,
  "passiveOnly": true,
  "severity": 1024,
  "tags": ["String"],
  "targetProduct": "String",
  "threatType": "String",
  "tlpLevel": "string",
  "url": "String",
  "userAgent": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
