---
title: driveItemUploadableProperties 资源类型
description: DriveItemUploadableProperties 资源表示在创建上载会话时要上载的项。
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: c05c69f0cf72f74913882ddbf75355dc37592584
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032717"
---
# <a name="driveitemuploadableproperties-resource-type"></a>driveItemUploadableProperties 资源类型

命名空间：microsoft.graph

表示在 [创建上载会话](../api/driveitem-createuploadsession.md)时要上载的项。

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

