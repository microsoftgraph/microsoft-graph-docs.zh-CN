---
author: JeremyKelley
description: baseItem 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 38e697e4a991871bd592cc891dcd131e845572fe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013141"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="31639-103">BaseItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="31639-103">BaseItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31639-p101">**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：</span><span class="sxs-lookup"><span data-stu-id="31639-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="31639-106">drive</span><span class="sxs-lookup"><span data-stu-id="31639-106">drive</span></span>](drive.md)
* [<span data-ttu-id="31639-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="31639-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="31639-108">网站</span><span class="sxs-lookup"><span data-stu-id="31639-108">site</span></span>](site.md)
* [<span data-ttu-id="31639-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="31639-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="31639-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="31639-110">JSON representation</span></span>

<span data-ttu-id="31639-111">下面是 **baseItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="31639-111">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItem",
  "abstract": true
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

## <a name="properties"></a><span data-ttu-id="31639-112">属性</span><span class="sxs-lookup"><span data-stu-id="31639-112">Properties</span></span>

| <span data-ttu-id="31639-113">属性</span><span class="sxs-lookup"><span data-stu-id="31639-113">Property</span></span>             | <span data-ttu-id="31639-114">类型</span><span class="sxs-lookup"><span data-stu-id="31639-114">Type</span></span>              | <span data-ttu-id="31639-115">说明</span><span class="sxs-lookup"><span data-stu-id="31639-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="31639-116">id</span><span class="sxs-lookup"><span data-stu-id="31639-116">id</span></span>                   | <span data-ttu-id="31639-117">string</span><span class="sxs-lookup"><span data-stu-id="31639-117">string</span></span>            | <span data-ttu-id="31639-p102">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="31639-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="31639-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="31639-120">createdBy</span></span>            | <span data-ttu-id="31639-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="31639-121">[identitySet][]</span></span>   | <span data-ttu-id="31639-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="31639-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="31639-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31639-124">createdDateTime</span></span>      | <span data-ttu-id="31639-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31639-125">dateTimeOffset</span></span>    | <span data-ttu-id="31639-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="31639-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="31639-128">eTag</span><span class="sxs-lookup"><span data-stu-id="31639-128">eTag</span></span>                 | <span data-ttu-id="31639-129">字符串</span><span class="sxs-lookup"><span data-stu-id="31639-129">string</span></span>            | <span data-ttu-id="31639-p105">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="31639-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="31639-132">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="31639-132">lastModifiedBy</span></span>       | <span data-ttu-id="31639-133">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="31639-133">[identitySet][]</span></span>   | <span data-ttu-id="31639-p106">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="31639-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="31639-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31639-136">lastModifiedDateTime</span></span> | <span data-ttu-id="31639-137">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31639-137">dateTimeOffset</span></span>    | <span data-ttu-id="31639-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="31639-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="31639-140">name</span><span class="sxs-lookup"><span data-stu-id="31639-140">name</span></span>                 | <span data-ttu-id="31639-141">string</span><span class="sxs-lookup"><span data-stu-id="31639-141">string</span></span>            | <span data-ttu-id="31639-p108">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="31639-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="31639-144">parentReference</span><span class="sxs-lookup"><span data-stu-id="31639-144">parentReference</span></span>      | <span data-ttu-id="31639-145">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="31639-145">[itemReference][]</span></span> | <span data-ttu-id="31639-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="31639-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="31639-148">WebUrl</span><span class="sxs-lookup"><span data-stu-id="31639-148">webUrl</span></span>               | <span data-ttu-id="31639-149">string (url)</span><span class="sxs-lookup"><span data-stu-id="31639-149">string (url)</span></span>      | <span data-ttu-id="31639-p110">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="31639-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="31639-154">注解</span><span class="sxs-lookup"><span data-stu-id="31639-154">Remarks</span></span>

<span data-ttu-id="31639-155">`baseItem` 类型不应直接使用。</span><span class="sxs-lookup"><span data-stu-id="31639-155">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem",
  "suppressions": []
}
-->
