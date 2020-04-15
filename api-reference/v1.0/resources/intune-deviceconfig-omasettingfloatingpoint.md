---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b5db5b376bdce3d428b36c014c949087ab36185
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473024"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="fb3df-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb3df-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="fb3df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb3df-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb3df-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb3df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb3df-106">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="fb3df-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="fb3df-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fb3df-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fb3df-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb3df-108">Properties</span></span>
|<span data-ttu-id="fb3df-109">属性</span><span class="sxs-lookup"><span data-stu-id="fb3df-109">Property</span></span>|<span data-ttu-id="fb3df-110">类型</span><span class="sxs-lookup"><span data-stu-id="fb3df-110">Type</span></span>|<span data-ttu-id="fb3df-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb3df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb3df-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fb3df-112">displayName</span></span>|<span data-ttu-id="fb3df-113">字符串</span><span class="sxs-lookup"><span data-stu-id="fb3df-113">String</span></span>|<span data-ttu-id="fb3df-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="fb3df-114">Display Name.</span></span> <span data-ttu-id="fb3df-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fb3df-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fb3df-116">description</span><span class="sxs-lookup"><span data-stu-id="fb3df-116">description</span></span>|<span data-ttu-id="fb3df-117">String</span><span class="sxs-lookup"><span data-stu-id="fb3df-117">String</span></span>|<span data-ttu-id="fb3df-118">说明。</span><span class="sxs-lookup"><span data-stu-id="fb3df-118">Description.</span></span> <span data-ttu-id="fb3df-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fb3df-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fb3df-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="fb3df-120">omaUri</span></span>|<span data-ttu-id="fb3df-121">String</span><span class="sxs-lookup"><span data-stu-id="fb3df-121">String</span></span>|<span data-ttu-id="fb3df-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="fb3df-122">OMA.</span></span> <span data-ttu-id="fb3df-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fb3df-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fb3df-124">value</span><span class="sxs-lookup"><span data-stu-id="fb3df-124">value</span></span>|<span data-ttu-id="fb3df-125">单个</span><span class="sxs-lookup"><span data-stu-id="fb3df-125">Single</span></span>|<span data-ttu-id="fb3df-126">值。</span><span class="sxs-lookup"><span data-stu-id="fb3df-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb3df-127">关系</span><span class="sxs-lookup"><span data-stu-id="fb3df-127">Relationships</span></span>
<span data-ttu-id="fb3df-128">无</span><span class="sxs-lookup"><span data-stu-id="fb3df-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb3df-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb3df-129">JSON Representation</span></span>
<span data-ttu-id="fb3df-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb3df-130">Here is a JSON representation of the resource.</span></span>
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







