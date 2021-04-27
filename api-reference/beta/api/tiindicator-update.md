---
title: 更新 tiIndicator
description: 更新 tiIndicator 对象的属性。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 6cb7f92d2a9d6c69b8daba94fddd2229beeab839
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050785"
---
# <a name="update-tiindicator"></a>更新 tiIndicator

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [tiIndicator 对象](../resources/tiindicator.md) 的属性。

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
| Authorization | Bearer {code} **必填** |
|Prefer | return=representation |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。 所需字段包括 `id` `expirationDateTime` `targetProduct` ：、、。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|action|string| 当 targetProduct 安全工具中的指示器匹配时要应用的操作。 可取值为：`unknown`、`allow`、`block`、`alert`。|
|activityGroupNames|字符串集合|网络威胁情报名称 (威胁) 威胁指示器涵盖的恶意活动的各方提供。|
|additionalInformation|String|可以放置其他 tiIndicator 属性未覆盖的指示器的额外数据到的捕获区域。 放置在 additionalInformation 的数据通常不会由 targetProduct 安全工具使用。|
|confidence|Int32|表示指示器内数据准确识别恶意行为的置信度整数。 可接受的值为 0 – 100，100 为最高值。|
|说明|String|简要 (指示器所代表的威胁) 少于 100 个字符。|
|diamondModel|[diamondModel](../resources/tiindicator.md#diamondmodel-values)|存在此指示器的菱形模型区域。 可取值为：`unknown`、`adversary`、`capability`、`infrastructure`、`victim`。|
|expirationDateTime|DateTimeOffset| 指示指示器何时过期的 DateTime 字符串。 所有指示器都必须具有过期日期，以避免在系统中保留过时的指示器。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`。|
|externalId|String|将指示器与指示器提供程序的系统连接在一起 (标识号，例如外键) 。|
|isActive|布尔值|用于在系统内停用指示器。 默认情况下，提交的任何指示器都设置为活动。 但是，提供商可能会提交现有指示器（此设置为"False"）来停用系统指示器。|
|killChain|[killChain](../resources/tiindicator.md#killchain-values) 集合|一个字符串的 JSON 数组，描述此指示器指向击杀链上的哪个点。 有关确切值，请参阅下面的"killChain 值"。|
|knownFalsePositives|String|指示符可能导致误报的方案。 这应该是可读文本。|
|lastReportedDateTime|DateTimeOffset|上一次看到指示器的时间。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`2014-01-01T00:00:00Z`|
|malwareFamilyNames|字符串集合|与指示器关联的恶意软件系列名称（如果存在）。 Microsoft 首选 Microsoft 恶意软件系列名称（如果可以通过安全智能威胁Windows Defender[找到）。](https://www.microsoft.com/wdsi/threats)|
|passiveOnly|布尔值|确定指示器是否应触发对最终用户可见的事件。 设置为"true"时，安全工具不会通知最终用户"点击"已发生。 这通常被安全产品视为审核或静默模式，在此模式下，安全产品只会记录发生匹配的情况，但不执行该操作。 默认值为 false。|
|severity|Int32|表示由指示器内的数据标识的恶意行为严重性的整数。 可接受的值为 0 – 5，其中 5 表示最严重，0 表示不严重。 默认值为 3。|
|tags|字符串集合|存储任意标记/关键字的字符串的 JSON 数组。|
|tlpLevel|[tlpLevel](../resources/tiindicator.md#tlplevel-values)| 指示器的流量光协议值。 可取值为：`unknown`、`white`、`green`、`amber`、`red`。|


## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

如果使用可选请求标头，则该方法在响应正文中返回 响应代码和更新的 `200 OK` [tiIndicator](../resources/tiindicator.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-request-without-prefer-header"></a>示例 1：不带 Prefer 标头的请求

#### <a name="request"></a>请求

下面是一个没有 标头的请求 `Prefer` 示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_1"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-1-java-snippets.md)]
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

### <a name="example-2-request-with-prefer-header"></a>示例 2：具有 Prefer 标头的请求

#### <a name="request"></a>请求

下面是包含 标头的请求 `Prefer` 示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator_2"
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-tiindicator-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-tiindicator-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-tiindicator-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-tiindicator-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

> [!NOTE]
> 为了提高可读性，可能缩短了此处显示的响应对象。

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


