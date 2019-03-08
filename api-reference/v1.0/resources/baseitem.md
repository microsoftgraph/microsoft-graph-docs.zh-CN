---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
ms.openlocfilehash: ae22b0a36acb46c2a9d872f224c0a6d4c567782c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481130"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="6ba3e-102">BaseItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ba3e-102">BaseItem resource type</span></span>

<span data-ttu-id="6ba3e-p101">**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="6ba3e-105">drive</span><span class="sxs-lookup"><span data-stu-id="6ba3e-105">drive</span></span>](drive.md)
* [<span data-ttu-id="6ba3e-106">driveItem</span><span class="sxs-lookup"><span data-stu-id="6ba3e-106">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="6ba3e-107">网站</span><span class="sxs-lookup"><span data-stu-id="6ba3e-107">site</span></span>](site.md)
* [<span data-ttu-id="6ba3e-108">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="6ba3e-108">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="6ba3e-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ba3e-109">JSON representation</span></span>

<span data-ttu-id="6ba3e-110">下面是 **baseItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-110">Here is a JSON representation of a **baseItem** resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "createdBy", "lastModifiedBy", "description", "parentReference", "webUrl" ],
  "keyProperty": "id",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
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

## <a name="properties"></a><span data-ttu-id="6ba3e-111">属性</span><span class="sxs-lookup"><span data-stu-id="6ba3e-111">Properties</span></span>

| <span data-ttu-id="6ba3e-112">属性</span><span class="sxs-lookup"><span data-stu-id="6ba3e-112">Property</span></span>             | <span data-ttu-id="6ba3e-113">类型</span><span class="sxs-lookup"><span data-stu-id="6ba3e-113">Type</span></span>              | <span data-ttu-id="6ba3e-114">说明</span><span class="sxs-lookup"><span data-stu-id="6ba3e-114">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="6ba3e-115">id</span><span class="sxs-lookup"><span data-stu-id="6ba3e-115">id</span></span>                   | <span data-ttu-id="6ba3e-116">string</span><span class="sxs-lookup"><span data-stu-id="6ba3e-116">string</span></span>            | <span data-ttu-id="6ba3e-p102">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="6ba3e-119">createdBy</span><span class="sxs-lookup"><span data-stu-id="6ba3e-119">createdBy</span></span>            | <span data-ttu-id="6ba3e-120">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6ba3e-120">[identitySet][]</span></span>   | <span data-ttu-id="6ba3e-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="6ba3e-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba3e-123">createdDateTime</span></span>      | <span data-ttu-id="6ba3e-124">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba3e-124">dateTimeOffset</span></span>    | <span data-ttu-id="6ba3e-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="6ba3e-127">description</span><span class="sxs-lookup"><span data-stu-id="6ba3e-127">description</span></span>          | <span data-ttu-id="6ba3e-128">String</span><span class="sxs-lookup"><span data-stu-id="6ba3e-128">String</span></span>            | <span data-ttu-id="6ba3e-129">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-129">Provides a user-visible description of the item.</span></span> <span data-ttu-id="6ba3e-130">可选。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-130">Optional.</span></span>                             |
| <span data-ttu-id="6ba3e-131">eTag</span><span class="sxs-lookup"><span data-stu-id="6ba3e-131">eTag</span></span>                 | <span data-ttu-id="6ba3e-132">string</span><span class="sxs-lookup"><span data-stu-id="6ba3e-132">string</span></span>            | <span data-ttu-id="6ba3e-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="6ba3e-135">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6ba3e-135">lastModifiedBy</span></span>       | <span data-ttu-id="6ba3e-136">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6ba3e-136">[identitySet][]</span></span>   | <span data-ttu-id="6ba3e-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="6ba3e-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6ba3e-139">lastModifiedDateTime</span></span> | <span data-ttu-id="6ba3e-140">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6ba3e-140">dateTimeOffset</span></span>    | <span data-ttu-id="6ba3e-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="6ba3e-143">name</span><span class="sxs-lookup"><span data-stu-id="6ba3e-143">name</span></span>                 | <span data-ttu-id="6ba3e-144">string</span><span class="sxs-lookup"><span data-stu-id="6ba3e-144">string</span></span>            | <span data-ttu-id="6ba3e-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="6ba3e-147">parentReference</span><span class="sxs-lookup"><span data-stu-id="6ba3e-147">parentReference</span></span>      | <span data-ttu-id="6ba3e-148">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="6ba3e-148">[itemReference][]</span></span> | <span data-ttu-id="6ba3e-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="6ba3e-151">WebUrl</span><span class="sxs-lookup"><span data-stu-id="6ba3e-151">webUrl</span></span>               | <span data-ttu-id="6ba3e-152">string (url)</span><span class="sxs-lookup"><span data-stu-id="6ba3e-152">string (url)</span></span>      | <span data-ttu-id="6ba3e-p111">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="6ba3e-155">关系</span><span class="sxs-lookup"><span data-stu-id="6ba3e-155">Relationships</span></span>

| <span data-ttu-id="6ba3e-156">关系</span><span class="sxs-lookup"><span data-stu-id="6ba3e-156">Relationship</span></span>       | <span data-ttu-id="6ba3e-157">类型</span><span class="sxs-lookup"><span data-stu-id="6ba3e-157">Type</span></span>     | <span data-ttu-id="6ba3e-158">说明</span><span class="sxs-lookup"><span data-stu-id="6ba3e-158">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="6ba3e-159">createdByUser</span><span class="sxs-lookup"><span data-stu-id="6ba3e-159">createdByUser</span></span>      | <span data-ttu-id="6ba3e-160">[user][]</span><span class="sxs-lookup"><span data-stu-id="6ba3e-160">[user][]</span></span> | <span data-ttu-id="6ba3e-161">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-161">Identity of the user who created the item.</span></span> <span data-ttu-id="6ba3e-162">只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-162">Read-only.</span></span>
| <span data-ttu-id="6ba3e-163">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="6ba3e-163">lastModifiedByUser</span></span> | <span data-ttu-id="6ba3e-164">[用户][]</span><span class="sxs-lookup"><span data-stu-id="6ba3e-164">[user][]</span></span> | <span data-ttu-id="6ba3e-165">上次修改项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-165">Identity of the user who last modified the item.</span></span> <span data-ttu-id="6ba3e-166">只读。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-166">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="6ba3e-170">注解</span><span class="sxs-lookup"><span data-stu-id="6ba3e-170">Remarks</span></span>

<span data-ttu-id="6ba3e-171">`baseItem` 类型不应直接使用。</span><span class="sxs-lookup"><span data-stu-id="6ba3e-171">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
