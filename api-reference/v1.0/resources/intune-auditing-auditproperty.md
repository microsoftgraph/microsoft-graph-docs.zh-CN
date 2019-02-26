---
title: auditProperty 资源类型
description: 包含审核属性的属性的类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e819234fd4ee7065378046f8ec977276a8c9f2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260611"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="41881-103">auditProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="41881-103">auditProperty resource type</span></span>

> <span data-ttu-id="41881-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="41881-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41881-105">包含审核属性的属性的类。</span><span class="sxs-lookup"><span data-stu-id="41881-105">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="41881-106">属性</span><span class="sxs-lookup"><span data-stu-id="41881-106">Properties</span></span>
|<span data-ttu-id="41881-107">属性</span><span class="sxs-lookup"><span data-stu-id="41881-107">Property</span></span>|<span data-ttu-id="41881-108">类型</span><span class="sxs-lookup"><span data-stu-id="41881-108">Type</span></span>|<span data-ttu-id="41881-109">说明</span><span class="sxs-lookup"><span data-stu-id="41881-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41881-110">displayName</span><span class="sxs-lookup"><span data-stu-id="41881-110">displayName</span></span>|<span data-ttu-id="41881-111">字符串</span><span class="sxs-lookup"><span data-stu-id="41881-111">String</span></span>|<span data-ttu-id="41881-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="41881-112">Display name.</span></span>|
|<span data-ttu-id="41881-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="41881-113">oldValue</span></span>|<span data-ttu-id="41881-114">String</span><span class="sxs-lookup"><span data-stu-id="41881-114">String</span></span>|<span data-ttu-id="41881-115">旧值。</span><span class="sxs-lookup"><span data-stu-id="41881-115">Old value.</span></span>|
|<span data-ttu-id="41881-116">NewValue</span><span class="sxs-lookup"><span data-stu-id="41881-116">newValue</span></span>|<span data-ttu-id="41881-117">String</span><span class="sxs-lookup"><span data-stu-id="41881-117">String</span></span>|<span data-ttu-id="41881-118">新值。</span><span class="sxs-lookup"><span data-stu-id="41881-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41881-119">关系</span><span class="sxs-lookup"><span data-stu-id="41881-119">Relationships</span></span>
<span data-ttu-id="41881-120">无</span><span class="sxs-lookup"><span data-stu-id="41881-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41881-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41881-121">JSON Representation</span></span>
<span data-ttu-id="41881-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41881-122">Here is a JSON representation of the resource.</span></span>
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



