---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5330acfaa58cb5b1400851a861eb142d51b0ddb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355979"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="0aae0-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="0aae0-103">auditProperty resource type</span></span>

> <span data-ttu-id="0aae0-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0aae0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0aae0-105">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="0aae0-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="0aae0-106">属性</span><span class="sxs-lookup"><span data-stu-id="0aae0-106">Properties</span></span>
|<span data-ttu-id="0aae0-107">属性</span><span class="sxs-lookup"><span data-stu-id="0aae0-107">Property</span></span>|<span data-ttu-id="0aae0-108">类型</span><span class="sxs-lookup"><span data-stu-id="0aae0-108">Type</span></span>|<span data-ttu-id="0aae0-109">说明</span><span class="sxs-lookup"><span data-stu-id="0aae0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0aae0-110">displayName</span><span class="sxs-lookup"><span data-stu-id="0aae0-110">displayName</span></span>|<span data-ttu-id="0aae0-111">String</span><span class="sxs-lookup"><span data-stu-id="0aae0-111">String</span></span>|<span data-ttu-id="0aae0-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="0aae0-112">Display name.</span></span>|
|<span data-ttu-id="0aae0-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="0aae0-113">oldValue</span></span>|<span data-ttu-id="0aae0-114">String</span><span class="sxs-lookup"><span data-stu-id="0aae0-114">String</span></span>|<span data-ttu-id="0aae0-115">旧值。</span><span class="sxs-lookup"><span data-stu-id="0aae0-115">Old value.</span></span>|
|<span data-ttu-id="0aae0-116">NewValue</span><span class="sxs-lookup"><span data-stu-id="0aae0-116">newValue</span></span>|<span data-ttu-id="0aae0-117">String</span><span class="sxs-lookup"><span data-stu-id="0aae0-117">String</span></span>|<span data-ttu-id="0aae0-118">新值。</span><span class="sxs-lookup"><span data-stu-id="0aae0-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0aae0-119">关系</span><span class="sxs-lookup"><span data-stu-id="0aae0-119">Relationships</span></span>
<span data-ttu-id="0aae0-120">无</span><span class="sxs-lookup"><span data-stu-id="0aae0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0aae0-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0aae0-121">JSON Representation</span></span>
<span data-ttu-id="0aae0-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aae0-122">Here is a JSON representation of the resource.</span></span>
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




