---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: baseItem 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2bde386a736805d52758f6d80e629c585f82d87e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029979"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="509dd-103">BaseItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="509dd-103">BaseItem resource type</span></span>

<span data-ttu-id="509dd-p101">**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：</span><span class="sxs-lookup"><span data-stu-id="509dd-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="509dd-106">drive</span><span class="sxs-lookup"><span data-stu-id="509dd-106">drive</span></span>](drive.md)
* [<span data-ttu-id="509dd-107">driveItem</span><span class="sxs-lookup"><span data-stu-id="509dd-107">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="509dd-108">网站</span><span class="sxs-lookup"><span data-stu-id="509dd-108">site</span></span>](site.md)
* [<span data-ttu-id="509dd-109">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="509dd-109">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="509dd-110">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="509dd-110">JSON representation</span></span>

<span data-ttu-id="509dd-111">下面是 **baseItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="509dd-111">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="509dd-112">属性</span><span class="sxs-lookup"><span data-stu-id="509dd-112">Properties</span></span>

| <span data-ttu-id="509dd-113">属性</span><span class="sxs-lookup"><span data-stu-id="509dd-113">Property</span></span>             | <span data-ttu-id="509dd-114">类型</span><span class="sxs-lookup"><span data-stu-id="509dd-114">Type</span></span>              | <span data-ttu-id="509dd-115">说明</span><span class="sxs-lookup"><span data-stu-id="509dd-115">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="509dd-116">id</span><span class="sxs-lookup"><span data-stu-id="509dd-116">id</span></span>                   | <span data-ttu-id="509dd-117">string</span><span class="sxs-lookup"><span data-stu-id="509dd-117">string</span></span>            | <span data-ttu-id="509dd-p102">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="509dd-120">createdBy</span><span class="sxs-lookup"><span data-stu-id="509dd-120">createdBy</span></span>            | <span data-ttu-id="509dd-121">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="509dd-121">[identitySet][]</span></span>   | <span data-ttu-id="509dd-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="509dd-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="509dd-124">createdDateTime</span></span>      | <span data-ttu-id="509dd-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="509dd-125">dateTimeOffset</span></span>    | <span data-ttu-id="509dd-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="509dd-128">description</span><span class="sxs-lookup"><span data-stu-id="509dd-128">description</span></span>          | <span data-ttu-id="509dd-129">String</span><span class="sxs-lookup"><span data-stu-id="509dd-129">String</span></span>            | <span data-ttu-id="509dd-130">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="509dd-130">Provides a user-visible description of the item.</span></span> <span data-ttu-id="509dd-131">可选。</span><span class="sxs-lookup"><span data-stu-id="509dd-131">Optional.</span></span>                             |
| <span data-ttu-id="509dd-132">eTag</span><span class="sxs-lookup"><span data-stu-id="509dd-132">eTag</span></span>                 | <span data-ttu-id="509dd-133">字符串</span><span class="sxs-lookup"><span data-stu-id="509dd-133">string</span></span>            | <span data-ttu-id="509dd-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="509dd-136">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="509dd-136">lastModifiedBy</span></span>       | <span data-ttu-id="509dd-137">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="509dd-137">[identitySet][]</span></span>   | <span data-ttu-id="509dd-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="509dd-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="509dd-140">lastModifiedDateTime</span></span> | <span data-ttu-id="509dd-141">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="509dd-141">dateTimeOffset</span></span>    | <span data-ttu-id="509dd-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="509dd-144">name</span><span class="sxs-lookup"><span data-stu-id="509dd-144">name</span></span>                 | <span data-ttu-id="509dd-145">string</span><span class="sxs-lookup"><span data-stu-id="509dd-145">string</span></span>            | <span data-ttu-id="509dd-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="509dd-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="509dd-148">parentReference</span><span class="sxs-lookup"><span data-stu-id="509dd-148">parentReference</span></span>      | <span data-ttu-id="509dd-149">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="509dd-149">[itemReference][]</span></span> | <span data-ttu-id="509dd-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="509dd-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="509dd-152">WebUrl</span><span class="sxs-lookup"><span data-stu-id="509dd-152">webUrl</span></span>               | <span data-ttu-id="509dd-153">string (url)</span><span class="sxs-lookup"><span data-stu-id="509dd-153">string (url)</span></span>      | <span data-ttu-id="509dd-p111">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="509dd-156">关系</span><span class="sxs-lookup"><span data-stu-id="509dd-156">Relationships</span></span>

| <span data-ttu-id="509dd-157">关系</span><span class="sxs-lookup"><span data-stu-id="509dd-157">Relationship</span></span>       | <span data-ttu-id="509dd-158">类型</span><span class="sxs-lookup"><span data-stu-id="509dd-158">Type</span></span>     | <span data-ttu-id="509dd-159">说明</span><span class="sxs-lookup"><span data-stu-id="509dd-159">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="509dd-160">createdByUser</span><span class="sxs-lookup"><span data-stu-id="509dd-160">createdByUser</span></span>      | <span data-ttu-id="509dd-161">[用户][]</span><span class="sxs-lookup"><span data-stu-id="509dd-161">[user][]</span></span> | <span data-ttu-id="509dd-162">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="509dd-162">Identity of the user who created the item.</span></span> <span data-ttu-id="509dd-163">只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-163">Read-only.</span></span>
| <span data-ttu-id="509dd-164">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="509dd-164">lastModifiedByUser</span></span> | <span data-ttu-id="509dd-165">[user][]</span><span class="sxs-lookup"><span data-stu-id="509dd-165">[user][]</span></span> | <span data-ttu-id="509dd-166">上次修改项的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="509dd-166">Identity of the user who last modified the item.</span></span> <span data-ttu-id="509dd-167">只读。</span><span class="sxs-lookup"><span data-stu-id="509dd-167">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[用户]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="509dd-171">注解</span><span class="sxs-lookup"><span data-stu-id="509dd-171">Remarks</span></span>

<span data-ttu-id="509dd-172">`baseItem` 类型不应直接使用。</span><span class="sxs-lookup"><span data-stu-id="509dd-172">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
