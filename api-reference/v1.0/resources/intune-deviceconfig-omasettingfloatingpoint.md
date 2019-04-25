---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4720d635eeb119a2e1cacc741ab9c96f8ac55d4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568995"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="e0df7-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0df7-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="e0df7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0df7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0df7-105">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="e0df7-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="e0df7-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0df7-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0df7-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0df7-107">Properties</span></span>
|<span data-ttu-id="e0df7-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0df7-108">Property</span></span>|<span data-ttu-id="e0df7-109">类型</span><span class="sxs-lookup"><span data-stu-id="e0df7-109">Type</span></span>|<span data-ttu-id="e0df7-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0df7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0df7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e0df7-111">displayName</span></span>|<span data-ttu-id="e0df7-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e0df7-112">String</span></span>|<span data-ttu-id="e0df7-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e0df7-113">Display Name.</span></span> <span data-ttu-id="e0df7-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0df7-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0df7-115">说明</span><span class="sxs-lookup"><span data-stu-id="e0df7-115">description</span></span>|<span data-ttu-id="e0df7-116">String</span><span class="sxs-lookup"><span data-stu-id="e0df7-116">String</span></span>|<span data-ttu-id="e0df7-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e0df7-117">Description.</span></span> <span data-ttu-id="e0df7-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0df7-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0df7-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e0df7-119">omaUri</span></span>|<span data-ttu-id="e0df7-120">String</span><span class="sxs-lookup"><span data-stu-id="e0df7-120">String</span></span>|<span data-ttu-id="e0df7-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e0df7-121">OMA.</span></span> <span data-ttu-id="e0df7-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e0df7-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0df7-123">value</span><span class="sxs-lookup"><span data-stu-id="e0df7-123">value</span></span>|<span data-ttu-id="e0df7-124">单个</span><span class="sxs-lookup"><span data-stu-id="e0df7-124">Single</span></span>|<span data-ttu-id="e0df7-125">值。</span><span class="sxs-lookup"><span data-stu-id="e0df7-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0df7-126">关系</span><span class="sxs-lookup"><span data-stu-id="e0df7-126">Relationships</span></span>
<span data-ttu-id="e0df7-127">无</span><span class="sxs-lookup"><span data-stu-id="e0df7-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0df7-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0df7-128">JSON Representation</span></span>
<span data-ttu-id="e0df7-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0df7-129">Here is a JSON representation of the resource.</span></span>
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



