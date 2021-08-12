---
title: 配置资源类型
description: 指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加应用程序 ID。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 213c24c9388f555d772f2c0243b1d55d023239922d059b63478a8953ac6d5b25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141670"
---
# <a name="configuration-resource-type"></a>配置资源类型

命名空间：microsoft.graph.externalConnectors



指定允许管理 externalConnection 和为 externalConnection 中的内容编制索引的附加[应用程序 ID。](../resources/externalconnectors-externalconnection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|authorizedAppIds|String collection|允许管理 externalConnection 和为 externalConnection 中的内容编制索引的已注册 Azure Active Directory 应用程序的应用程序 ID 的集合。|

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

