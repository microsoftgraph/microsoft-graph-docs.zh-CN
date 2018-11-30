---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: BaseItem
ms.openlocfilehash: d70a75be0be4d7ecbd010288cb313b8394736932
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049412"
---
# <a name="baseitem-resource-type"></a><span data-ttu-id="3a71f-102">BaseItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a71f-102">BaseItem resource type</span></span>

> <span data-ttu-id="3a71f-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3a71f-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a71f-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3a71f-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a71f-p102">**baseItem** 资源是抽象资源，其中包含一组在若干其他资源类型中共享的常见类型。从 **baseItem** 派生的资源包括：</span><span class="sxs-lookup"><span data-stu-id="3a71f-p102">The **baseItem** resource is an abstract resource that contains a common set of properties shared among several other resources types. Resources that derive from **baseItem** include:</span></span>

* [<span data-ttu-id="3a71f-107">drive</span><span class="sxs-lookup"><span data-stu-id="3a71f-107">drive</span></span>](drive.md)
* [<span data-ttu-id="3a71f-108">driveItem</span><span class="sxs-lookup"><span data-stu-id="3a71f-108">driveItem</span></span>](driveitem.md)
* [<span data-ttu-id="3a71f-109">网站</span><span class="sxs-lookup"><span data-stu-id="3a71f-109">site</span></span>](site.md)
* [<span data-ttu-id="3a71f-110">sharedDriveItem</span><span class="sxs-lookup"><span data-stu-id="3a71f-110">sharedDriveItem</span></span>](shareddriveitem.md)

## <a name="json-representation"></a><span data-ttu-id="3a71f-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a71f-111">JSON representation</span></span>

<span data-ttu-id="3a71f-112">下面是 **baseItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a71f-112">Here is a JSON representation of a **baseItem** resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3a71f-113">属性</span><span class="sxs-lookup"><span data-stu-id="3a71f-113">Properties</span></span>

| <span data-ttu-id="3a71f-114">属性</span><span class="sxs-lookup"><span data-stu-id="3a71f-114">Property</span></span>             | <span data-ttu-id="3a71f-115">类型</span><span class="sxs-lookup"><span data-stu-id="3a71f-115">Type</span></span>              | <span data-ttu-id="3a71f-116">说明</span><span class="sxs-lookup"><span data-stu-id="3a71f-116">Description</span></span>                                                                            |
| :------------------- | :---------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="3a71f-117">ID</span><span class="sxs-lookup"><span data-stu-id="3a71f-117">id</span></span>                   | <span data-ttu-id="3a71f-118">string</span><span class="sxs-lookup"><span data-stu-id="3a71f-118">string</span></span>            | <span data-ttu-id="3a71f-p103">驱动器唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p103">The unique identifier of the drive. Read-only.</span></span>                                         |
| <span data-ttu-id="3a71f-121">createdBy</span><span class="sxs-lookup"><span data-stu-id="3a71f-121">createdBy</span></span>            | <span data-ttu-id="3a71f-122">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3a71f-122">[identitySet][]</span></span>   | <span data-ttu-id="3a71f-p104">识别创建项目的用户、设备或应用程序。只读。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p104">Identity of the user, device, or application which created the item. Read-only.</span></span>        |
| <span data-ttu-id="3a71f-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3a71f-125">createdDateTime</span></span>      | <span data-ttu-id="3a71f-126">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a71f-126">dateTimeOffset</span></span>    | <span data-ttu-id="3a71f-p105">创建项的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p105">Date and time of item creation. Read-only.</span></span>                                             |
| <span data-ttu-id="3a71f-129">eTag</span><span class="sxs-lookup"><span data-stu-id="3a71f-129">eTag</span></span>                 | <span data-ttu-id="3a71f-130">string</span><span class="sxs-lookup"><span data-stu-id="3a71f-130">string</span></span>            | <span data-ttu-id="3a71f-p106">该项目的 ETag。只读。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p106">ETag for the item. Read-only.</span></span>                                                          |
| <span data-ttu-id="3a71f-133">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="3a71f-133">lastModifiedBy</span></span>       | <span data-ttu-id="3a71f-134">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3a71f-134">[identitySet][]</span></span>   | <span data-ttu-id="3a71f-p107">上次修改项目的用户、设备和应用程序的标识。只读。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p107">Identity of the user, device, and application which last modified the item. Read-only.</span></span> |
| <span data-ttu-id="3a71f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3a71f-137">lastModifiedDateTime</span></span> | <span data-ttu-id="3a71f-138">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a71f-138">dateTimeOffset</span></span>    | <span data-ttu-id="3a71f-p108">上次修改项目的日期和时间。只读。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p108">Date and time the item was last modified. Read-only.</span></span>                                   |
| <span data-ttu-id="3a71f-141">name</span><span class="sxs-lookup"><span data-stu-id="3a71f-141">name</span></span>                 | <span data-ttu-id="3a71f-142">string</span><span class="sxs-lookup"><span data-stu-id="3a71f-142">string</span></span>            | <span data-ttu-id="3a71f-p109">项目名称。读写。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p109">The name of the item. Read-write.</span></span>                                                      |
| <span data-ttu-id="3a71f-145">parentReference</span><span class="sxs-lookup"><span data-stu-id="3a71f-145">parentReference</span></span>      | <span data-ttu-id="3a71f-146">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="3a71f-146">[itemReference][]</span></span> | <span data-ttu-id="3a71f-p110">父信息（如果此项具有父级）。读写。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p110">Parent information, if the item has a parent. Read-write.</span></span>                              |
| <span data-ttu-id="3a71f-149">WebUrl</span><span class="sxs-lookup"><span data-stu-id="3a71f-149">webUrl</span></span>               | <span data-ttu-id="3a71f-150">string (url)</span><span class="sxs-lookup"><span data-stu-id="3a71f-150">string (url)</span></span>      | <span data-ttu-id="3a71f-p111">在浏览器中显示此资源的 URL。只读。</span><span class="sxs-lookup"><span data-stu-id="3a71f-p111">URL that displays the resource in the browser. Read-only.</span></span>                              |

[identitySet]: identityset.md
[itemReference]: itemreference.md

## <a name="remarks"></a><span data-ttu-id="3a71f-155">注解</span><span class="sxs-lookup"><span data-stu-id="3a71f-155">Remarks</span></span>

<span data-ttu-id="3a71f-156">`baseItem` 类型不应直接使用。</span><span class="sxs-lookup"><span data-stu-id="3a71f-156">The `baseItem` type is not expected to be used directly.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/BaseItem"
} -->
