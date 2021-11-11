---
title: companies 资源类型
description: Dynamics 365 Business Central 中的一家公司。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 8230e7aca8b222c54656845c0e52d4fc60bc7abd
ms.sourcegitcommit: 6b5bee1a1cea92c1f3d6439110c4916eb8b249a5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/11/2021
ms.locfileid: "60908571"
---
# <a name="companies-resource-type"></a>companies 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Dynamics 365 Business Central 中的公司资源类型。 

## <a name="methods"></a>Methods

| 方法         | 返回类型  |Description|
|:---------------|:-------------|:----------|
|[获取公司](../api/dynamics-companies-get.md)|companies|获取公司。|

## <a name="properties"></a>属性
| 属性        | 类型 |说明                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |公司的唯一 ID。 只读。|
|name             |string|指定 Company。                  |
|displayName      |string|指定公司显示名称。     |
|systemVersion    |string|指定公司的内部版本。|
|businessProfileId|string|指定链接到公司的业务配置文件 ID。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是公司的 JSON 表示形式。

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}
```




