---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c0ecb59f45a83cc98c6ff060b46ba0c620dc9cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031337"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="cee88-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="cee88-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="cee88-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cee88-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cee88-105">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="cee88-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="cee88-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cee88-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cee88-107">属性</span><span class="sxs-lookup"><span data-stu-id="cee88-107">Properties</span></span>
|<span data-ttu-id="cee88-108">属性</span><span class="sxs-lookup"><span data-stu-id="cee88-108">Property</span></span>|<span data-ttu-id="cee88-109">类型</span><span class="sxs-lookup"><span data-stu-id="cee88-109">Type</span></span>|<span data-ttu-id="cee88-110">说明</span><span class="sxs-lookup"><span data-stu-id="cee88-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee88-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cee88-111">displayName</span></span>|<span data-ttu-id="cee88-112">字符串</span><span class="sxs-lookup"><span data-stu-id="cee88-112">String</span></span>|<span data-ttu-id="cee88-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="cee88-113">Display Name.</span></span> <span data-ttu-id="cee88-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cee88-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cee88-115">说明</span><span class="sxs-lookup"><span data-stu-id="cee88-115">description</span></span>|<span data-ttu-id="cee88-116">String</span><span class="sxs-lookup"><span data-stu-id="cee88-116">String</span></span>|<span data-ttu-id="cee88-117">说明。</span><span class="sxs-lookup"><span data-stu-id="cee88-117">Description.</span></span> <span data-ttu-id="cee88-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cee88-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cee88-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="cee88-119">omaUri</span></span>|<span data-ttu-id="cee88-120">String</span><span class="sxs-lookup"><span data-stu-id="cee88-120">String</span></span>|<span data-ttu-id="cee88-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="cee88-121">OMA.</span></span> <span data-ttu-id="cee88-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="cee88-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cee88-123">value</span><span class="sxs-lookup"><span data-stu-id="cee88-123">value</span></span>|<span data-ttu-id="cee88-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="cee88-124">Boolean</span></span>|<span data-ttu-id="cee88-125">值。</span><span class="sxs-lookup"><span data-stu-id="cee88-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cee88-126">关系</span><span class="sxs-lookup"><span data-stu-id="cee88-126">Relationships</span></span>
<span data-ttu-id="cee88-127">无</span><span class="sxs-lookup"><span data-stu-id="cee88-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cee88-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cee88-128">JSON Representation</span></span>
<span data-ttu-id="cee88-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cee88-129">Here is a JSON representation of the resource.</span></span>
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



