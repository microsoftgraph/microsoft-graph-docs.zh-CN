---
title: 公司资源类型
description: Dynamics 365 Business Central 中的公司。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 13bc765f873bc893925ffbddc82b2f0685376cf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505138"
---
# <a name="companies-resource-type"></a>公司资源类型

命名空间： microsoft. graph

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


