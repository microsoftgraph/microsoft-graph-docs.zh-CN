---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d202997cdf0c1325e887337842513cc30dd2941
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256390"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="4379f-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="4379f-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="4379f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4379f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4379f-105">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="4379f-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="4379f-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4379f-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4379f-107">属性</span><span class="sxs-lookup"><span data-stu-id="4379f-107">Properties</span></span>
|<span data-ttu-id="4379f-108">属性</span><span class="sxs-lookup"><span data-stu-id="4379f-108">Property</span></span>|<span data-ttu-id="4379f-109">类型</span><span class="sxs-lookup"><span data-stu-id="4379f-109">Type</span></span>|<span data-ttu-id="4379f-110">说明</span><span class="sxs-lookup"><span data-stu-id="4379f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4379f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4379f-111">displayName</span></span>|<span data-ttu-id="4379f-112">String</span><span class="sxs-lookup"><span data-stu-id="4379f-112">String</span></span>|<span data-ttu-id="4379f-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="4379f-113">Display Name.</span></span> <span data-ttu-id="4379f-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4379f-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4379f-115">description</span><span class="sxs-lookup"><span data-stu-id="4379f-115">description</span></span>|<span data-ttu-id="4379f-116">String</span><span class="sxs-lookup"><span data-stu-id="4379f-116">String</span></span>|<span data-ttu-id="4379f-117">说明。</span><span class="sxs-lookup"><span data-stu-id="4379f-117">Description.</span></span> <span data-ttu-id="4379f-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4379f-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4379f-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4379f-119">omaUri</span></span>|<span data-ttu-id="4379f-120">String</span><span class="sxs-lookup"><span data-stu-id="4379f-120">String</span></span>|<span data-ttu-id="4379f-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="4379f-121">OMA.</span></span> <span data-ttu-id="4379f-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4379f-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4379f-123">value</span><span class="sxs-lookup"><span data-stu-id="4379f-123">value</span></span>|<span data-ttu-id="4379f-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4379f-124">Boolean</span></span>|<span data-ttu-id="4379f-125">值。</span><span class="sxs-lookup"><span data-stu-id="4379f-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4379f-126">关系</span><span class="sxs-lookup"><span data-stu-id="4379f-126">Relationships</span></span>
<span data-ttu-id="4379f-127">无</span><span class="sxs-lookup"><span data-stu-id="4379f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4379f-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4379f-128">JSON Representation</span></span>
<span data-ttu-id="4379f-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4379f-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



