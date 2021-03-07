---
title: printConnector 资源类型
description: 表示已使用通用打印订阅注册的打印连接器。 printConnector 资源可用于查看连接器状态和更新属性。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: e791ca755b695fc8e4704b65aff98a9db934d901
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517197"
---
# <a name="printconnector-resource-type"></a>printConnector 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示已使用通用打印订阅注册的打印连接器。 printConnector 资源可用于查看连接器状态和更新属性。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
| [Get connector](../api/printconnector-get.md) | [printConnector](printconnector.md) | 读取连接器对象的属性和关系。 |
| [更新连接器](../api/printconnector-update.md) | [printConnector](printconnector.md) | 更新连接器对象。 |
| [删除连接器](../api/printconnector-delete.md) | 无 | 从通用打印服务中注销连接器。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| 只读。|
|displayName|String|连接器的名称。|
|fullyQualifiedDomainName|String|连接器计算机主机名。|
|operatingSystem|String|连接器计算机的操作系统版本。|
|appVersion|String|连接器的版本。|
|位置|[printerLocation](printerlocation.md)|连接器的物理和/或组织位置。|
|registeredDateTime|DateTimeOffset|连接器注册时的日期/时间Offset。|
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