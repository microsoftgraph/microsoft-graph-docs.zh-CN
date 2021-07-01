---
title: driveItemUploadableProperties 资源类型
description: driveItemUploadableProperties 资源表示创建上载会话时要上载的项目。
localization_priority: Normal
author: JeremyKelley
ms.prod: sites-and-lists
doc_type: resourcePageType
ms.openlocfilehash: 6c00270f1e86e2bb8f44af36c6c514c9b80a647d
ms.sourcegitcommit: 0adbbcbc65b6acab80e9195f13321055994f56be
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2021
ms.locfileid: "53236206"
---
# <a name="driveitemuploadableproperties-resource-type"></a>driveItemUploadableProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**driveItemUploadableProperties** 资源表示创建上传会话时 [上传的项](../api/driveitem-createuploadsession.md)。

## <a name="properties"></a>属性

| 属性     | 类型                              | 说明                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|说明   |String                             | 提供项的用户可见的说明。 读写。 仅在个人OneDrive上。             |
|driveItemSource| [driveItemSource](driveItemSource.md)              | 有关驱动器项源的信息。 读写。 仅在 OneDrive for Business 和 SharePoint。  |
|fileSize      |Int64                              | 提供在上载之前执行配额检查的预期文件大小。 仅在个人OneDrive上。 |
|fileSystemInfo|[fileSystemInfo](filesysteminfo.md)| 客户端上的文件系统信息。读写。                                                      |
|mediaSource  | [mediaSource](mediaSource.md)                    | 媒体源信息。 读写。 仅在 OneDrive for Business 和 SharePoint。                 |
|name          |String                             | 项目名称（文件名和扩展名）。读写。                                          |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.driveItemUploadableProperties",
  "baseType": null
}-->

```json
{
  "description": "String",
  "fileSize": 1024,
  "fileSystemInfo": {"@odata.type": "microsoft.graph.fileSystemInfo"},
  "name": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

