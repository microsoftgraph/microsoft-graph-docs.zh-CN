---
title: driveItemUploadableProperties 资源类型
description: DriveItemUploadableProperties 资源表示在创建上载会话时要上载的项。
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 1f3ef83f36af70aa2efd3cce8d0215d705114e50
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863871"
---
# <a name="driveitemuploadableproperties-resource-type"></a>driveItemUploadableProperties 资源类型

命名空间：microsoft.graph

表示在[创建上载会话](../api/driveitem-createuploadsession.md)时要上载的项。

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
|**description**   |String                             | 提供项的用户可见的说明。 读写。 仅适用于 OneDrive 个人版。             |
|**fileSize**      |Int64                              | 提供在上载前执行配额检查所需的文件大小。 仅适用于 OneDrive 个人版。 |
|**fileSystemInfo**|[fileSystemInfo](filesysteminfo.md)| File system information on client. Read-write.                                                      |
|**name**          |String                             | The name of the item (filename and extension). Read-write.                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->
