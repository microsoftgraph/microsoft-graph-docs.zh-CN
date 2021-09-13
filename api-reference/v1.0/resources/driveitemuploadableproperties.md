---
title: driveItemUploadableProperties 资源类型
description: driveItemUploadableProperties 资源表示创建上载会话时要上载的项目。
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: bedbdbd67010352c3bc69a743e355efaf0514409
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067463"
---
# <a name="driveitemuploadableproperties-resource-type"></a>driveItemUploadableProperties 资源类型

命名空间：microsoft.graph

表示创建上传会话 [时上传的项目](../api/driveitem-createuploadsession.md)。

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

## <a name="properties"></a>属性

| 属性     | 类型                              | 说明                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|**description**   |String                             | 提供项的用户可见的说明。 读写。 仅在个人OneDrive上。             |
|**fileSize**      |Int64                              | 提供在上载之前执行配额检查的预期文件大小。 仅在个人OneDrive上。 |
|**fileSystemInfo**|[fileSystemInfo](filesysteminfo.md)| 客户端上的文件系统信息。读写。                                                      |
|**name**          |String                             | 项目名称（文件名和扩展名）。读写。                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

