---
title: printerCreateOperation 资源类型
description: 表示长时间运行的打印机注册操作。 派生自 printOperation。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 91a1d70afccf94abe1c611e696bc4349a59964e1dbb176cce0ddb8aa32dc287a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54169352"
---
# <a name="printercreateoperation-resource-type"></a>printerCreateOperation 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示长时间运行的打印机注册操作。 派生自 [printOperation](printoperation.md)。

继承自 [printOperation](printoperation.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
| [获取操作](../api/printoperation-get.md) | [printOperation](printoperation.md) | 在当前用户或应用的租户中检索长时间运行的操作。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|操作标识符。 只读。|
|status|[printOperationStatus](printoperationstatus.md)|注册操作的状态。 包含操作的进度以及是否成功完成。 只读。|
|createdDateTime|DateTimeOffset|创建操作时的日期时间Offset。 只读。|
|证书|String|在注册过程中创建的已签名证书。 只读。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|打印机|[打印机](printer.md)|创建的打印机实体。 只读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "baseType": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCreateOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)",
  "certificate": "String"
}
```

