---
author: JeremyKelley
description: baseItem 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 5d72147602872478578b39617c77b227a27124b4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508029"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="8c2d7-103">BaseItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c2d7-103">BaseItem resource type</span></span>

<span data-ttu-id="8c2d7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8c2d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c2d7-p101">**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="8c2d7-107">drive</span><span class="sxs-lookup"><span data-stu-id="8c2d7-107">drive</span></span>](drive.md)
* [<span data-ttu-id="8c2d7-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="8c2d7-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="8c2d7-109">网站</span><span class="sxs-lookup"><span data-stu-id="8c2d7-109">site</span></span>](site.md)
* [<span data-ttu-id="8c2d7-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="8c2d7-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="8c2d7-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c2d7-111">JSON representation</span></span>

<span data-ttu-id="8c2d7-112">下面是 **baseItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="8c2d7-113">属性</span><span class="sxs-lookup"><span data-stu-id="8c2d7-113">Properties</span></span>

| <span data-ttu-id="8c2d7-114">属性</span><span class="sxs-lookup"><span data-stu-id="8c2d7-114">Property</span></span>             | <span data-ttu-id="8c2d7-115">类型</span><span class="sxs-lookup"><span data-stu-id="8c2d7-115">Type</span></span>              | <span data-ttu-id="8c2d7-116">说明</span><span class="sxs-lookup"><span data-stu-id="8c2d7-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="8c2d7-117">id</span><span class="sxs-lookup"><span data-stu-id="8c2d7-117">id</span></span>                   | <span data-ttu-id="8c2d7-118">string</span><span class="sxs-lookup"><span data-stu-id="8c2d7-118">string</span></span>            | <span data-ttu-id="8c2d7-p102">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="8c2d7-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="8c2d7-121">createdBy</span></span>            | <span data-ttu-id="8c2d7-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8c2d7-122">[identitySet][]</span></span>   | <span data-ttu-id="8c2d7-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="8c2d7-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c2d7-125">createdDateTime</span></span>      | <span data-ttu-id="8c2d7-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c2d7-126">dateTimeOffset</span></span>    | <span data-ttu-id="8c2d7-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="8c2d7-129">eTag</span><span class="sxs-lookup"><span data-stu-id="8c2d7-129">eTag</span></span>                 | <span data-ttu-id="8c2d7-130">字符串</span><span class="sxs-lookup"><span data-stu-id="8c2d7-130">string</span></span>            | <span data-ttu-id="8c2d7-p105">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p105">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="8c2d7-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8c2d7-133">lastModifiedBy</span></span>       | <span data-ttu-id="8c2d7-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="8c2d7-134">[identitySet][]</span></span>   | <span data-ttu-id="8c2d7-p106">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p106">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="8c2d7-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c2d7-137">lastModifiedDateTime</span></span> | <span data-ttu-id="8c2d7-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c2d7-138">dateTimeOffset</span></span>    | <span data-ttu-id="8c2d7-p107">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p107">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="8c2d7-141">name</span><span class="sxs-lookup"><span data-stu-id="8c2d7-141">name</span></span>                 | <span data-ttu-id="8c2d7-142">string</span><span class="sxs-lookup"><span data-stu-id="8c2d7-142">string</span></span>            | <span data-ttu-id="8c2d7-p108">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p108">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="8c2d7-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="8c2d7-145">parentReference</span></span>      | <span data-ttu-id="8c2d7-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="8c2d7-146">[itemReference][]</span></span> | <span data-ttu-id="8c2d7-p109">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p109">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="8c2d7-149">webUrl</span><span class="sxs-lookup"><span data-stu-id="8c2d7-149">webUrl</span></span>               | <span data-ttu-id="8c2d7-150">string (url)</span><span class="sxs-lookup"><span data-stu-id="8c2d7-150">string (url)</span></span>      | <span data-ttu-id="8c2d7-p110">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-p110">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="8c2d7-155">注解</span><span class="sxs-lookup"><span data-stu-id="8c2d7-155">Remarks</span></span>

<span data-ttu-id="8c2d7-156">`baseItem` 类型不应直接使用。</span><span class="sxs-lookup"><span data-stu-id="8c2d7-156">The `baseItem` type is not expected to be used directly.</span></span>

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
