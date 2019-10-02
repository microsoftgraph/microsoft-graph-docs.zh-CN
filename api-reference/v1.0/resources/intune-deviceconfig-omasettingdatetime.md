---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4405f8446ceb76dbdd5b4c9df1407ee14861a3b8
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360795"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="e10f9-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="e10f9-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="e10f9-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e10f9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e10f9-105">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="e10f9-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="e10f9-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10f9-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e10f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="e10f9-107">Properties</span></span>
|<span data-ttu-id="e10f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="e10f9-108">Property</span></span>|<span data-ttu-id="e10f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="e10f9-109">Type</span></span>|<span data-ttu-id="e10f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="e10f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10f9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e10f9-111">displayName</span></span>|<span data-ttu-id="e10f9-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e10f9-112">String</span></span>|<span data-ttu-id="e10f9-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e10f9-113">Display Name.</span></span> <span data-ttu-id="e10f9-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10f9-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e10f9-115">说明</span><span class="sxs-lookup"><span data-stu-id="e10f9-115">description</span></span>|<span data-ttu-id="e10f9-116">String</span><span class="sxs-lookup"><span data-stu-id="e10f9-116">String</span></span>|<span data-ttu-id="e10f9-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e10f9-117">Description.</span></span> <span data-ttu-id="e10f9-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10f9-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e10f9-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e10f9-119">omaUri</span></span>|<span data-ttu-id="e10f9-120">String</span><span class="sxs-lookup"><span data-stu-id="e10f9-120">String</span></span>|<span data-ttu-id="e10f9-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e10f9-121">OMA.</span></span> <span data-ttu-id="e10f9-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e10f9-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e10f9-123">value</span><span class="sxs-lookup"><span data-stu-id="e10f9-123">value</span></span>|<span data-ttu-id="e10f9-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e10f9-124">DateTimeOffset</span></span>|<span data-ttu-id="e10f9-125">值。</span><span class="sxs-lookup"><span data-stu-id="e10f9-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e10f9-126">关系</span><span class="sxs-lookup"><span data-stu-id="e10f9-126">Relationships</span></span>
<span data-ttu-id="e10f9-127">无</span><span class="sxs-lookup"><span data-stu-id="e10f9-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e10f9-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e10f9-128">JSON Representation</span></span>
<span data-ttu-id="e10f9-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e10f9-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```




