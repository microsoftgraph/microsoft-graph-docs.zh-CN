---
title: connectionInfo 资源类型
description: connectionInfo 对象定义用于与资源通信的连接信息。
author: hanki-microsoft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4c00cf41bd89deebf4b1453cb4f7389094e3dcb8
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242307"
---
# <a name="connectioninfo-resource-type"></a>connectionInfo 资源类型

命名空间：microsoft.graph


connectionInfo 对象定义用于与权利管理中的资源Azure AD定位器。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|url|String|授权管理用于与访问包资源通信的终结点。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.connectionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectionInfo",
  "url": "String"
}
```


