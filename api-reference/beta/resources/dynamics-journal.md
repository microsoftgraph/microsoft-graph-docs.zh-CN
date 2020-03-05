---
title: 日记资源类型
description: Dynamics 365 Business Central 中的日记。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 041de72a3372fd80063b96ba73d10272247c4fdb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503745"
---
# <a name="journal-resource-type"></a>日记资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Dynamics 365 Business Central 中的日记。

## <a name="methods"></a>方法

| 方法                                            |返回类型|说明    |
|:--------------------------------------------------|:----------|:--------------|
|[获取分类账](../api/dynamics-journal-get.md)      |日志    |获取日记。   |
|[过帐日记](../api/dynamics-create-journal.md)  |日志    |创建日记。|
|[修补程序日记](../api/dynamics-journal-update.md) |日志    |更新日记。|
|[删除分类账](../api/dynamics-journal-delete.md)|无       |删除日记。|

## <a name="properties"></a>属性
| 属性           | 类型                  |说明                                           |
|:-------------------|:----------------------|:-----------------------------------------------------|
|id                  |GUID                   |日记的唯一 ID。 不可编辑。           |
|code                |字符串，最大值为10| 日记的代码。                             |
|displayName         |字符串，最大大小为50| 日记的显示名称。                     |
|lastModifiedDateTime|datetime               |日记已修改的最后一个日期/时间。 只读。|

## <a name="bound-actions"></a>绑定操作
日记资源类型提供一个调用`post`的绑定操作，该操作将发布相应的常规日记批处理。

下面的示例演示了如何过帐常规日记批处理：  
`POST https://graph.microsoft.com/beta/financials/companies{id}/journals{id}/post`.

响应没有内容;响应代码为204。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。


```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "lastModifiedDateTime": "datetime"
}
```

