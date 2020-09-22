---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: BaseItem
localization_priority: Normal
description: baseItem 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6c247891afed001977174f3de232a8b2385e0841
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075082"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="49977-103">BaseItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="49977-103">BaseItem resource type</span></span>

<span data-ttu-id="49977-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49977-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49977-p101">**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：</span><span class="sxs-lookup"><span data-stu-id="49977-p101">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="49977-107">drive</span><span class="sxs-lookup"><span data-stu-id="49977-107">drive</span></span>](drive.md)
* [<span data-ttu-id="49977-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="49977-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="49977-109">网站</span><span class="sxs-lookup"><span data-stu-id="49977-109">site</span></span>](site.md)
* [<span data-ttu-id="49977-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="49977-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="49977-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49977-111">JSON representation</span></span>

<span data-ttu-id="49977-112">下面是 **baseItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49977-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="49977-113">属性</span><span class="sxs-lookup"><span data-stu-id="49977-113">Properties</span></span>

| <span data-ttu-id="49977-114">属性</span><span class="sxs-lookup"><span data-stu-id="49977-114">Property</span></span>             | <span data-ttu-id="49977-115">类型</span><span class="sxs-lookup"><span data-stu-id="49977-115">Type</span></span>              | <span data-ttu-id="49977-116">说明</span><span class="sxs-lookup"><span data-stu-id="49977-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="49977-117">id</span><span class="sxs-lookup"><span data-stu-id="49977-117">id</span></span>                   | <span data-ttu-id="49977-118">string</span><span class="sxs-lookup"><span data-stu-id="49977-118">string</span></span>            | <span data-ttu-id="49977-p102">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="49977-p102">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="49977-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="49977-121">createdBy</span></span>            | <span data-ttu-id="49977-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="49977-122">[identitySet][]</span></span>   | <span data-ttu-id="49977-p103">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="49977-p103">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="49977-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49977-125">createdDateTime</span></span>      | <span data-ttu-id="49977-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49977-126">dateTimeOffset</span></span>    | <span data-ttu-id="49977-p104">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="49977-p104">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="49977-129">description</span><span class="sxs-lookup"><span data-stu-id="49977-129">description</span></span>          | <span data-ttu-id="49977-130">String</span><span class="sxs-lookup"><span data-stu-id="49977-130">String</span></span>            | <span data-ttu-id="49977-131">提供项的用户可见的说明。</span><span class="sxs-lookup"><span data-stu-id="49977-131">Provides a user-visible description of the item.</span></span> <span data-ttu-id="49977-132">可选。</span><span class="sxs-lookup"><span data-stu-id="49977-132">Optional.</span></span>                             |
| <span data-ttu-id="49977-133">eTag</span><span class="sxs-lookup"><span data-stu-id="49977-133">eTag</span></span>                 | <span data-ttu-id="49977-134">字符串</span><span class="sxs-lookup"><span data-stu-id="49977-134">string</span></span>            | <span data-ttu-id="49977-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="49977-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="49977-137">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="49977-137">lastModifiedBy</span></span>       | <span data-ttu-id="49977-138">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="49977-138">[identitySet][]</span></span>   | <span data-ttu-id="49977-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="49977-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="49977-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49977-141">lastModifiedDateTime</span></span> | <span data-ttu-id="49977-142">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49977-142">dateTimeOffset</span></span>    | <span data-ttu-id="49977-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="49977-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="49977-145">name</span><span class="sxs-lookup"><span data-stu-id="49977-145">name</span></span>                 | <span data-ttu-id="49977-146">string</span><span class="sxs-lookup"><span data-stu-id="49977-146">string</span></span>            | <span data-ttu-id="49977-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="49977-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="49977-149">parentReference</span><span class="sxs-lookup"><span data-stu-id="49977-149">parentReference</span></span>      | <span data-ttu-id="49977-150">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="49977-150">[itemReference][]</span></span> | <span data-ttu-id="49977-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="49977-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="49977-153">webUrl</span><span class="sxs-lookup"><span data-stu-id="49977-153">webUrl</span></span>               | <span data-ttu-id="49977-154">string (url)</span><span class="sxs-lookup"><span data-stu-id="49977-154">string (url)</span></span>      | <span data-ttu-id="49977-p111">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="49977-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

## <a name="relationships"></a><span data-ttu-id="49977-157">关系</span><span class="sxs-lookup"><span data-stu-id="49977-157">Relationships</span></span>

| <span data-ttu-id="49977-158">关系</span><span class="sxs-lookup"><span data-stu-id="49977-158">Relationship</span></span>       | <span data-ttu-id="49977-159">类型</span><span class="sxs-lookup"><span data-stu-id="49977-159">Type</span></span>     | <span data-ttu-id="49977-160">说明</span><span class="sxs-lookup"><span data-stu-id="49977-160">Description</span></span>
|:-------------------|:---------|:---------------------------------------------
| <span data-ttu-id="49977-161">createdByUser</span><span class="sxs-lookup"><span data-stu-id="49977-161">createdByUser</span></span>      | <span data-ttu-id="49977-162">[user][]</span><span class="sxs-lookup"><span data-stu-id="49977-162">[user][]</span></span> | <span data-ttu-id="49977-163">创建了项的用户的身份。</span><span class="sxs-lookup"><span data-stu-id="49977-163">Identity of the user who created the item.</span></span> <span data-ttu-id="49977-164">只读。</span><span class="sxs-lookup"><span data-stu-id="49977-164">Read-only.</span></span>
| <span data-ttu-id="49977-165">lastModifiedByUser</span><span class="sxs-lookup"><span data-stu-id="49977-165">lastModifiedByUser</span></span> | <span data-ttu-id="49977-166">[user][]</span><span class="sxs-lookup"><span data-stu-id="49977-166">[user][]</span></span> | <span data-ttu-id="49977-167">上次修改项的用户的标识。</span><span class="sxs-lookup"><span data-stu-id="49977-167">Identity of the user who last modified the item.</span></span> <span data-ttu-id="49977-168">只读。</span><span class="sxs-lookup"><span data-stu-id="49977-168">Read-only.</span></span>

[identitySet]: identityset.md
[itemReference]: itemreference.md
[用户]: user.md
[user]: user.md

## <a name="remarks"></a><span data-ttu-id="49977-172">注解</span><span class="sxs-lookup"><span data-stu-id="49977-172">Remarks</span></span>

<span data-ttu-id="49977-173">`baseItem` 类型不应直接使用。</span><span class="sxs-lookup"><span data-stu-id="49977-173">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->

