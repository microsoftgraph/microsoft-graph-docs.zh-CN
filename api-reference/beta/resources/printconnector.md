---
title: printConnector 资源类型
description: 表示已使用通用打印订阅注册的打印连接器。 printConnector 资源可用于查看连接器状态和更新属性。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c482d17cd702751f5f2cd2b8cff5e34166fb2075
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176910"
---
# <a name="printconnector-resource-type"></a>printConnector 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示已使用通用打印订阅注册的打印连接器。 printConnector 资源可用于查看连接器状态和更新属性。

## <a name="methods"></a>方法

| 方法       | 返回类型 | Description |
|:-------------|:------------|:------------|
| [List connectors](../api/print-list-connectors.md) | [printConnector](printconnector.md) | 检索打印连接器的列表。 |
| [Get connector](../api/printconnector-get.md) | [printConnector](printconnector.md) | 读取连接器对象的属性和关系。 |
| [更新连接器](../api/printconnector-update.md) | [printConnector](printconnector.md) | 更新连接器对象。 |
| [删除连接器](../api/printconnector-delete.md) | 无 | 从通用打印服务注销连接器。 |

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|id|String| 只读。|
|displayName|String|连接器的名称。|
|fullyQualifiedDomainName|String|连接器计算机的主机名。|
|operatingSystem|String|连接器计算机的操作系统版本。|
|appVersion|字符串|连接器的版本。|
|deviceHealth|[deviceHealth](devicehealth.md)|连接器的设备运行状况。|
|位置|[printerLocation](printerlocation.md)|连接器的物理位置和/或组织位置。|
|registeredDateTime|DateTimeOffset|注册连接器时的 DateTimeOffset。|
|registeredBy|[userIdentity](useridentity.md)|注册连接器的用户。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printConnector"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "deviceHealth": {"@odata.type": "microsoft.graph.deviceHealth"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "registeredDateTime": "String (timestamp)",
  "registeredBy": {"@odata.type": "microsoft.graph.userIdentity"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printConnector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


