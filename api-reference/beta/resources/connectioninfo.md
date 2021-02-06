---
title: connectionInfo 资源类型
description: connectionInfo 对象定义用于与资源通信的连接信息。
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 454dc7fcd045bb91819b39ad30f603191bab8380
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137714"
---
# <a name="connectioninfo-resource-type"></a>connectionInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

connectionInfo 对象定义用于与 Azure AD 权利管理中的资源通信的资源定位器。

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
