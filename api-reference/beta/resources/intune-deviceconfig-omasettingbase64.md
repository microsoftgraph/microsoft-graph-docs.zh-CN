---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ff036a8d3bac70193f9653f42fb5380a8d1f0fbf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084903"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="8ebea-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ebea-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="8ebea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ebea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ebea-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ebea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ebea-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ebea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ebea-107">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="8ebea-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="8ebea-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ebea-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ebea-109">属性</span><span class="sxs-lookup"><span data-stu-id="8ebea-109">Properties</span></span>
|<span data-ttu-id="8ebea-110">属性</span><span class="sxs-lookup"><span data-stu-id="8ebea-110">Property</span></span>|<span data-ttu-id="8ebea-111">类型</span><span class="sxs-lookup"><span data-stu-id="8ebea-111">Type</span></span>|<span data-ttu-id="8ebea-112">说明</span><span class="sxs-lookup"><span data-stu-id="8ebea-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ebea-113">displayName</span><span class="sxs-lookup"><span data-stu-id="8ebea-113">displayName</span></span>|<span data-ttu-id="8ebea-114">字符串</span><span class="sxs-lookup"><span data-stu-id="8ebea-114">String</span></span>|<span data-ttu-id="8ebea-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="8ebea-115">Display Name.</span></span> <span data-ttu-id="8ebea-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ebea-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8ebea-117">说明</span><span class="sxs-lookup"><span data-stu-id="8ebea-117">description</span></span>|<span data-ttu-id="8ebea-118">字符串</span><span class="sxs-lookup"><span data-stu-id="8ebea-118">String</span></span>|<span data-ttu-id="8ebea-119">说明。</span><span class="sxs-lookup"><span data-stu-id="8ebea-119">Description.</span></span> <span data-ttu-id="8ebea-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ebea-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8ebea-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="8ebea-121">omaUri</span></span>|<span data-ttu-id="8ebea-122">String</span><span class="sxs-lookup"><span data-stu-id="8ebea-122">String</span></span>|<span data-ttu-id="8ebea-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="8ebea-123">OMA.</span></span> <span data-ttu-id="8ebea-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="8ebea-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8ebea-125">fileName</span><span class="sxs-lookup"><span data-stu-id="8ebea-125">fileName</span></span>|<span data-ttu-id="8ebea-126">String</span><span class="sxs-lookup"><span data-stu-id="8ebea-126">String</span></span>|<span data-ttu-id="8ebea-127">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="8ebea-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="8ebea-128">\* .crt</span><span class="sxs-lookup"><span data-stu-id="8ebea-128">\*.crt</span></span> | <span data-ttu-id="8ebea-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="8ebea-129">\*.p7b</span></span> | <span data-ttu-id="8ebea-130">\* bin) 。</span><span class="sxs-lookup"><span data-stu-id="8ebea-130">\*.bin).</span></span>|
|<span data-ttu-id="8ebea-131">value</span><span class="sxs-lookup"><span data-stu-id="8ebea-131">value</span></span>|<span data-ttu-id="8ebea-132">String</span><span class="sxs-lookup"><span data-stu-id="8ebea-132">String</span></span>|<span data-ttu-id="8ebea-133">值。</span><span class="sxs-lookup"><span data-stu-id="8ebea-133">Value.</span></span> <span data-ttu-id="8ebea-134">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="8ebea-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ebea-135">关系</span><span class="sxs-lookup"><span data-stu-id="8ebea-135">Relationships</span></span>
<span data-ttu-id="8ebea-136">无</span><span class="sxs-lookup"><span data-stu-id="8ebea-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ebea-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ebea-137">JSON Representation</span></span>
<span data-ttu-id="8ebea-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ebea-138">Here is a JSON representation of the resource.</span></span>
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






