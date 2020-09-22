---
title: 更新 tiIndicator
description: 更新 tiIndicator 对象的属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 6f6adcc3e4f069297fd0b22dee24a33331d040cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076508"
---
# <a name="update-tiindicator"></a>更新 tiIndicator

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [tiIndicator](../resources/tiindicator.md) 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | ThreatIndicators.ReadWrite.OwnedBy |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | **必需**的持有者 {代码} |
|Prefer | return = 表示形式 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。 必填字段为： `id` 、 `expirationDateTime` 、 `targetProduct` 。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|action|string| 在 targetProduct 安全工具中匹配指标时要应用的操作。 可取值为：`unknown`、`allow`、`block`、`alert`。|
|activityGroupNames|String 集合|负责威胁指示器所涵盖的恶意活动的各方) 的网络威胁智能名称 (s。|
|additionalInformation|String|可以放置其他 tiIndicator 属性中未涵盖的指标中的额外数据的 "容器" 区域。 放置在 additionalInformation 中的数据通常不会被 targetProduct 安全工具使用。|
|confidence|Int32|一个整数，表示对指示器中的数据准确标识恶意行为的可信度。 可接受的值为0–100，100的值为最高。|
|说明|String|由指示器表示的威胁 (100 个字符或更少) 的简短说明。|
|diamondModel|[diamondModel](#diamondmodel-values)|此指示器所在的菱形模型的面积。 可取值为：`unknown`、`adversary`、`capability`、`infrastructure`、`victim`。|
|expirationDateTime|DateTimeOffset| 指示指示器过期时间的日期/时间字符串。 所有指标都必须具有到期日期，以避免系统中的陈旧指示器持久化。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。|
|externalId|String|将指示器与指示器提供程序的系统相结合的标识号 (例如，外键) 。|
|isActive|Boolean|用于停用系统中的指示器。 默认情况下，提交的任何指示器都设置为活动状态。 但是，提供程序可能会将此设置为 "False" 的现有指示器提交到系统中停用指示器。|
|killChain|[killChain](#killchain-values) 集合|一个 JSON 字符串数组，用于描述此指示器针对终止链上的哪个点或点。 有关确切值，请参阅下面的 "killChain 值"。|
|knownFalsePositives|String|指示符可能导致误报的情况。 这应该是可读的文本。|
|lastReportedDateTime|DateTimeOffset|上次发现指示器的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`|
|malwareFamilyNames|String 集合|与指示器关联的恶意软件系列名称（如果存在）。 如果所有可能都可以通过 Windows Defender 安全智能 [威胁百科全书](https://www.microsoft.com/wdsi/threats)找到，microsoft 将首选 microsoft 恶意软件系列名称。|
|passiveOnly|Boolean|确定该指示符是否应触发对最终用户可见的事件。 如果设置为 "true"，则安全工具将不会通知最终用户已发生 "命中"。 通常情况下，这通常被视为审核或静默模式，安全产品只需记录已发生的匹配项，但不会执行该操作。 默认值为 false。|
|severity|Int32|一个整数，表示由指示器中的数据标识的恶意行为的严重程度。 可接受的值为0–5，其中5为最严重，0表示根本不严重。 默认值为3。|
|tags|String 集合|存储任意标记/关键字的字符串的 JSON 数组。|
|tlpLevel|[tlpLevel](#tlplevel-values)| 指标的流量灯协议值。 可取值为：`unknown`、`white`、`green`、`amber`、`red`。|

### <a name="diamondmodel-values"></a>diamondModel 值

有关此模型的信息，请参阅 [菱形模型](http://diamondmodel.org)。

| 值 | 说明 |
|:-------|:------------|
|对手|该指示器描述了敌人。|
|性能|该指标是入侵者的一种功能。|
|基本|此指标介绍了入侵者的基础结构。|
|者|该指标描述敌人的牺牲品。|

### <a name="killchain-values"></a>killChain 值

| 值 | 说明 |
|:-------|:------------|
|操作|代表 "针对目标的操作"。 攻击者利用受攻击的系统执行诸如分布式拒绝服务攻击之类的操作。|
|C2|表示操纵受损系统时所使用的控制通道。|
|Delivery|将攻击代码分发给受害者的过程 (例如，USB、电子邮件、网站) 。|
|具备|利用漏洞的攻击代码 (例如，代码执行) 。|
|安装|在漏洞受到攻击后安装恶意软件。|
|侦查|指标是活动组收集信息以用于将来的攻击的证据。|
|Weaponization|将漏洞变成攻击代码 (例如，恶意软件) 。|

### <a name="tlplevel-values"></a>tlpLevel 值

每个指示器在提交时都必须有流量灯协议 (tlp) 值。 此值表示给定指标的敏感度和共享作用域。

| 值 | 说明 |
|:-------|:------------|
|白色| 共享范围：无限制。 指示器可以自由共享，无需限制。|
|绿色| 共享作用域：社区。 指标可与安全社区共享。|
|亮| 共享作用域：受限。 这是指示器的默认设置，并且仅将共享限制为仅有需要了解的内容： 1) 服务和实施威胁智能的服务运算符;2) 其系统 (s) 表现为与指示器一致的行为的客户。|
|红色| 共享作用域：个人。 这些指标仅可直接共享，最好是人员。 通常情况下，TLP 红色指示器不会引入，因为其预定义限制。 如果提交了 TLP 红色指示器，则 **passiveOnly** 属性也应设置为 `True` 。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

如果使用可选请求标头，则该方法将 `200 OK` 在响应正文中返回响应代码和更新的 [tiIndicator](../resources/tiindicator.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-request-without-prefer-header"></a>示例1：不带首选标头的请求

#### <a name="request"></a>请求

以下是不带标头的请求示例 `Prefer` 。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>示例2：具有首选标头的请求

#### <a name="request"></a>请求

以下是包含标头的请求的示例 `Prefer` 。

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a>响应

下面展示了示例响应。

> [!NOTE]
> 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


