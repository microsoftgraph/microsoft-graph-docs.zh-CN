---
title: 公司资源类型
description: Dynamics 365 Business Central 中的公司。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 3fedbd9407a4124c38a6ff08a95dbf4cd22c9fe1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081760"
---
# <a name="companies-resource-type"></a>公司资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 "Dynamics 365 Business Central 中的公司" 资源类型。 

## <a name="methods"></a>方法

| 方法         | 返回类型  |说明|
|:---------------|:-------------|:----------|
|[获取公司](../api/dynamics-companies-get.md)|companies|获取公司。|

## <a name="properties"></a>属性
| 属性        | 类型 |说明                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |公司的唯一 ID。 只读。|
|name             |string|指定公司。                  |
|displayName      |string|指定公司显示名称。     |
|systemVersion    |string|指定公司的内部版本。|
|businessProfileId|string|指定链接到公司的业务配置文件 ID。|


## <a name="relationships"></a>关系
无

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




