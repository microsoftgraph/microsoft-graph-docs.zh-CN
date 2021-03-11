---
title: securityAction 资源类型
description: 利用 Microsoft Graph 安全性 securityAction 实体立即采取行动来抵御威胁。 当安全分析师发现新的指示器（如恶意文件、URL、域或 IP 地址）时，可立即在你的 Microsoft 安全解决方案中启用保护。 针对特定提供商采取操作，查看所采取的全部操作，还可在需要时取消操作。 请通过 Windows Defender ATP（即将推出）尝试安全操作，以使用在警报中看到或在调查期间确定的属性来阻止 Windows 终结点上的恶意活动。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: c1adeb6ee5ab3b3ad2165e854b2812e39b8df5ab
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720625"
---
# <a name="securityaction-resource-type"></a>securityAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

利用 Microsoft Graph 安全性 securityAction 实体立即采取行动来抵御威胁。 当安全分析师发现新的指示器（如恶意文件、URL、域或 IP 地址）时，可立即在你的 Microsoft 安全解决方案中启用保护。 针对特定提供商采取操作，查看所采取的全部操作，还可在需要时取消操作。 请通过 [Windows Defender ATP](/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) 尝试安全操作，以使用在警报中看到或在调查期间确定的属性来阻止 Windows 终结点上的恶意活动。

  > **注意：** 安全操作当前仅支持应用程序权限。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取安全操作](../api/securityaction-get.md) | [securityAction](securityaction.md) | 读取 securityAction 对象的属性和关系。 |
| [创建安全操作](../api/securityactions-post.md) | [securityAction](securityaction.md) | 通过发布到 securityActions 集合创建新的 securityAction。 |
| [列出安全操作](../api/securityactions-list.md) | [securityAction](securityaction.md) 集合 | 获取 securityAction 对象集合。 |
|[取消安全操作](../api/securityaction-cancelsecurityaction.md)|无|取消安全操作。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|actionReason|String|调用此操作的原因。|
|appId|String|在 POST 中提交的调用应用程序 (ID) 操作。 appId 应从身份验证令牌中提取，调用应用程序不应手动输入。|
|azureTenantId|字符串|实体的 Azure 租户 ID，用于确定实体属于 (租户支持) 。 azureTenantId 应从身份验证令牌中提取，调用应用程序不应手动输入。|
|completedDateTime|DateTimeOffset|操作完成时时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|createdDateTime|DateTimeOffset|创建操作时时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|errorInfo|[resultInfo](resultinfo.md)| 操作失败时的错误信息。|
|id|String| 在操作被启用时由系统创建。 生成的 GUID/唯一标识符。 只读。|
|lastActionDateTime|DateTimeOffset| 上次更新此操作的时间戳。 时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|name|String| 操作名称。|
|parameters|[keyValuePair](keyvaluepair.md) 集合| 参数集合 (键值对) 操作所必需的，例如要阻止的 URL 或 fileHash 等) 。 **必需**|
|状态|[securityActionState](securityactionstate.md) 集合|securityActionState 集合，以保留操作历史记录。|
|状态|string| 操作的状态。 可取值为：`NotStarted`、`Running`、`Completed`、`Failed`。|
|user|String| 在 POST 中提交的已登录用户的用户主体 () 操作。 用户应从身份验证令牌中提取，而不是由调用应用程序手动输入。|
|vendorInformation|[securityVendorInformation](securityvendorinformation.md)|复杂类型，包含有关安全产品/服务供应商、提供程序和子 (的详细信息，例如 vendor=Microsoft;provider=Windows Defender ATP;sub-provider=AppLocker) 。|

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
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