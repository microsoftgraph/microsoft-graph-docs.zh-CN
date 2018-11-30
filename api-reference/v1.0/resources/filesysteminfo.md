---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: FileSystemInfo
ms.openlocfilehash: 9a5214f9c5e161de0be66ac634c7c5538b203772
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="filesysteminfo-facet"></a><span data-ttu-id="e3c76-102">FileSystemInfo Facet</span><span class="sxs-lookup"><span data-stu-id="e3c76-102">FileSystemInfo facet</span></span>

<span data-ttu-id="e3c76-103">**FileSystemInfo** 资源包含设备本地文件系统所报告的项目本地版本的属性。</span><span class="sxs-lookup"><span data-stu-id="e3c76-103">The **FileSystemInfo** resource contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>
<span data-ttu-id="e3c76-104">此 Facet 可用于指定本地设备上项的上次修改日期或创建日期。</span><span class="sxs-lookup"><span data-stu-id="e3c76-104">The FileSystemInfo facet contains properties that are reported by the device's local file system for the local version of an item. This facet can be used to specify the last modified date or created date of the item as it was on the local device.</span></span>

<span data-ttu-id="e3c76-105">可用于 [driveItem][item-resource] 资源的 fileSystemInfo 属性。</span><span class="sxs-lookup"><span data-stu-id="e3c76-105">It is available on the fileSystemInfo property of [driveItem][item-resource] resources.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3c76-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3c76-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="e3c76-107">属性</span><span class="sxs-lookup"><span data-stu-id="e3c76-107">Properties</span></span>

| <span data-ttu-id="e3c76-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3c76-108">Property</span></span>                 | <span data-ttu-id="e3c76-109">类型</span><span class="sxs-lookup"><span data-stu-id="e3c76-109">Type</span></span>           | <span data-ttu-id="e3c76-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3c76-110">Description</span></span>                                                                                                          |
| :----------------------- | :------------- | :------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e3c76-111">**createdDateTime**</span><span class="sxs-lookup"><span data-stu-id="e3c76-111">**createdDateTime**</span></span>      | <span data-ttu-id="e3c76-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c76-112">DateTimeOffset</span></span> | <span data-ttu-id="e3c76-113">在客户端创建文件时的 UTC 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e3c76-113">The UTC date and time the file was created on a client.</span></span>                                                              |
| <span data-ttu-id="e3c76-114">**lastAccessedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e3c76-114">**lastAccessedDateTime**</span></span> | <span data-ttu-id="e3c76-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c76-115">DateTimeOffset</span></span> | <span data-ttu-id="e3c76-116">上次访问文件时的 UTC 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e3c76-116">The UTC date and time the file was last accessed on a client.</span></span> <span data-ttu-id="e3c76-117">仅可用于[最近的文件列表](../api/drive_recent.md)。</span><span class="sxs-lookup"><span data-stu-id="e3c76-117">Available for the [recent file list](../api/drive_recent.md) only.</span></span> |
| <span data-ttu-id="e3c76-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="e3c76-118">**lastModifiedDateTime**</span></span> | <span data-ttu-id="e3c76-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c76-119">DateTimeOffset</span></span> | <span data-ttu-id="e3c76-120">在客户端上次修改文件时的 UTC 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e3c76-120">The UTC date and time the file was last modified on a client.</span></span>                                                        |

## <a name="notes"></a><span data-ttu-id="e3c76-121">注意</span><span class="sxs-lookup"><span data-stu-id="e3c76-121">Notes</span></span>

<span data-ttu-id="e3c76-122">来自 [DriveItem](driveitem.md) 资源上同一属性的 **createdDateTime** 和 **lastModifiedDateTime** 值有所不同。</span><span class="sxs-lookup"><span data-stu-id="e3c76-122">Values for **createdDateTime** and **lastModifiedDateTime** vary from the same properties on the [DriveItem](driveitem.md) resource.</span></span>
<span data-ttu-id="e3c76-123">DriveItem 资源上的值是从服务中所见的创建和修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e3c76-123">The properties on the driveItem resource are the created and modified date and time from the perspective of when the service saw the file.</span></span>
<span data-ttu-id="e3c76-124">**FileSystemInfo** 资源中存储的值由客户端提供。</span><span class="sxs-lookup"><span data-stu-id="e3c76-124">The values stored in the **FileSystemInfo** facet are provided by the client are are the values displayed to the user if they exist.</span></span>

<span data-ttu-id="e3c76-125">例如，如果星期一在设备上创建文件，但直到星期二才上传到服务，则上传文件的客户端应写入 `fileSystemInfo` facet，以包括星期一这一创建日期。</span><span class="sxs-lookup"><span data-stu-id="e3c76-125">For example, if a file was created on the device on Monday, but not uploaded to the service until Tuesday, the client that uploads the file should write the `fileSystemInfo` facet to include the created date on Monday. When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the  facet will show the original created date on Monday.</span></span> <span data-ttu-id="e3c76-126">检索项元数据时，项的创建日期将反映为星期二，但 `fileSystemInfo` Facet 将显示星期一这一原始创建日期。</span><span class="sxs-lookup"><span data-stu-id="e3c76-126">When the item metadata is retrieved, the created date for the item will reflect Tuesday, but the `fileSystemInfo` facet will show the original created date on Monday.</span></span>

<span data-ttu-id="e3c76-p105">这些属性为读/写。如果正在上载文件，并且知道这些字段的本地客户端值，则应该在请求中包括它们。</span><span class="sxs-lookup"><span data-stu-id="e3c76-p105">These properties are read/write. If you are uploading a file and know the local client values for these fields, you should include them in the request.</span></span>

<span data-ttu-id="e3c76-129">如果文件内容已更新且未提供这些属性，**lastModifiedDateTime** 将自动重置为当前时间。</span><span class="sxs-lookup"><span data-stu-id="e3c76-129">If the file's content is updated and these properties are not provided, **lastModifiedDateTime** automatically resets to the current time.</span></span>

## <a name="remarks"></a><span data-ttu-id="e3c76-130">备注</span><span class="sxs-lookup"><span data-stu-id="e3c76-130">Remarks</span></span>

* <span data-ttu-id="e3c76-131">**lastAccessedDateTime** 不适用于 SharePoint Online 或 OneDrive for Business 中的项。</span><span class="sxs-lookup"><span data-stu-id="e3c76-131">**lastAccessedDateTime** is not available for items in SharePoint online, OneDrive for Business, or SharePoint Server 2016.</span></span>

<span data-ttu-id="e3c76-132">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e3c76-132">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "The fileSystemInfo facet provides information about date created and modified by clients.",
  "keywords": "fileSystemInfo,client,system info,onedrive",
  "section": "documentation",
  "tocPath": "Facets/FileSystemInfo"
} -->
