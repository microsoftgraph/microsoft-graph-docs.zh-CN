---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f1f5cc213f99300811c627692a516ac8c0b6e89
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797421"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="a7f32-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="a7f32-103">auditProperty resource type</span></span>

> <span data-ttu-id="a7f32-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7f32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7f32-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7f32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7f32-106">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="a7f32-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="a7f32-107">属性</span><span class="sxs-lookup"><span data-stu-id="a7f32-107">Properties</span></span>
|<span data-ttu-id="a7f32-108">属性</span><span class="sxs-lookup"><span data-stu-id="a7f32-108">Property</span></span>|<span data-ttu-id="a7f32-109">类型</span><span class="sxs-lookup"><span data-stu-id="a7f32-109">Type</span></span>|<span data-ttu-id="a7f32-110">说明</span><span class="sxs-lookup"><span data-stu-id="a7f32-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7f32-111">displayName</span><span class="sxs-lookup"><span data-stu-id="a7f32-111">displayName</span></span>|<span data-ttu-id="a7f32-112">String</span><span class="sxs-lookup"><span data-stu-id="a7f32-112">String</span></span>|<span data-ttu-id="a7f32-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="a7f32-113">Display name.</span></span>|
|<span data-ttu-id="a7f32-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="a7f32-114">oldValue</span></span>|<span data-ttu-id="a7f32-115">String</span><span class="sxs-lookup"><span data-stu-id="a7f32-115">String</span></span>|<span data-ttu-id="a7f32-116">旧值。</span><span class="sxs-lookup"><span data-stu-id="a7f32-116">Old value.</span></span>|
|<span data-ttu-id="a7f32-117">NewValue</span><span class="sxs-lookup"><span data-stu-id="a7f32-117">newValue</span></span>|<span data-ttu-id="a7f32-118">String</span><span class="sxs-lookup"><span data-stu-id="a7f32-118">String</span></span>|<span data-ttu-id="a7f32-119">新值。</span><span class="sxs-lookup"><span data-stu-id="a7f32-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7f32-120">关系</span><span class="sxs-lookup"><span data-stu-id="a7f32-120">Relationships</span></span>
<span data-ttu-id="a7f32-121">无</span><span class="sxs-lookup"><span data-stu-id="a7f32-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7f32-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7f32-122">JSON Representation</span></span>
<span data-ttu-id="a7f32-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7f32-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



