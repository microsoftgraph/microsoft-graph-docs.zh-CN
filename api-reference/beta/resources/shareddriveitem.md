---
author: JeremyKelley
description: 使用 Shares API 访问共享的 driveItem 时，返回 sharedDriveItem 资源。
ms.date: 09/10/2017
title: SharedDriveItem
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7d5af60c4ba5c67046909f6998d298444fa06d51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965157"
---
# <a name="shareddriveitem-resource-type"></a><span data-ttu-id="cde03-103">SharedDriveItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="cde03-103">SharedDriveItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cde03-104">使用 [Shares](../api/shares-get.md) API 访问共享的 [driveItem](driveitem.md) 时，返回 **sharedDriveItem** 资源。</span><span class="sxs-lookup"><span data-stu-id="cde03-104">The **sharedDriveItem** resource is returned when using the [Shares](../api/shares-get.md) API to access a shared [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="cde03-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cde03-105">JSON representation</span></span>

<span data-ttu-id="cde03-106">下面是 **sharedDriveItem** 资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cde03-106">Here is a JSON representation of the **sharedDriveItem** resource.</span></span>

<span data-ttu-id="cde03-107">**sharedDriveItem** 资源由 [**baseItem**](baseitem.md) 派生并继承该资源的属性。</span><span class="sxs-lookup"><span data-stu-id="cde03-107">The **sharedDriveItem** resource is derived from [**baseItem**](baseitem.md) and inherits properties from that resource.</span></span>

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
  "permission": { "@odata.type": "microsoft.graph.permission" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "site": { "@odata.type": "microsoft.graph.site" }
}
```

## <a name="properties"></a><span data-ttu-id="cde03-108">属性</span><span class="sxs-lookup"><span data-stu-id="cde03-108">Properties</span></span>

| <span data-ttu-id="cde03-109">属性</span><span class="sxs-lookup"><span data-stu-id="cde03-109">Property</span></span> | <span data-ttu-id="cde03-110">类型</span><span class="sxs-lookup"><span data-stu-id="cde03-110">Type</span></span>                          | <span data-ttu-id="cde03-111">说明</span><span class="sxs-lookup"><span data-stu-id="cde03-111">Description</span></span>                                                      |
| :------- | :---------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="cde03-112">id</span><span class="sxs-lookup"><span data-stu-id="cde03-112">id</span></span>       | <span data-ttu-id="cde03-113">String</span><span class="sxs-lookup"><span data-stu-id="cde03-113">String</span></span>                        | <span data-ttu-id="cde03-114">要访问的内容的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cde03-114">The unique identifier for the share being accessed.</span></span>              |
| <span data-ttu-id="cde03-115">name</span><span class="sxs-lookup"><span data-stu-id="cde03-115">name</span></span>     | <span data-ttu-id="cde03-116">String</span><span class="sxs-lookup"><span data-stu-id="cde03-116">String</span></span>                        | <span data-ttu-id="cde03-117">共享项的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cde03-117">The display name of the shared item.</span></span>                             |
| <span data-ttu-id="cde03-118">所有者</span><span class="sxs-lookup"><span data-stu-id="cde03-118">owner</span></span>    | [<span data-ttu-id="cde03-119">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="cde03-119">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="cde03-120">正在引用的共享项的所有者信息。</span><span class="sxs-lookup"><span data-stu-id="cde03-120">Information about the owner of the shared item being referenced.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cde03-121">关系</span><span class="sxs-lookup"><span data-stu-id="cde03-121">Relationships</span></span>

| <span data-ttu-id="cde03-122">关系名称</span><span class="sxs-lookup"><span data-stu-id="cde03-122">Relationship name</span></span> | <span data-ttu-id="cde03-123">类型</span><span class="sxs-lookup"><span data-stu-id="cde03-123">Type</span></span>                | <span data-ttu-id="cde03-124">说明</span><span class="sxs-lookup"><span data-stu-id="cde03-124">Description</span></span>
| ------------------|:--------------------|:-----------------------------------
| <span data-ttu-id="cde03-125">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="cde03-125">**driveItem**</span></span>     | <span data-ttu-id="cde03-126">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="cde03-126">[**driveItem**][driveItem]</span></span> | <span data-ttu-id="cde03-127">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="cde03-127">Used to access the underlying **driveItem**</span></span>
| <span data-ttu-id="cde03-128">**list**</span><span class="sxs-lookup"><span data-stu-id="cde03-128">**list**</span></span>          | <span data-ttu-id="cde03-129">[**簿**][list]</span><span class="sxs-lookup"><span data-stu-id="cde03-129">[**list**][list]</span></span>           | <span data-ttu-id="cde03-130">用于访问基础 **list**</span><span class="sxs-lookup"><span data-stu-id="cde03-130">Used to access the underlying **list**</span></span>
| <span data-ttu-id="cde03-131">**listItem**</span><span class="sxs-lookup"><span data-stu-id="cde03-131">**listItem**</span></span>      | <span data-ttu-id="cde03-132">[**listItem**][listItem]</span><span class="sxs-lookup"><span data-stu-id="cde03-132">[**listItem**][listItem]</span></span>   | <span data-ttu-id="cde03-133">用于访问基础 **listItem**</span><span class="sxs-lookup"><span data-stu-id="cde03-133">Used to access the underlying **listItem**</span></span>
| <span data-ttu-id="cde03-134">**权限**</span><span class="sxs-lookup"><span data-stu-id="cde03-134">**permission**</span></span>    | <span data-ttu-id="cde03-135">[**拒绝**][permission]</span><span class="sxs-lookup"><span data-stu-id="cde03-135">[**permission**][permission]</span></span> | <span data-ttu-id="cde03-136">用于访问代表基础共享链接的**权限**</span><span class="sxs-lookup"><span data-stu-id="cde03-136">Used to access the **permission** representing the underlying sharing link</span></span>
| <span data-ttu-id="cde03-137">**网站**</span><span class="sxs-lookup"><span data-stu-id="cde03-137">**site**</span></span>          | <span data-ttu-id="cde03-138">[**网站**][site]</span><span class="sxs-lookup"><span data-stu-id="cde03-138">[**site**][site]</span></span>           | <span data-ttu-id="cde03-139">用于访问基础 **site**</span><span class="sxs-lookup"><span data-stu-id="cde03-139">Used to access the underlying **site**</span></span>

<span data-ttu-id="cde03-140">另外，对于从个人 OneDrive 帐户共享的 **driveItems**，也可使用以下关系。</span><span class="sxs-lookup"><span data-stu-id="cde03-140">Alternatively, for **driveItems** shared from personal OneDrive accounts, the following relationships may also be used.</span></span>

| <span data-ttu-id="cde03-141">关系名称</span><span class="sxs-lookup"><span data-stu-id="cde03-141">Relationship name</span></span> | <span data-ttu-id="cde03-142">类型</span><span class="sxs-lookup"><span data-stu-id="cde03-142">Type</span></span>                         | <span data-ttu-id="cde03-143">说明</span><span class="sxs-lookup"><span data-stu-id="cde03-143">Description</span></span>
| ------------------|:-----------------------------|:-----------------------------------
| <span data-ttu-id="cde03-144">**items**</span><span class="sxs-lookup"><span data-stu-id="cde03-144">**items**</span></span>         | <span data-ttu-id="cde03-145">[**driveItem**][driveItem]集合</span><span class="sxs-lookup"><span data-stu-id="cde03-145">[**driveItem**][driveItem] collection</span></span> | <span data-ttu-id="cde03-146">共享根中包含的所有 driveItem。</span><span class="sxs-lookup"><span data-stu-id="cde03-146">All driveItems contained in the sharing root.</span></span> <span data-ttu-id="cde03-147">不能枚举该集合。</span><span class="sxs-lookup"><span data-stu-id="cde03-147">This collection cannot be enumerated.</span></span>
| <span data-ttu-id="cde03-148">**driveItem**</span><span class="sxs-lookup"><span data-stu-id="cde03-148">**driveItem**</span></span>     | <span data-ttu-id="cde03-149">[**driveItem**][driveItem]</span><span class="sxs-lookup"><span data-stu-id="cde03-149">[**driveItem**][driveItem]</span></span>            | <span data-ttu-id="cde03-150">用于访问基础 **driveItem**</span><span class="sxs-lookup"><span data-stu-id="cde03-150">Used to access the underlying **driveItem**</span></span>

[driveItem]: driveitem.md
[list]: list.md
[listItem]: listitem.md
[permission]: permission.md
[site]: site.md

## <a name="methods"></a><span data-ttu-id="cde03-151">方法</span><span class="sxs-lookup"><span data-stu-id="cde03-151">Methods</span></span>

| <span data-ttu-id="cde03-152">方法</span><span class="sxs-lookup"><span data-stu-id="cde03-152">Method</span></span>                                  | <span data-ttu-id="cde03-153">REST 路径</span><span class="sxs-lookup"><span data-stu-id="cde03-153">REST Path</span></span>                |
| :-------------------------------------- | :----------------------- |
| [<span data-ttu-id="cde03-154">获取共享项目</span><span class="sxs-lookup"><span data-stu-id="cde03-154">Get shared item</span></span>](../api/shares-get.md) | `GET /shares/{share-id}` |

## <a name="remarks"></a><span data-ttu-id="cde03-155">注解</span><span class="sxs-lookup"><span data-stu-id="cde03-155">Remarks</span></span>

<span data-ttu-id="cde03-156">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="cde03-156">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Share resource returns information about a shared item or collection of items.",
  "keywords": "share,shared,sharing root,shared files, shared items",
  "section": "documentation",
  "tocPath": "Resources/Share",
  "suppressions": []
}
-->
