---
title: printConnector 资源类型
description: 表示已使用通用打印订阅注册的打印连接器。 printConnector 资源可用于查看连接器状态和更新属性。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 184a2bc57252b3190754a4eb61e8415114a3c8d0
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945010"
---
# <a name="printconnector-resource-type"></a>printConnector 资源类型

命名空间：microsoft.graph

表示已使用通用打印订阅注册的打印连接器。 printConnector 资源可用于查看连接器状态和更新属性。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [List connectors](../api/print-list-connectors.md) | [printConnector](printconnector.md) | 检索打印连接器的列表。 |
| [Get connector](../api/printconnector-get.md) | [printConnector](printconnector.md) | 读取 connector 对象的属性和关系。 |
| [更新连接器](../api/printconnector-update.md) | [printConnector](printconnector.md) | 更新连接器对象。 |
| [删除连接器](../api/printconnector-delete.md) | 无 | 从通用打印服务注销连接器。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| 只读。|
|displayName|String|连接器的名称。|
|fullyQualifiedDomainName|String|连接器计算机主机名。|
|operatingSystem|String|连接器计算机的操作系统版本。|
|appVersion|String|连接器的版本。|
|位置|[printerLocation](printerlocation.md)|连接器的物理和/或组织位置。|
|registeredDateTime|DateTimeOffset|注册连接器时的日期时间Offset。|
|registeredBy|[userIdentity](useridentity.md)|注册连接器的用户。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printConnector",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "fullyQualifiedDomainName": "String",
  "operatingSystem": "String",
  "appVersion": "String",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "registeredDateTime": "String (timestamp)"
}
```
