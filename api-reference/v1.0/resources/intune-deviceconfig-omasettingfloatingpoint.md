---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ba82e79c16d8aeebd591f55849df74febad0073b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755873"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="ce867-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce867-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="ce867-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce867-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce867-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce867-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce867-106">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="ce867-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="ce867-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce867-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce867-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce867-108">Properties</span></span>
|<span data-ttu-id="ce867-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce867-109">Property</span></span>|<span data-ttu-id="ce867-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce867-110">Type</span></span>|<span data-ttu-id="ce867-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce867-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce867-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ce867-112">displayName</span></span>|<span data-ttu-id="ce867-113">String</span><span class="sxs-lookup"><span data-stu-id="ce867-113">String</span></span>|<span data-ttu-id="ce867-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ce867-114">Display Name.</span></span> <span data-ttu-id="ce867-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce867-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce867-116">说明</span><span class="sxs-lookup"><span data-stu-id="ce867-116">description</span></span>|<span data-ttu-id="ce867-117">String</span><span class="sxs-lookup"><span data-stu-id="ce867-117">String</span></span>|<span data-ttu-id="ce867-118">说明。</span><span class="sxs-lookup"><span data-stu-id="ce867-118">Description.</span></span> <span data-ttu-id="ce867-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce867-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce867-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="ce867-120">omaUri</span></span>|<span data-ttu-id="ce867-121">String</span><span class="sxs-lookup"><span data-stu-id="ce867-121">String</span></span>|<span data-ttu-id="ce867-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="ce867-122">OMA.</span></span> <span data-ttu-id="ce867-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce867-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce867-124">value</span><span class="sxs-lookup"><span data-stu-id="ce867-124">value</span></span>|<span data-ttu-id="ce867-125">单个</span><span class="sxs-lookup"><span data-stu-id="ce867-125">Single</span></span>|<span data-ttu-id="ce867-126">值。</span><span class="sxs-lookup"><span data-stu-id="ce867-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce867-127">关系</span><span class="sxs-lookup"><span data-stu-id="ce867-127">Relationships</span></span>
<span data-ttu-id="ce867-128">无</span><span class="sxs-lookup"><span data-stu-id="ce867-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce867-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce867-129">JSON Representation</span></span>
<span data-ttu-id="ce867-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce867-130">Here is a JSON representation of the resource.</span></span>
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
  "value": 4.2
}
```




