---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a36d30cb62862b469d7b32d742275d399ed36db0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888128"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="d8757-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8757-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="d8757-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d8757-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8757-105">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="d8757-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="d8757-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d8757-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d8757-107">属性</span><span class="sxs-lookup"><span data-stu-id="d8757-107">Properties</span></span>
|<span data-ttu-id="d8757-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8757-108">Property</span></span>|<span data-ttu-id="d8757-109">类型</span><span class="sxs-lookup"><span data-stu-id="d8757-109">Type</span></span>|<span data-ttu-id="d8757-110">说明</span><span class="sxs-lookup"><span data-stu-id="d8757-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8757-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d8757-111">displayName</span></span>|<span data-ttu-id="d8757-112">String</span><span class="sxs-lookup"><span data-stu-id="d8757-112">String</span></span>|<span data-ttu-id="d8757-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="d8757-113">Display Name.</span></span> <span data-ttu-id="d8757-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d8757-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d8757-115">description</span><span class="sxs-lookup"><span data-stu-id="d8757-115">description</span></span>|<span data-ttu-id="d8757-116">String</span><span class="sxs-lookup"><span data-stu-id="d8757-116">String</span></span>|<span data-ttu-id="d8757-117">说明。</span><span class="sxs-lookup"><span data-stu-id="d8757-117">Description.</span></span> <span data-ttu-id="d8757-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d8757-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d8757-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d8757-119">omaUri</span></span>|<span data-ttu-id="d8757-120">String</span><span class="sxs-lookup"><span data-stu-id="d8757-120">String</span></span>|<span data-ttu-id="d8757-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="d8757-121">OMA.</span></span> <span data-ttu-id="d8757-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d8757-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d8757-123">value</span><span class="sxs-lookup"><span data-stu-id="d8757-123">value</span></span>|<span data-ttu-id="d8757-124">单个</span><span class="sxs-lookup"><span data-stu-id="d8757-124">Single</span></span>|<span data-ttu-id="d8757-125">值。</span><span class="sxs-lookup"><span data-stu-id="d8757-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8757-126">关系</span><span class="sxs-lookup"><span data-stu-id="d8757-126">Relationships</span></span>
<span data-ttu-id="d8757-127">无</span><span class="sxs-lookup"><span data-stu-id="d8757-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d8757-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8757-128">JSON Representation</span></span>
<span data-ttu-id="d8757-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8757-129">Here is a JSON representation of the resource.</span></span>
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



