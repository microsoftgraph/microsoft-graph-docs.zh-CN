---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 72c7bdd9eda67d9bdebc2452ad778d4ad653d7df
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079275"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="c9138-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9138-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="c9138-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9138-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c9138-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9138-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9138-106">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="c9138-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="c9138-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9138-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9138-108">属性</span><span class="sxs-lookup"><span data-stu-id="c9138-108">Properties</span></span>
|<span data-ttu-id="c9138-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9138-109">Property</span></span>|<span data-ttu-id="c9138-110">类型</span><span class="sxs-lookup"><span data-stu-id="c9138-110">Type</span></span>|<span data-ttu-id="c9138-111">说明</span><span class="sxs-lookup"><span data-stu-id="c9138-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9138-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c9138-112">displayName</span></span>|<span data-ttu-id="c9138-113">String</span><span class="sxs-lookup"><span data-stu-id="c9138-113">String</span></span>|<span data-ttu-id="c9138-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c9138-114">Display Name.</span></span> <span data-ttu-id="c9138-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9138-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9138-116">description</span><span class="sxs-lookup"><span data-stu-id="c9138-116">description</span></span>|<span data-ttu-id="c9138-117">String</span><span class="sxs-lookup"><span data-stu-id="c9138-117">String</span></span>|<span data-ttu-id="c9138-118">说明。</span><span class="sxs-lookup"><span data-stu-id="c9138-118">Description.</span></span> <span data-ttu-id="c9138-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9138-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9138-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="c9138-120">omaUri</span></span>|<span data-ttu-id="c9138-121">String</span><span class="sxs-lookup"><span data-stu-id="c9138-121">String</span></span>|<span data-ttu-id="c9138-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="c9138-122">OMA.</span></span> <span data-ttu-id="c9138-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c9138-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9138-124">fileName</span><span class="sxs-lookup"><span data-stu-id="c9138-124">fileName</span></span>|<span data-ttu-id="c9138-125">String</span><span class="sxs-lookup"><span data-stu-id="c9138-125">String</span></span>|<span data-ttu-id="c9138-126">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="c9138-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="c9138-127">\* .crt</span><span class="sxs-lookup"><span data-stu-id="c9138-127">\*.crt</span></span> | <span data-ttu-id="c9138-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="c9138-128">\*.p7b</span></span> | <span data-ttu-id="c9138-129">\* bin) 。</span><span class="sxs-lookup"><span data-stu-id="c9138-129">\*.bin).</span></span>|
|<span data-ttu-id="c9138-130">value</span><span class="sxs-lookup"><span data-stu-id="c9138-130">value</span></span>|<span data-ttu-id="c9138-131">String</span><span class="sxs-lookup"><span data-stu-id="c9138-131">String</span></span>|<span data-ttu-id="c9138-132">值。</span><span class="sxs-lookup"><span data-stu-id="c9138-132">Value.</span></span> <span data-ttu-id="c9138-133">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="c9138-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9138-134">关系</span><span class="sxs-lookup"><span data-stu-id="c9138-134">Relationships</span></span>
<span data-ttu-id="c9138-135">无</span><span class="sxs-lookup"><span data-stu-id="c9138-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9138-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9138-136">JSON Representation</span></span>
<span data-ttu-id="c9138-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9138-137">Here is a JSON representation of the resource.</span></span>
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









