---
title: tiIndicator 资源类型
description: 威胁情报 (TI) 指示器表示用于识别恶意活动的数据。
ms.localizationpriority: medium
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 3abd788b6bd4199b5ef64baf4c89308437724f98
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424628"
---
# <a name="tiindicator-resource-type"></a>tiIndicator 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

威胁情报 (TI) 指示器表示用于识别恶意活动的数据。 如果组织使用威胁指示器，无论是通过生成自己的指标、从开放源源获取指标、与合作伙伴组织或社区共享，还是通过购买数据馈送获得，您可能希望在各种安全工具中使用这些指示器与日志数据匹配。 Microsoft Graph安全 API **tiIndicators** 实体允许你将威胁指示器上载到 Microsoft 安全工具，以便执行允许、阻止或警报操作。

通过 **tiIndicator** 上载的威胁指示器将与 Microsoft 威胁智能结合使用，为组织提供自定义的安全解决方案。 使用 **tiIndicators** 实体时，通过 **targetProduct** 属性指定想要利用其指示器的 Microsoft 安全解决方案，并指定操作 (允许、阻止或警报) 安全解决方案应通过 **action** 属性应用这些指示器。

当前 **targetProduct** 支持包括以下内容：

- **Azure Sentinel** – 支持下一节中列出的所有记录 **tiIndicators** 方法。
- **Microsoft Defender for Endpoint** – 支持以下 **tiIndicators** 方法：
     - [获取 tiIndicator](../api/tiindicator-get.md)
     - [创建 tiIndicator](../api/tiindicators-post.md)
     - [列出 tiIndicator](../api/tiindicators-list.md)
     - [更新](../api/tiindicator-update.md)
     - [删除](../api/tiindicator-delete.md)

     即将推出对批量方法的支持。

  > [!NOTE]
  >以下指示器类型受 Microsoft Defender for Endpoint targetProduct 支持：
  > - 文件
  > - IP 地址：Microsoft Defender for Endpoint 仅支持目标 IPv4/IPv6 – 在 networkDestinationIPv4 或 microsoft Graph Security API **tiIndicator** 中的 networkDestinationIPv6 属性中设置属性。
  > - URL/域

   每个租户的 Microsoft Defender for Endpoint 的指示器限制为 15000 个。

有关支持的指示器类型以及每个租户的指示器数限制的详细信息，请参阅[管理指示器](/windows/security/threat-protection/microsoft-defender-atp/manage-indicators)。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 tiIndicator](../api/tiindicator-get.md) | [tiIndicator](tiindicator.md) | 读取 tiIndicator 对象的属性和关系。 |
| [创建 tiIndicator](../api/tiindicators-post.md) | [tiIndicator](tiindicator.md) | 通过发布到 tiIndicators 集合创建新的 tiIndicator。 |
| [列出 tiIndicator](../api/tiindicators-list.md) | [tiIndicator](tiindicator.md) 集合 | 获取 tiIndicator 对象集合。 |
| [更新](../api/tiindicator-update.md) | [tiIndicator](tiindicator.md) | 更新 tiIndicator 对象。 |
| [删除](../api/tiindicator-delete.md) | 无 | 删除 tiIndicator 对象。 |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|无| 删除多个 tiIndicator 对象。|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|无| 通过 属性删除多个 tiIndicator `externalId` 对象。|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|[tiIndicator](tiindicator.md) 集合|通过发布 tiIndicators 集合创建新的 tiIndicator。|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|[tiIndicator](tiindicator.md) 集合| 更新多个 tiIndicator 对象。|

### <a name="methods-supported-by-each-target-product"></a>每个目标产品支持的方法

| 方法                                                          | Azure Sentinel                                                                                                                                                                                                                                                                                                                                                                      | Microsoft Defender for Endpoint                                                                                                                                                                                               |
|:----------------------------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [创建 tiIndicator](../api/tiindicators-post.md)               | 所需字段包括 `action` ：、、、、、、，以及 `azureTenantId` `description` `expirationDateTime` `targetProduct` `threatType` `tlpLevel` 至少一个可观测的电子邮件、网络或文件。                                                                                                                                                                                                | 必需字段包括： 和以下值之一 `action` `domainName` `url` `networkDestinationIPv4` `networkDestinationIPv6` `fileHashValue` ：、 ( `fileHashType` 必须提供以防 `fileHashValue`) 。 |
| [提交 tiIndicator](../api/tiindicator-submittiindicators.md) | 有关每个 [tiIndicator](../api/tiindicators-post.md) 的必填字段，请参阅创建 tiIndicator 方法。 每个请求限制为 100 个 tiIndicator。                                                                                                                                                                                                                    | 有关每个 [tiIndicator](../api/tiindicators-post.md) 的必填字段，请参阅创建 tiIndicator 方法。 每个请求限制为 100 个 tiIndicator。                                                     |
| [更新 tiIndicator](../api/tiindicator-update.md)              | 所需字段包括 `id` `expirationDateTime` `targetProduct` ：、、。 <br> 可编辑的字段包括 `action` `activityGroupNames` ：、、、、、、、、、、。 `additionalInformation` `confidence` `description` `diamondModel` `expirationDateTime` `externalId` `isActive` `killChain` `knownFalsePositives` `lastReportedDateTime` `malwareFamilyNames` `passiveOnly` `severity` `tags` `tlpLevel` | 所需字段包括 `id` `expirationDateTime` `targetProduct` ：、、。 <br> 可编辑的字段包括 `expirationDateTime` `severity` `description` ：、、。                                                                         |
| [更新 tiIndicator](../api/tiindicator-updatetiindicators.md) | 有关每个 [tiIndicator](../api/tiindicator-update.md) 的必需和可编辑字段，请参阅更新 tiIndicator 方法。                                                                                                                                                                                                                                                       | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |
| [删除 tiIndicator](../api/tiindicator-delete.md)              | 必填字段为 `id` ：。                                                                                                                                                                                                                                                                                                                                                            | 必填字段为 `id` ：。                                                                                                                                                                                             |
| [删除 tiIndicator](../api/tiindicator-deletetiindicators.md) | 有关每个 [tiIndicator](../api/tiindicator-delete.md) 的必填字段，请参阅上面的删除 tiIndicator 方法。                                                                                                                                                                                                                                                               | <p align="center">[提交问题](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p>                                                                                                             |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|action|string| 当 targetProduct 安全工具中的指示器匹配时要应用的操作。 可能的值是：`unknown`、`allow`、`block`、`alert`。 **必需。**|
|activityGroupNames|字符串集合|网络威胁情报名称 (威胁) 威胁指示器涵盖的恶意活动的各方提供。|
|additionalInformation|字符串|可以放置其他 tiIndicator 属性未覆盖的指示器的额外数据到的捕获区域。 放置在 additionalInformation 的数据通常不会由 targetProduct 安全工具使用。|
|azureTenantId|字符串| 在指标被启用时由系统标记。 提交Azure Active Directory的租户 ID。 **必需。**|
|confidence|Int32|表示指示器内数据准确识别恶意行为的置信度整数。 可接受的值为 0 – 100，100 为最高值。|
|说明|字符串| 简要 (表示的威胁) 少于 100 个字符。 **必需。**|
|diamondModel|[diamondModel](#diamondmodel-values)|存在此指示器的菱形模型区域。 可取值为：`unknown`、`adversary`、`capability`、`infrastructure`、`victim`。|
|expirationDateTime|DateTimeOffset| 指示指示器何时过期的 DateTime 字符串。 所有指示器都必须具有过期日期，以避免在系统中保留过时的指示器。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。 **必需。**|
|externalId|String| 将指示器与指示器提供程序的系统系统连接在一起 (标识号，例如外键) 。 |
|id|字符串|在指标被启用时由系统创建。 生成的 GUID/唯一标识符。 只读。|
|ingestedDateTime|DateTimeOffset| 在指标被启用时由系统标记。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|isActive|Boolean| 用于在系统内停用指示器。 默认情况下，提交的任何指示器都设置为活动。 但是，提供商可能会提交现有指示器（此设置为"False"）来停用系统指示器。|
|killChain|[killChain](#killchain-values) 集合|一个字符串的 JSON 数组，描述此指示器指向击杀链上的哪个点。 有关确切值，请参阅下面的"killChain 值"。 |
|knownFalsePositives|字符串|指示符可能导致误报的方案。 这应该是可读文本。|
|lastReportedDateTime|DateTimeOffset|上一次看到指示器的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|malwareFamilyNames|字符串集合|与指示器关联的恶意软件系列名称（如果存在）。 Microsoft 首选 Microsoft 恶意软件系列名称（如果可以通过安全智能威胁Windows Defender[找到）。](https://www.microsoft.com/wdsi/threats)|
|passiveOnly|Boolean |确定指示器是否应触发对最终用户可见的事件。 设置为"true"时，安全工具不会通知最终用户"点击"已发生。 这通常被安全产品视为审核或静默模式，在此模式下，安全产品只会记录发生匹配但不执行该操作。 默认值为 false。 |
|severity|Int32| 表示由指示器内的数据标识的恶意行为严重性的整数。 可接受的值为 0 – 5，其中 5 表示最严重，0 表示不严重。 默认值为 3。 |
|标记|字符串集合|存储任意标记/关键字的字符串的 JSON 数组。 |
|targetProduct|字符串|一个字符串值，表示应该应用指示器的单个安全产品。 可接受的值为 `Azure Sentinel` `Microsoft Defender ATP` ：、。 **Required**|
|threatType|[threatType](#threattype-values)| 每个指示器必须具有有效的指示器威胁类型。 可取值为：`Botnet`、`C2`、`CryptoMining`、`Darknet`、`DDoS`、`MaliciousUrl`、`Malware`、`Phishing`、`Proxy`、`PUA`、`WatchList`。 **必需。** |
|tlpLevel|[tlpLevel](#tlplevel-values)| 指示器的流量灯协议值。 可取值为：`unknown`、`white`、`green`、`amber`、`red`。 **必需。**|

### <a name="indicator-observables---email"></a>指示器可观测项 - 电子邮件

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|emailEncoding|字符串|电子邮件中使用的文本编码类型。|
|emailLanguage|字符串|电子邮件的语言。|
|emailRecipient|字符串|收件人电子邮件地址。|
|emailSenderAddress|字符串|攻击者或攻击者&#124;的电子邮件地址。|
|emailSenderName|字符串|攻击者和攻击者的&#124;名称。|
|emailSourceDomain|字符串|电子邮件中使用的域。|
|emailSourceIpAddress|字符串|电子邮件的源 IP 地址。|
|emailSubject|字符串|电子邮件的主题行。|
|emailXMailer|字符串|电子邮件中使用的 X-Mailer 值。|

### <a name="indicator-observables---file"></a>指示器可观测值 - 文件

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|编译文件时的日期/时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|fileCreatedDateTime|DateTimeOffset| 创建文件的 DateTime。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|fileHashType|string| 存储在 fileHashValue 中的哈希类型。 可取值为：`unknown`、`sha1`、`sha256`、`md5`、`authenticodeHash256`、`lsHash` 或 `ctph`。|
|fileHashValue|字符串| 文件哈希值。|
|fileMutexName|字符串| 基于文件的检测中使用的互斥名称。|
|fileName|String|如果指示器基于文件，则该文件的名称。 多个文件名可能用逗号分隔。 |
|filePacker|字符串|用于生成问题文件的打包程序。|
|filePath|字符串|指示泄露的文件的路径。 可能是一个Windows *nix 样式路径。|
|fileSize|Int64|文件大小（以字节为单位）。|
|fileType|字符串| 文件类型的文本说明。 例如，"Word Document"或"Binary"。|

### <a name="indicator-observables---network"></a>指示器可观测值 - 网络

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|domainName|String|与此指示器关联的域名。 应为 subdomain.domain.topleveldomain 格式 (例如，baddomain.domain.net) |
|networkCidrBlock|字符串| 此指示器中引用的网络的 CIDR 阻止表示法表示形式。 仅在无法标识 Source 和 Destination 时使用。 |
|networkDestinationAsn|Int32|指示器中引用的网络的目标自治系统标识符。|
|networkDestinationCidrBlock|字符串|CIDR 此指示器中目标网络的表示形式。|
|networkDestinationIPv4|字符串|IPv4 IP 地址目标。|
|networkDestinationIPv6|字符串|IPv6 IP 地址目标。|
|networkDestinationPort|Int32|TCP 端口目标。|
|networkIPv4|字符串| IPv4 IP 地址。 仅在无法标识 Source 和 Destination 时使用。 |
|networkIPv6|字符串| IPv6 IP 地址。 仅在无法标识 Source 和 Destination 时使用。 |
|networkPort|Int32| TCP 端口。 仅在无法标识 Source 和 Destination 时使用。 |
|networkProtocol|Int32|IPv4 标头中协议字段的小数表示形式。|
|networkSourceAsn|Int32|指示器中引用的网络的源自治系统标识符。|
|networkSourceCidrBlock|字符串|此指示器中源网络的 CIDR 阻止表示法表示|
|networkSourceIPv4|字符串|IPv4 IP 地址源。|
|networkSourceIPv6|字符串|IPv6 IP 地址源。|
|networkSourcePort|Int32|TCP 端口源。|
|url|String|统一资源定位器。 此 URL 必须符合 RFC 1738。|
|userAgent|字符串|User-Agent来自可能指示泄露的 Web 请求中的字符串。|

### <a name="diamondmodel-values"></a>diamondModel 值

有关此模型的信息，请参阅 [菱形模型](http://diamondmodel.org)。

| 成员 | 值 | 说明 |
|:-------|:----- |:------------|
| unknown |  0    | |
| 一对多 |  1    |该指示器描述对手。|
| capability |  2   |指示器是攻击者的一项功能。|
| 基础结构 | 3 |该指示器描述攻击者的基础结构。|
| 一个 | 4 |该标记描述攻击者的受攻击者。|
| unknownFutureValue | 127 | |

### <a name="killchain-values"></a>killChain 值

| 成员 | 说明 |
|:-------|:------------|
|操作|阻止攻击者利用受到威胁的系统采取分布式拒绝服务攻击等操作。|
|C2|表示处理损坏系统的控制通道。|
|传递|向攻击者分发攻击代码 (例如 USB、电子邮件、网站) 。|
|利用|利用漏洞的利用代码 (例如，代码执行) 。|
|安装|在漏洞被攻击后安装恶意软件。|
|侦查|指示器是活动组收集信息以用于未来攻击的证据。|
|武器化|将漏洞转换为攻击代码 (例如，恶意软件) 。|

### <a name="threattype-values"></a>threatType 值

| 成员 | 说明 |
|:-------|:------------|
|Botnet| 指示器详细介绍了 botnet 节点/成员。|
|C2|指示器详细说明了&网络"控件"节点的 Command 对象。|
|CryptoMining|涉及此网络地址/URL 的流量是 CyrptoMining / 资源滥用的指示。|
|深网|指示符是"深色网络"节点/网络的指示器。
|DDoS|与活动或即将进行的 DDoS 活动相关的指示器。|
|MaliciousUrl|提供恶意软件服务的 URL。|
|恶意软件|描述恶意文件或文件的指示器。|
|网络钓鱼|与网络钓鱼活动相关的指示器。|
|代理|指示符是代理服务指示器。|
|PUA|可能不需要的应用程序。|
|WatchList|这是一般存储桶，当无法确定威胁是什么或需要手动解释时，将放置指示器。 向系统中提交数据的合作伙伴通常不应使用此功能。|

### <a name="tlplevel-values"></a>tlpLevel 值

每个指示器在提交时还必须有一个交通灯协议值。 此值表示给定指示器的敏感度和共享范围。

| 成员 | 说明 |
|:-------|:------------|
|白色| 共享范围：无限制。 可以不受限制地自由共享指示器。|
|绿色| 共享范围：Community。 指示器可以与安全社区共享。|
|琥珀色| 共享范围：受限。 这是指示器的默认设置，将共享限制为仅"需要知道"为 1 个实施威胁情报 2) 客户的) 服务和服务运营商，其系统 () 显示与指示器一致的行为。|
|红色| 共享范围：个人。 这些指示器仅直接共享，最好在个人共享。 由于 TLP 红色指示器的预定义限制，因此通常不会进行使用。 如果提交 TLP 红色指示器，则"PassiveOnly"属性也应 `True` 设置为。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tiIndicator",
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
