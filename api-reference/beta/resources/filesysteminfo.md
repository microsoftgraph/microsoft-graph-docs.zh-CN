---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
ms.openlocfilehash: e2dfac79f5c7d511cab11c076d697940a01f4c7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524693"
---
# <a name="filesysteminfo-facet"></a>FileSystemInfo Facet

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 FileSystemInfo 资源包含设备本地文件系统所报告的项目本地版本的属性。和在本地设备上一样，此 facet 可用于指定项目的上次修改日期或创建日期。

可用于 [driveItem][item-resource] 资源的 fileSystemInfo 属性。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "lastAccessedDateTime"
  ],
  "@odata.type": "microsoft.graph.fileSystemInfo"
}-->

```json
{
  "createdDateTime" : "datetime",
  "lastAccessedDateTime": "datetime",
  "lastModifiedDateTime" : "datetime"
}
```

## <a name="properties"></a>属性

| 属性                 | 类型           | 说明                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| **createdDateTime**      | DateTimeOffset | 在客户端创建文件时的 UTC 日期和时间。                                                              |
| **lastAccessedDateTime** | DateTimeOffset | 上次访问文件时的 UTC 日期和时间。仅可用于最近的文件列表。 |
| **lastModifiedDateTime** | DateTimeOffset | 在客户端上次修改文件时的 UTC 日期和时间。                                                        |

## <a name="notes"></a>注意

来自 DriveItem 资源上同一属性的 createdDateTime 和 lastModifiedDateTime 值有所不同。DriveItem 资源上的值是从服务中所见的创建和修改的日期和时间。FileSystemInfo 资源中存储的值由客户端提供。

例如，如果星期一在设备上创建文件，但直到星期二才上载到服务，则上载文件的客户端应写入 `fileSystemInfo` facet，以包括星期一这一创建日期。检索项元数据时，项的创建日期将反映为星期二，但 `fileSystemInfo` facet 将显示星期一这一创建的原始创建日期。

这些属性为读/写。如果正在上载文件，并且知道这些字段的本地客户端值，则应该在请求中包括它们。

如果文件内容已更新且未提供这些属性，**lastModifiedDateTime** 将自动重置为当前时间。

## <a name="remarks"></a>注解

* **lastAccessedDateTime** 不适用于 SharePoint Online 或 OneDrive for Business 中的项。

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

[item-resource]: ../resources/driveitem.md

<!--
{
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo",
  "suppressions": [
    "Error: /api-reference/beta/resources/filesysteminfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
