---
title: windowsUpdateCatalogItem 资源类型
description: Windows 更新目录项实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6faffa482a2fc79e653eedf8a70a041f264d7d49
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863609"
---
# <a name="windowsupdatecatalogitem-resource-type"></a><span data-ttu-id="d6952-103">windowsUpdateCatalogItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6952-103">windowsUpdateCatalogItem resource type</span></span>

<span data-ttu-id="d6952-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6952-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6952-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6952-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6952-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6952-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6952-107">Windows 更新目录项实体</span><span class="sxs-lookup"><span data-stu-id="d6952-107">Windows update catalog item entity</span></span>

## <a name="methods"></a><span data-ttu-id="d6952-108">方法</span><span class="sxs-lookup"><span data-stu-id="d6952-108">Methods</span></span>
|<span data-ttu-id="d6952-109">方法</span><span class="sxs-lookup"><span data-stu-id="d6952-109">Method</span></span>|<span data-ttu-id="d6952-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d6952-110">Return Type</span></span>|<span data-ttu-id="d6952-111">说明</span><span class="sxs-lookup"><span data-stu-id="d6952-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6952-112">列出 windowsUpdateCatalogItems</span><span class="sxs-lookup"><span data-stu-id="d6952-112">List windowsUpdateCatalogItems</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|<span data-ttu-id="d6952-113">[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d6952-113">[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) collection</span></span>|<span data-ttu-id="d6952-114">列出 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6952-114">List properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) objects.</span></span>|
|[<span data-ttu-id="d6952-115">获取 windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="d6952-115">Get windowsUpdateCatalogItem</span></span>](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[<span data-ttu-id="d6952-116">windowsUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="d6952-116">windowsUpdateCatalogItem</span></span>](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|<span data-ttu-id="d6952-117">读取 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d6952-117">Read properties and relationships of the [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6952-118">属性</span><span class="sxs-lookup"><span data-stu-id="d6952-118">Properties</span></span>
|<span data-ttu-id="d6952-119">属性</span><span class="sxs-lookup"><span data-stu-id="d6952-119">Property</span></span>|<span data-ttu-id="d6952-120">类型</span><span class="sxs-lookup"><span data-stu-id="d6952-120">Type</span></span>|<span data-ttu-id="d6952-121">说明</span><span class="sxs-lookup"><span data-stu-id="d6952-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6952-122">id</span><span class="sxs-lookup"><span data-stu-id="d6952-122">id</span></span>|<span data-ttu-id="d6952-123">String</span><span class="sxs-lookup"><span data-stu-id="d6952-123">String</span></span>|<span data-ttu-id="d6952-124">目录项 ID。</span><span class="sxs-lookup"><span data-stu-id="d6952-124">The catalog item id.</span></span>|
|<span data-ttu-id="d6952-125">displayName</span><span class="sxs-lookup"><span data-stu-id="d6952-125">displayName</span></span>|<span data-ttu-id="d6952-126">String</span><span class="sxs-lookup"><span data-stu-id="d6952-126">String</span></span>|<span data-ttu-id="d6952-127">目录显示名称列表。</span><span class="sxs-lookup"><span data-stu-id="d6952-127">The display name for the catalog item.</span></span>|
|<span data-ttu-id="d6952-128">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="d6952-128">releaseDateTime</span></span>|<span data-ttu-id="d6952-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6952-129">DateTimeOffset</span></span>|<span data-ttu-id="d6952-130">目录项的发布日期</span><span class="sxs-lookup"><span data-stu-id="d6952-130">The date the catalog item was released</span></span>|
|<span data-ttu-id="d6952-131">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="d6952-131">endOfSupportDate</span></span>|<span data-ttu-id="d6952-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6952-132">DateTimeOffset</span></span>|<span data-ttu-id="d6952-133">目录项的上次支持日期</span><span class="sxs-lookup"><span data-stu-id="d6952-133">The last supported date for a catalog item</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6952-134">关系</span><span class="sxs-lookup"><span data-stu-id="d6952-134">Relationships</span></span>
<span data-ttu-id="d6952-135">无</span><span class="sxs-lookup"><span data-stu-id="d6952-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6952-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6952-136">JSON Representation</span></span>
<span data-ttu-id="d6952-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6952-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)"
}
```




