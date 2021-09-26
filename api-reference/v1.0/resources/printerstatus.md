---
title: printerStatus 资源类型
description: 表示打印机的处理状态，包括任何错误。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 67bdf6ebd458fd6e5ebe239ec057a682c53c78bf
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765508"
---
# <a name="printerstatus-resource-type"></a>printerStatus 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

表示打印机的处理状态，包括任何错误。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|state|printerProcessingState|当前处理状态。 下表介绍了有效值。 只读。|
|详细信息|printerProcessingStateDetail 集合|描述打印机为何当前状态的详细信息列表。 下表介绍了有效值。 只读。|
|说明|String|打印机当前处理状态可读的说明。 只读。|

### <a name="printerprocessingstate-values"></a>printerProcessingState 值

|成员|值|说明|
|:---|:---|:---|
|unknown|0|打印机报告的处理状态未知。|
|idle|1|打印机处于空闲状态并准备接受新的打印作业。|
|processing|2|打印机当前正在处理打印作业，并且将在完成时处理所有挂起的作业。|
|已停止|3|打印机遇到问题 (例如，活动纸盒中的纸张) 无法继续当前打印作业，直到问题得到解决。 有关详细信息 **，** 请参阅 (的详细信息) **或说明** 值。|
|unknownFutureValue|4 |可发展枚举 sentinel 值。 请勿使用。|

### <a name="printerprocessingstatedetail-values"></a>printerProcessingStateDetail 值

[printerProcessingStateDetail 枚举类型](./printerprocessingstatedetail.md)

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerStatus",
  "state": "String",
  "details": [
    "String"
  ],
  "description": "String"
}
```
