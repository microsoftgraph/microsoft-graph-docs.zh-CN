---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
description: 使用 Shares API 访问共享的 driveItem 时，返回 sharedDriveItem 资源。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 10e6146151b64470386b6071bc19cb8764744b3e
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43934897"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="f4421-103">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f4421-103">SharedDriveItem resource type</span></span>

<span data-ttu-id="f4421-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4421-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4421-105">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="f4421-105">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f4421-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4421-106">JSON representation</span></span>

<span data-ttu-id="f4421-107">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4421-107">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="f4421-108">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="f4421-108">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItem",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.sharedDriveItem"
}-->

```json
{
  "id": "string",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },

  "driveItem": { "@odata.type": "microsoft.graph.driveItem" },
  "items": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "list": { "@odata.type": "microsoft.graph.list" },
  "listItem": { "@odata.type": "microsoft.graph.listItem" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="f4421-109">属性</span><span class="sxs-lookup"><span data-stu-id="f4421-109">Properties</span></span>

| <span data-ttu-id="f4421-110">属性</span><span class="sxs-lookup"><span data-stu-id="f4421-110">Property</span></span> | <span data-ttu-id="f4421-111">类型</span><span class="sxs-lookup"><span data-stu-id="f4421-111">Type</span></span>                          | <span data-ttu-id="f4421-112">说明</span><span class="sxs-lookup"><span data-stu-id="f4421-112">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="f4421-113">id</span><span class="sxs-lookup"><span data-stu-id="f4421-113">id</span></span>       | <span data-ttu-id="f4421-114">String</span><span class="sxs-lookup"><span data-stu-id="f4421-114">String</span></span>                        | <span data-ttu-id="f4421-115">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4421-115">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="f4421-116">name</span><span class="sxs-lookup"><span data-stu-id="f4421-116">name</span></span>     | <span data-ttu-id="f4421-117">字符串</span><span class="sxs-lookup"><span data-stu-id="f4421-117">String</span></span>                        | <span data-ttu-id="f4421-118">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f4421-118">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="f4421-119">所有者</span><span class="sxs-lookup"><span data-stu-id="f4421-119">owner</span></span>    | [<span data-ttu-id="f4421-120">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="f4421-120">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="f4421-121">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="f4421-121">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f4421-122">关系</span><span class="sxs-lookup"><span data-stu-id="f4421-122">Relationships</span></span>

| <span data-ttu-id="f4421-123">关系名称</span><span class="sxs-lookup"><span data-stu-id="f4421-123">Relationship name</span></span> | <span data-ttu-id="f4421-124">类型</span><span class="sxs-lookup"><span data-stu-id="f4421-124">Type</span></span>                | <span data-ttu-id="f4421-125">说明</span><span class="sxs-lookup"><span data-stu-id="f4421-125">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="f4421-126">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="f4421-126">**driveItem**</span></span>     | <span data-ttu-id="f4421-127">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f4421-127">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="f4421-128">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="f4421-128">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="f4421-129">**list**</span><span class="sxs-lookup"><span data-stu-id="f4421-129">**list**</span></span>          | <span data-ttu-id="f4421-130">[**簿**][list]</span><span class="sxs-lookup"><span data-stu-id="f4421-130">[**list**][list]</span></span>        | <span data-ttu-id="f4421-131">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="f4421-131">Used to access the underlying **list**</span></span>
| <span data-ttu-id="f4421-132">**listItem**</span><span class="sxs-lookup"><span data-stu-id="f4421-132">**listItem**</span></span>      | <span data-ttu-id="f4421-133">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="f4421-133">[**listItem**][listItem]</span></span>    | <span data-ttu-id="f4421-134">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="f4421-134">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="f4421-135">**权限**</span><span class="sxs-lookup"><span data-stu-id="f4421-135">**permission**</span></span>    | <span data-ttu-id="f4421-136">[**拒绝**][permission]</span><span class="sxs-lookup"><span data-stu-id="f4421-136">[**permission**][permission]</span></span> | <span data-ttu-id="f4421-137">用于访问代表基础共享链接的**权限**</span><span class="sxs-lookup"><span data-stu-id="f4421-137">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="f4421-138">**网站**</span><span class="sxs-lookup"><span data-stu-id="f4421-138">**site**</span></span>          | <span data-ttu-id="f4421-139">[**网站**][site]</span><span class="sxs-lookup"><span data-stu-id="f4421-139">[**site**][site]</span></span>        | <span data-ttu-id="f4421-140">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="f4421-140">Used to access the underlying **site**</span></span>

<span data-ttu-id="f4421-141">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="f4421-141">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="f4421-142">关系名称</span><span class="sxs-lookup"><span data-stu-id="f4421-142">Relationship name</span></span> | <span data-ttu-id="f4421-143">类型</span><span class="sxs-lookup"><span data-stu-id="f4421-143">Type</span></span>                         | <span data-ttu-id="f4421-144">说明</span><span class="sxs-lookup"><span data-stu-id="f4421-144">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="f4421-145">**items**</span><span class="sxs-lookup"><span data-stu-id="f4421-145">**items**</span></span>         | <span data-ttu-id="f4421-146">[**driveItem**][driveItem]集合</span><span class="sxs-lookup"><span data-stu-id="f4421-146">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="f4421-147">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="f4421-147">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="f4421-148">不能枚举此集合。</span><span class="sxs-lookup"><span data-stu-id="f4421-148">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="f4421-149">**root**</span><span class="sxs-lookup"><span data-stu-id="f4421-149">**root**</span></span>          | <span data-ttu-id="f4421-150">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="f4421-150">[**driveItem**][driveItem]</span></span>   | <span data-ttu-id="f4421-151">用于访问基础**driveItem**。</span><span class="sxs-lookup"><span data-stu-id="f4421-151">Used to access the underlying **driveItem**.</span></span> <span data-ttu-id="f4421-152">已弃用-- `driveItem`改用。</span><span class="sxs-lookup"><span data-stu-id="f4421-152">Deprecated -- use `driveItem` instead.</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="f4421-153">Methods</span><span class="sxs-lookup"><span data-stu-id="f4421-153">Methods</span></span>

| <span data-ttu-id="f4421-154">方法</span><span class="sxs-lookup"><span data-stu-id="f4421-154">Method</span></span>                                  | <span data-ttu-id="f4421-155">REST 路径</span><span class="sxs-lookup"><span data-stu-id="f4421-155">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="f4421-156">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="f4421-156">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="f4421-157">注解</span><span class="sxs-lookup"><span data-stu-id="f4421-157">Remarks</span></span>

<span data-ttu-id="f4421-158">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f4421-158">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share"
} -->
