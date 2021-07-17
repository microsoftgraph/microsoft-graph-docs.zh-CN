---
title: 配置资源类型
description: 指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加应用程序 ID。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cd8f4ad66a80873d24f6ed14785e1f24d88077c4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467277"
---
# <a name="configuration-resource-type"></a>配置资源类型

命名空间：microsoft.graph.externalConnectors



指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加[应用程序 ID。](../resources/externalconnectors-externalconnection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authorizedAppIds|字符串集合|允许管理 externalConnection 和为 externalConnection 中的内容编制索引的已注册 Azure Active Directory 应用程序的应用程序 ID 的集合。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.configuration"
}
-->
``` json
{
  "authorizedAppIds": [
    "String"
  ]
}
```

