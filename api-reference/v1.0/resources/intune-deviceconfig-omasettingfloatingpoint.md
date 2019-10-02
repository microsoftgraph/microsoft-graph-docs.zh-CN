---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e2f397d309f2199458595e3ed7d5cd4a204a1874
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359927"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="e0054-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0054-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="e0054-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0054-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0054-105">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="e0054-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="e0054-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0054-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0054-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0054-107">Properties</span></span>
|<span data-ttu-id="e0054-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0054-108">Property</span></span>|<span data-ttu-id="e0054-109">类型</span><span class="sxs-lookup"><span data-stu-id="e0054-109">Type</span></span>|<span data-ttu-id="e0054-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0054-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0054-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e0054-111">displayName</span></span>|<span data-ttu-id="e0054-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e0054-112">String</span></span>|<span data-ttu-id="e0054-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e0054-113">Display Name.</span></span> <span data-ttu-id="e0054-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0054-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0054-115">说明</span><span class="sxs-lookup"><span data-stu-id="e0054-115">description</span></span>|<span data-ttu-id="e0054-116">String</span><span class="sxs-lookup"><span data-stu-id="e0054-116">String</span></span>|<span data-ttu-id="e0054-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e0054-117">Description.</span></span> <span data-ttu-id="e0054-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0054-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0054-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e0054-119">omaUri</span></span>|<span data-ttu-id="e0054-120">String</span><span class="sxs-lookup"><span data-stu-id="e0054-120">String</span></span>|<span data-ttu-id="e0054-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e0054-121">OMA.</span></span> <span data-ttu-id="e0054-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0054-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0054-123">value</span><span class="sxs-lookup"><span data-stu-id="e0054-123">value</span></span>|<span data-ttu-id="e0054-124">单个</span><span class="sxs-lookup"><span data-stu-id="e0054-124">Single</span></span>|<span data-ttu-id="e0054-125">值。</span><span class="sxs-lookup"><span data-stu-id="e0054-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0054-126">关系</span><span class="sxs-lookup"><span data-stu-id="e0054-126">Relationships</span></span>
<span data-ttu-id="e0054-127">无</span><span class="sxs-lookup"><span data-stu-id="e0054-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0054-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0054-128">JSON Representation</span></span>
<span data-ttu-id="e0054-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0054-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```




