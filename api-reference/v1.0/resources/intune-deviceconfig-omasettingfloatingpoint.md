---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17883b580671517bcdee88d95f1ac5a424e707da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073017"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="78502-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="78502-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="78502-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78502-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78502-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78502-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78502-106">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="78502-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="78502-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78502-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="78502-108">属性</span><span class="sxs-lookup"><span data-stu-id="78502-108">Properties</span></span>
|<span data-ttu-id="78502-109">属性</span><span class="sxs-lookup"><span data-stu-id="78502-109">Property</span></span>|<span data-ttu-id="78502-110">类型</span><span class="sxs-lookup"><span data-stu-id="78502-110">Type</span></span>|<span data-ttu-id="78502-111">说明</span><span class="sxs-lookup"><span data-stu-id="78502-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78502-112">displayName</span><span class="sxs-lookup"><span data-stu-id="78502-112">displayName</span></span>|<span data-ttu-id="78502-113">String</span><span class="sxs-lookup"><span data-stu-id="78502-113">String</span></span>|<span data-ttu-id="78502-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="78502-114">Display Name.</span></span> <span data-ttu-id="78502-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78502-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="78502-116">description</span><span class="sxs-lookup"><span data-stu-id="78502-116">description</span></span>|<span data-ttu-id="78502-117">String</span><span class="sxs-lookup"><span data-stu-id="78502-117">String</span></span>|<span data-ttu-id="78502-118">说明。</span><span class="sxs-lookup"><span data-stu-id="78502-118">Description.</span></span> <span data-ttu-id="78502-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78502-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="78502-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="78502-120">omaUri</span></span>|<span data-ttu-id="78502-121">String</span><span class="sxs-lookup"><span data-stu-id="78502-121">String</span></span>|<span data-ttu-id="78502-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="78502-122">OMA.</span></span> <span data-ttu-id="78502-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="78502-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="78502-124">value</span><span class="sxs-lookup"><span data-stu-id="78502-124">value</span></span>|<span data-ttu-id="78502-125">单个</span><span class="sxs-lookup"><span data-stu-id="78502-125">Single</span></span>|<span data-ttu-id="78502-126">值。</span><span class="sxs-lookup"><span data-stu-id="78502-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78502-127">关系</span><span class="sxs-lookup"><span data-stu-id="78502-127">Relationships</span></span>
<span data-ttu-id="78502-128">无</span><span class="sxs-lookup"><span data-stu-id="78502-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78502-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78502-129">JSON Representation</span></span>
<span data-ttu-id="78502-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78502-130">Here is a JSON representation of the resource.</span></span>
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









