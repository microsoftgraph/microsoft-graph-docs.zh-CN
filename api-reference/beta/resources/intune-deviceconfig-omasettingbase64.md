---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f6eae88e7158d5fd8d09caadda9fee6778182a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166645"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="3adc3-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="3adc3-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="3adc3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3adc3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3adc3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3adc3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3adc3-106">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="3adc3-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="3adc3-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3adc3-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3adc3-108">属性</span><span class="sxs-lookup"><span data-stu-id="3adc3-108">Properties</span></span>
|<span data-ttu-id="3adc3-109">属性</span><span class="sxs-lookup"><span data-stu-id="3adc3-109">Property</span></span>|<span data-ttu-id="3adc3-110">类型</span><span class="sxs-lookup"><span data-stu-id="3adc3-110">Type</span></span>|<span data-ttu-id="3adc3-111">说明</span><span class="sxs-lookup"><span data-stu-id="3adc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3adc3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3adc3-112">displayName</span></span>|<span data-ttu-id="3adc3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="3adc3-113">String</span></span>|<span data-ttu-id="3adc3-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="3adc3-114">Display Name.</span></span> <span data-ttu-id="3adc3-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3adc3-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3adc3-116">description</span><span class="sxs-lookup"><span data-stu-id="3adc3-116">description</span></span>|<span data-ttu-id="3adc3-117">字符串</span><span class="sxs-lookup"><span data-stu-id="3adc3-117">String</span></span>|<span data-ttu-id="3adc3-118">说明。</span><span class="sxs-lookup"><span data-stu-id="3adc3-118">Description.</span></span> <span data-ttu-id="3adc3-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3adc3-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3adc3-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="3adc3-120">omaUri</span></span>|<span data-ttu-id="3adc3-121">字符串</span><span class="sxs-lookup"><span data-stu-id="3adc3-121">String</span></span>|<span data-ttu-id="3adc3-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="3adc3-122">OMA.</span></span> <span data-ttu-id="3adc3-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="3adc3-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="3adc3-124">fileName</span><span class="sxs-lookup"><span data-stu-id="3adc3-124">fileName</span></span>|<span data-ttu-id="3adc3-125">String</span><span class="sxs-lookup"><span data-stu-id="3adc3-125">String</span></span>|<span data-ttu-id="3adc3-126">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="3adc3-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="3adc3-127">\* .crt</span><span class="sxs-lookup"><span data-stu-id="3adc3-127">\*.crt</span></span> | <span data-ttu-id="3adc3-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="3adc3-128">\*.p7b</span></span> | <span data-ttu-id="3adc3-129">\* bin)。</span><span class="sxs-lookup"><span data-stu-id="3adc3-129">\*.bin).</span></span>|
|<span data-ttu-id="3adc3-130">值</span><span class="sxs-lookup"><span data-stu-id="3adc3-130">value</span></span>|<span data-ttu-id="3adc3-131">String</span><span class="sxs-lookup"><span data-stu-id="3adc3-131">String</span></span>|<span data-ttu-id="3adc3-132">值。</span><span class="sxs-lookup"><span data-stu-id="3adc3-132">Value.</span></span> <span data-ttu-id="3adc3-133">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="3adc3-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3adc3-134">关系</span><span class="sxs-lookup"><span data-stu-id="3adc3-134">Relationships</span></span>
<span data-ttu-id="3adc3-135">无</span><span class="sxs-lookup"><span data-stu-id="3adc3-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3adc3-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3adc3-136">JSON Representation</span></span>
<span data-ttu-id="3adc3-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3adc3-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```




