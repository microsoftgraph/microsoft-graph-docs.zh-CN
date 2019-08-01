---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f80f8583907a25646643fdd5770d6bce5adcb4b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028019"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="ee5c4-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee5c4-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="ee5c4-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ee5c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee5c4-105">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="ee5c4-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="ee5c4-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c4-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ee5c4-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee5c4-107">Properties</span></span>
|<span data-ttu-id="ee5c4-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee5c4-108">Property</span></span>|<span data-ttu-id="ee5c4-109">类型</span><span class="sxs-lookup"><span data-stu-id="ee5c4-109">Type</span></span>|<span data-ttu-id="ee5c4-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee5c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee5c4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="ee5c4-111">displayName</span></span>|<span data-ttu-id="ee5c4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="ee5c4-112">String</span></span>|<span data-ttu-id="ee5c4-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ee5c4-113">Display Name.</span></span> <span data-ttu-id="ee5c4-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c4-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ee5c4-115">说明</span><span class="sxs-lookup"><span data-stu-id="ee5c4-115">description</span></span>|<span data-ttu-id="ee5c4-116">String</span><span class="sxs-lookup"><span data-stu-id="ee5c4-116">String</span></span>|<span data-ttu-id="ee5c4-117">说明。</span><span class="sxs-lookup"><span data-stu-id="ee5c4-117">Description.</span></span> <span data-ttu-id="ee5c4-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c4-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ee5c4-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="ee5c4-119">omaUri</span></span>|<span data-ttu-id="ee5c4-120">String</span><span class="sxs-lookup"><span data-stu-id="ee5c4-120">String</span></span>|<span data-ttu-id="ee5c4-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="ee5c4-121">OMA.</span></span> <span data-ttu-id="ee5c4-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ee5c4-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ee5c4-123">值</span><span class="sxs-lookup"><span data-stu-id="ee5c4-123">value</span></span>|<span data-ttu-id="ee5c4-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ee5c4-124">Int32</span></span>|<span data-ttu-id="ee5c4-125">值。</span><span class="sxs-lookup"><span data-stu-id="ee5c4-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee5c4-126">关系</span><span class="sxs-lookup"><span data-stu-id="ee5c4-126">Relationships</span></span>
<span data-ttu-id="ee5c4-127">无</span><span class="sxs-lookup"><span data-stu-id="ee5c4-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee5c4-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee5c4-128">JSON Representation</span></span>
<span data-ttu-id="ee5c4-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee5c4-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



