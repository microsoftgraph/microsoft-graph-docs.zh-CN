---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3986bcb6294e2a6da8240e1f1930778fabbeff4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366578"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="d61df-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="d61df-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="d61df-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d61df-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d61df-105">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="d61df-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="d61df-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d61df-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d61df-107">属性</span><span class="sxs-lookup"><span data-stu-id="d61df-107">Properties</span></span>
|<span data-ttu-id="d61df-108">属性</span><span class="sxs-lookup"><span data-stu-id="d61df-108">Property</span></span>|<span data-ttu-id="d61df-109">类型</span><span class="sxs-lookup"><span data-stu-id="d61df-109">Type</span></span>|<span data-ttu-id="d61df-110">说明</span><span class="sxs-lookup"><span data-stu-id="d61df-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d61df-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d61df-111">displayName</span></span>|<span data-ttu-id="d61df-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d61df-112">String</span></span>|<span data-ttu-id="d61df-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="d61df-113">Display Name.</span></span> <span data-ttu-id="d61df-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d61df-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d61df-115">说明</span><span class="sxs-lookup"><span data-stu-id="d61df-115">description</span></span>|<span data-ttu-id="d61df-116">String</span><span class="sxs-lookup"><span data-stu-id="d61df-116">String</span></span>|<span data-ttu-id="d61df-117">说明。</span><span class="sxs-lookup"><span data-stu-id="d61df-117">Description.</span></span> <span data-ttu-id="d61df-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d61df-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d61df-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d61df-119">omaUri</span></span>|<span data-ttu-id="d61df-120">String</span><span class="sxs-lookup"><span data-stu-id="d61df-120">String</span></span>|<span data-ttu-id="d61df-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="d61df-121">OMA.</span></span> <span data-ttu-id="d61df-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d61df-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d61df-123">fileName</span><span class="sxs-lookup"><span data-stu-id="d61df-123">fileName</span></span>|<span data-ttu-id="d61df-124">String</span><span class="sxs-lookup"><span data-stu-id="d61df-124">String</span></span>|<span data-ttu-id="d61df-125">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="d61df-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="d61df-126">\* .crt</span><span class="sxs-lookup"><span data-stu-id="d61df-126">\*.crt</span></span> | <span data-ttu-id="d61df-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="d61df-127">\*.p7b</span></span> | <span data-ttu-id="d61df-128">\* bin）。</span><span class="sxs-lookup"><span data-stu-id="d61df-128">\*.bin).</span></span>|
|<span data-ttu-id="d61df-129">value</span><span class="sxs-lookup"><span data-stu-id="d61df-129">value</span></span>|<span data-ttu-id="d61df-130">String</span><span class="sxs-lookup"><span data-stu-id="d61df-130">String</span></span>|<span data-ttu-id="d61df-131">值。</span><span class="sxs-lookup"><span data-stu-id="d61df-131">Value.</span></span> <span data-ttu-id="d61df-132">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="d61df-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d61df-133">关系</span><span class="sxs-lookup"><span data-stu-id="d61df-133">Relationships</span></span>
<span data-ttu-id="d61df-134">无</span><span class="sxs-lookup"><span data-stu-id="d61df-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d61df-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d61df-135">JSON Representation</span></span>
<span data-ttu-id="d61df-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d61df-136">Here is a JSON representation of the resource.</span></span>
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




