---
title: cloudPcForensicStorageAccount 资源类型
description: 表示用于取证分析的云电脑存储帐户。
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ec722361b1d6fd1944ef22d32e2dbe38a5442741
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366305"
---
# <a name="cloudpcforensicstorageaccount-resource-type"></a>cloudPcForensicStorageAccount 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可用于存储云电脑的快照或快照以进行取证分析的存储帐户信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|storageAccountId|String|存储帐户的 ID。|
|storageAccountName|String|存储帐户的名称。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "storageAccountId",
  "@odata.type": "microsoft.graph.cloudPcForensicStorageAccount",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcForensicStorageAccount",
  "storageAccountId": "String",
  "storageAccountName": "String"
}
```
