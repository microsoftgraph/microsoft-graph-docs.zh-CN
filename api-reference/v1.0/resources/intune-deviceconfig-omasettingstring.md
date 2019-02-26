---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b32d5f6942dc5c0284e0ecaa11a27f4df0e99b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259911"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="d3028-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3028-103">omaSettingString resource type</span></span>

> <span data-ttu-id="d3028-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3028-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3028-105">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="d3028-105">OMA Settings String definition.</span></span>


<span data-ttu-id="d3028-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3028-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3028-107">属性</span><span class="sxs-lookup"><span data-stu-id="d3028-107">Properties</span></span>
|<span data-ttu-id="d3028-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3028-108">Property</span></span>|<span data-ttu-id="d3028-109">类型</span><span class="sxs-lookup"><span data-stu-id="d3028-109">Type</span></span>|<span data-ttu-id="d3028-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3028-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3028-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d3028-111">displayName</span></span>|<span data-ttu-id="d3028-112">String</span><span class="sxs-lookup"><span data-stu-id="d3028-112">String</span></span>|<span data-ttu-id="d3028-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="d3028-113">Display Name.</span></span> <span data-ttu-id="d3028-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3028-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3028-115">description</span><span class="sxs-lookup"><span data-stu-id="d3028-115">description</span></span>|<span data-ttu-id="d3028-116">String</span><span class="sxs-lookup"><span data-stu-id="d3028-116">String</span></span>|<span data-ttu-id="d3028-117">说明。</span><span class="sxs-lookup"><span data-stu-id="d3028-117">Description.</span></span> <span data-ttu-id="d3028-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3028-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3028-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d3028-119">omaUri</span></span>|<span data-ttu-id="d3028-120">String</span><span class="sxs-lookup"><span data-stu-id="d3028-120">String</span></span>|<span data-ttu-id="d3028-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="d3028-121">OMA.</span></span> <span data-ttu-id="d3028-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3028-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3028-123">值</span><span class="sxs-lookup"><span data-stu-id="d3028-123">value</span></span>|<span data-ttu-id="d3028-124">String</span><span class="sxs-lookup"><span data-stu-id="d3028-124">String</span></span>|<span data-ttu-id="d3028-125">值。</span><span class="sxs-lookup"><span data-stu-id="d3028-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3028-126">关系</span><span class="sxs-lookup"><span data-stu-id="d3028-126">Relationships</span></span>
<span data-ttu-id="d3028-127">无</span><span class="sxs-lookup"><span data-stu-id="d3028-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3028-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3028-128">JSON Representation</span></span>
<span data-ttu-id="d3028-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3028-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



