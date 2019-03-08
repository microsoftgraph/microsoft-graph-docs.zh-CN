---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: FileSystemInfo
localization_priority: Normal
ms.openlocfilehash: 65bbd2e371c856a6ffbd2c55ecba88c1635ce41c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480283"
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="2e946-102">FileSystemInfo Facet</span><span class="sxs-lookup"><span data-stu-id="2e946-102">FileSystemInfo facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e946-p101">**FileSystemInfo** 资源包含设备本地文件系统所报告的项目本地版本的属性。和在本地设备上一样，此 facet 可用于指定项目的上次修改日期或创建日期。</span><span class="sxs-lookup"><span data-stu-id="2e946-p101">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="2e946-105">可用于 [driveItem][item-resource] 资源的 fileSystemInfo 属性。</span><span class="sxs-lookup"><span data-stu-id="2e946-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e946-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e946-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2e946-107">属性</span><span class="sxs-lookup"><span data-stu-id="2e946-107">Properties</span></span>

| <span data-ttu-id="2e946-108">属性</span><span class="sxs-lookup"><span data-stu-id="2e946-108">Property</span></span>                 | <span data-ttu-id="2e946-109">类型</span><span class="sxs-lookup"><span data-stu-id="2e946-109">Type</span></span>           | <span data-ttu-id="2e946-110">说明</span><span class="sxs-lookup"><span data-stu-id="2e946-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2e946-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="2e946-111">**createdDateTime**</span></span>      | <span data-ttu-id="2e946-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e946-112">DateTimeOffset</span></span> | <span data-ttu-id="2e946-113">在客户端创建文件时的 UTC 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e946-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="2e946-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2e946-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="2e946-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e946-115">DateTimeOffset</span></span> | <span data-ttu-id="2e946-116">上次访问文件时的 UTC 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e946-116">The UTC date and time the file was last accessed.</span></span> <span data-ttu-id="2e946-117">仅可用于[最近的文件列表](../api/drive-recent.md)。</span><span class="sxs-lookup"><span data-stu-id="2e946-117">Available for the [recent file list](../api/drive-recent.md) only.</span></span> |
| <span data-ttu-id="2e946-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2e946-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="2e946-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e946-119">DateTimeOffset</span></span> | <span data-ttu-id="2e946-120">在客户端上次修改文件时的 UTC 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e946-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="2e946-121">注意</span><span class="sxs-lookup"><span data-stu-id="2e946-121">Notes</span></span>

<span data-ttu-id="2e946-p103">来自 **DriveItem** 资源上同一属性的 **createdDateTime** 和 [lastModifiedDateTime](driveitem.md) 值有所不同。DriveItem 资源上的值是从服务中所见的创建和修改的日期和时间。**FileSystemInfo** 资源中存储的值由客户端提供。</span><span class="sxs-lookup"><span data-stu-id="2e946-p103">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource. The values on the DriveItem resource are the created and modified date and time as seen from the service. The values stored in the **FileSystemInfo** resource are provided by the client.</span></span>

<span data-ttu-id="2e946-p104">例如，如果星期一在设备上创建文件，但直到星期二才上载到服务，则上载文件的客户端应写入 `fileSystemInfo` facet，以包括星期一这一创建日期。检索项元数据时，项的创建日期将反映为星期二，但 `fileSystemInfo` facet 将显示星期一这一创建的原始创建日期。</span><span class="sxs-lookup"><span data-stu-id="2e946-p104">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="2e946-p105">这些属性为读/写。如果正在上载文件，并且知道这些字段的本地客户端值，则应该在请求中包括它们。</span><span class="sxs-lookup"><span data-stu-id="2e946-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="2e946-129">如果文件内容已更新且未提供这些属性，**lastModifiedDateTime** 将自动重置为当前时间。</span><span class="sxs-lookup"><span data-stu-id="2e946-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="2e946-130">注解</span><span class="sxs-lookup"><span data-stu-id="2e946-130">Remarks</span></span>

* <span data-ttu-id="2e946-131">**lastAccessedDateTime** 不适用于 SharePoint Online 或 OneDrive for Business 中的项。</span><span class="sxs-lookup"><span data-stu-id="2e946-131">**lastAccessedDateTime** is not available for items in SharePoint online or OneDrive for Business.</span></span>

<span data-ttu-id="2e946-132">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="2e946-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
