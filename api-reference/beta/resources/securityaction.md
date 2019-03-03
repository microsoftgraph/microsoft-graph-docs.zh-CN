---
title: securityAction 资源类型
description: 立即采取行动以使用 Microsoft Graph Security securityAction 实体防御威胁。 当安全分析员发现新的指标 (如恶意文件、URL、域或 IP 地址) 时, 可以立即在 Microsoft 安全解决方案中启用保护。 调用特定提供程序的操作, 请参阅执行的所有操作, 并在需要时取消操作。 尝试使用 Windows Defender ATP 进行安全操作 (即将推出), 以阻止在调查过程中发现警报或标识的属性的 windows 终结点上的恶意活动。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 405f12c2cf484651f8bcefc791c9dd24dae410bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366985"
---
# <a name="securityaction-resource-type"></a>securityAction 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

立即采取行动以使用 Microsoft Graph Security securityAction 实体防御威胁。 当安全分析员发现新的指标 (如恶意文件、URL、域或 IP 地址) 时, 可以立即在 Microsoft 安全解决方案中启用保护。 调用特定提供程序的操作, 请参阅执行的所有操作, 并在需要时取消操作。 尝试使用[Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)进行安全操作 (即将推出), 以阻止在调查过程中发现警报或标识的属性的 windows 终结点上的恶意活动。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取 securityAction](../api/securityaction-get.md) | [securityAction](securityaction.md) | 读取 securityAction 对象的属性和关系。 |
| [创建 securityAction](../api/securityactions-post.md) | [securityAction](securityaction.md) | 通过发布到 securityActions 集合创建新的 securityAction。 |
| [列出 securityActions](../api/securityactions-list.md) | [securityAction](securityaction.md)集合 | 获取 securityAction 对象集合。 |
|[取消 securityAction](../api/securityaction-cancelsecurityaction.md)|无|取消安全操作。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|actionReason|String|调用此操作的原因。|
|appId|String|提交 (POST) 操作的调用应用程序的应用程序 ID。 应从身份验证令牌中提取 appId, 并且调用应用程序不手动输入该 appId。|
|azureTenantId|String|用于确定实体所属的租户的实体的 Azure 租户 ID (多租户支持)。 应从 auth 令牌中提取 azureTenantId, 而不是通过调用应用程序手动输入。|
|completedDateTime|DateTimeOffset|操作完成时的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|createdDateTime|DateTimeOffset|创建操作时的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|errorInfo|[resultInfo](resultinfo.md)| 操作失败时的错误消息。|
|id|字符串| 当操作为引入时由系统创建。 生成的 GUID/唯一标识符。 只读。|
|lastActionDateTime|DateTimeOffset| 上次更新此操作时的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时间。 例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|name|String| 操作名称。|
|参数|[keyValuePair](keyvaluepair.md) 集合| 调用操作所必需的参数 (键值对) 集合, 例如 URL 或 fileHash to block 等。 **Required**|
|市|[securityActionState](securityactionstate.md)集合|securityActionState 的集合, 以保留操作的历史记录。|
|status|string| 操作的状态。 可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。|
|user|String| 已提交 (POST) 操作的已登录用户的用户主体名称。 应从身份验证令牌中提取用户, 而不是通过调用应用程序手动输入。|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|包含有关安全产品/服务供应商、提供程序和子提供商的详细信息的复杂类型 (例如, 供应商 = Microsoft; 提供商 = Windows Defender ATP; 子提供程序 = AppLocker)。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->