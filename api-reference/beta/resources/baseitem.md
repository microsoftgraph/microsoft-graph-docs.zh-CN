---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: 8e01d219fcc67c583fddba8d9893ed94a23c409b
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481970"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="aceaa-102">BaseItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="aceaa-102">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aceaa-p101">**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：</span><span class="sxs-lookup"><span data-stu-id="aceaa-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="aceaa-105">drive</span><span class="sxs-lookup"><span data-stu-id="aceaa-105">drive</span></span>](drive.md)
* [<span data-ttu-id="aceaa-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="aceaa-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="aceaa-107">网站</span><span class="sxs-lookup"><span data-stu-id="aceaa-107">site</span></span>](site.md)
* [<span data-ttu-id="aceaa-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="aceaa-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="aceaa-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aceaa-109">JSON representation</span></span>

<span data-ttu-id="aceaa-110">下面是 **baseItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aceaa-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem"
}-->

```json
{
  "id": "string (identifier)",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "datetime",
  "description": "string",
  "eTag": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "datetime",
  "name": "string",
  "parentReference": { "@odata.type": "microsoft.graph.itemReference" },
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="aceaa-111">属性</span><span class="sxs-lookup"><span data-stu-id="aceaa-111">Properties</span></span>

| <span data-ttu-id="aceaa-112">属性</span><span class="sxs-lookup"><span data-stu-id="aceaa-112">Property</span></span>             | <span data-ttu-id="aceaa-113">类型</span><span class="sxs-lookup"><span data-stu-id="aceaa-113">Type</span></span>              | <span data-ttu-id="aceaa-114">说明</span><span class="sxs-lookup"><span data-stu-id="aceaa-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="aceaa-115">id</span><span class="sxs-lookup"><span data-stu-id="aceaa-115">id</span></span>                   | <span data-ttu-id="aceaa-116">string</span><span class="sxs-lookup"><span data-stu-id="aceaa-116">string</span></span>            | <span data-ttu-id="aceaa-p102">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="aceaa-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="aceaa-119">createdBy</span></span>            | <span data-ttu-id="aceaa-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="aceaa-120">[identitySet][]</span></span>   | <span data-ttu-id="aceaa-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="aceaa-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aceaa-123">createdDateTime</span></span>      | <span data-ttu-id="aceaa-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aceaa-124">dateTimeOffset</span></span>    | <span data-ttu-id="aceaa-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="aceaa-127">eTag</span><span class="sxs-lookup"><span data-stu-id="aceaa-127">eTag</span></span>                 | <span data-ttu-id="aceaa-128">string</span><span class="sxs-lookup"><span data-stu-id="aceaa-128">string</span></span>            | <span data-ttu-id="aceaa-p105">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="aceaa-131">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="aceaa-131">lastModifiedBy</span></span>       | <span data-ttu-id="aceaa-132">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="aceaa-132">[identitySet][]</span></span>   | <span data-ttu-id="aceaa-p106">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="aceaa-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aceaa-135">lastModifiedDateTime</span></span> | <span data-ttu-id="aceaa-136">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aceaa-136">dateTimeOffset</span></span>    | <span data-ttu-id="aceaa-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="aceaa-139">name</span><span class="sxs-lookup"><span data-stu-id="aceaa-139">name</span></span>                 | <span data-ttu-id="aceaa-140">string</span><span class="sxs-lookup"><span data-stu-id="aceaa-140">string</span></span>            | <span data-ttu-id="aceaa-p108">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="aceaa-143">parentReference</span><span class="sxs-lookup"><span data-stu-id="aceaa-143">parentReference</span></span>      | <span data-ttu-id="aceaa-144">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="aceaa-144">[itemReference][]</span></span> | <span data-ttu-id="aceaa-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="aceaa-147">WebUrl</span><span class="sxs-lookup"><span data-stu-id="aceaa-147">webUrl</span></span>               | <span data-ttu-id="aceaa-148">string (url)</span><span class="sxs-lookup"><span data-stu-id="aceaa-148">string (url)</span></span>      | <span data-ttu-id="aceaa-p110">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="aceaa-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="aceaa-153">注解</span><span class="sxs-lookup"><span data-stu-id="aceaa-153">Remarks</span></span>

<span data-ttu-id="aceaa-154">`baseItem` 类型不应直接使用。</span><span class="sxs-lookup"><span data-stu-id="aceaa-154">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": [
    "Error: /api-reference/beta/resources/baseitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
