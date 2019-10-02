---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 79261fe777d6251ba3c08d87d5d5a3d26ee83b53
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359913"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="4c2c8-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="4c2c8-103">omaSettingString resource type</span></span>

> <span data-ttu-id="4c2c8-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c2c8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c2c8-105">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="4c2c8-105">OMA Settings String definition.</span></span>


<span data-ttu-id="4c2c8-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c2c8-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4c2c8-107">属性</span><span class="sxs-lookup"><span data-stu-id="4c2c8-107">Properties</span></span>
|<span data-ttu-id="4c2c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="4c2c8-108">Property</span></span>|<span data-ttu-id="4c2c8-109">类型</span><span class="sxs-lookup"><span data-stu-id="4c2c8-109">Type</span></span>|<span data-ttu-id="4c2c8-110">说明</span><span class="sxs-lookup"><span data-stu-id="4c2c8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c2c8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4c2c8-111">displayName</span></span>|<span data-ttu-id="4c2c8-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4c2c8-112">String</span></span>|<span data-ttu-id="4c2c8-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="4c2c8-113">Display Name.</span></span> <span data-ttu-id="4c2c8-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c2c8-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4c2c8-115">说明</span><span class="sxs-lookup"><span data-stu-id="4c2c8-115">description</span></span>|<span data-ttu-id="4c2c8-116">String</span><span class="sxs-lookup"><span data-stu-id="4c2c8-116">String</span></span>|<span data-ttu-id="4c2c8-117">说明。</span><span class="sxs-lookup"><span data-stu-id="4c2c8-117">Description.</span></span> <span data-ttu-id="4c2c8-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c2c8-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4c2c8-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4c2c8-119">omaUri</span></span>|<span data-ttu-id="4c2c8-120">String</span><span class="sxs-lookup"><span data-stu-id="4c2c8-120">String</span></span>|<span data-ttu-id="4c2c8-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="4c2c8-121">OMA.</span></span> <span data-ttu-id="4c2c8-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="4c2c8-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4c2c8-123">value</span><span class="sxs-lookup"><span data-stu-id="4c2c8-123">value</span></span>|<span data-ttu-id="4c2c8-124">String</span><span class="sxs-lookup"><span data-stu-id="4c2c8-124">String</span></span>|<span data-ttu-id="4c2c8-125">值。</span><span class="sxs-lookup"><span data-stu-id="4c2c8-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c2c8-126">关系</span><span class="sxs-lookup"><span data-stu-id="4c2c8-126">Relationships</span></span>
<span data-ttu-id="4c2c8-127">无</span><span class="sxs-lookup"><span data-stu-id="4c2c8-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c2c8-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4c2c8-128">JSON Representation</span></span>
<span data-ttu-id="4c2c8-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c2c8-129">Here is a JSON representation of the resource.</span></span>
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




