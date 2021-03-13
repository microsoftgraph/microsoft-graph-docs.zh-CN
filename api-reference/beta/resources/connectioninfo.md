---
title: connectionInfo 资源类型
description: connectionInfo 对象定义用于与资源通信的连接信息。
author: hanki-microsoft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8bbab1e93cf5af0fcfbd401b6b726f3165f595b4
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761815"
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
