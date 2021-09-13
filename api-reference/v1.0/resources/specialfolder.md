---
author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
ms.localizationpriority: medium
description: SpecialFolder 资源将与特殊文件夹相关的数据项分组到一个单一结构。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f8bef54bc709cb457bf30e0ce01e8a774d785cbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136341"
---
# <a name="specialfolder-resource-type"></a>SpecialFolder 资源类型

命名空间：microsoft.graph

**SpecialFolder** 资源将与特殊文件夹相关的数据项分组到一个单一结构。

如果 **DriveItem** 具有一个非 null **specialFolder** facet，则该项表示特殊（命名的）文件夹。
可直接通过 [special folders 集合](../api/drive-get-specialfolder.md) 访问特殊文件夹。

特殊文件夹可提供简单别名，因此无需按路径查找（需要本地化）文件夹或通过 ID 引用文件夹来访问已知文件夹。如果特殊文件夹被重命名或移到驱动器中的其他位置，此语法将继续返回该文件夹。

应用程序第一次尝试向特殊文件夹中写入内容时，如果特殊文件夹不存在，系统会自动创建特殊文件夹。如果用户删除某个特殊文件夹，再次向其写入内容时会重新创建特殊文件夹。

**注意：** 如果应用仅请求 **Files.Read** 范围，而请求特殊文件夹不存在，则响应将是 `403 Forbidden` 错误。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a>属性

| 属性  | 类型   | 说明                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| name      | string | 此项在 `/drive/special` 集合中的唯一标识符。 |

## <a name="special-folders"></a>特殊文件夹

以下是 OneDrive 个人版和 OneDrive for Business 中可用的特殊文件夹。

| 名称        | 文件夹 ID    | 说明                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| App Root    | `approot`    | 应用程序的个人文件夹。通常位于 `/Apps/{Application Name}` 中 |
| Camera Roll | `cameraroll` | 本机照片备份文件夹。不适用于 OneDrive for Business。   |
| Documents   | `documents`  | “文档”文件夹。                                                    |
| Music       | `music`      | 音乐文件夹。不适用于 OneDrive for Business。                |
| Photos      | `photos`     | “照片”文件夹。                                                       |

## <a name="remarks"></a>注解 

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->

