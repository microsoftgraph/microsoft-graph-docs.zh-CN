---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c618673c59ca2a085663b8b33b5585045fbc001d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273177"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="62246-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="62246-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="62246-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62246-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62246-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62246-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62246-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62246-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62246-107">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="62246-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="62246-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="62246-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="62246-109">属性</span><span class="sxs-lookup"><span data-stu-id="62246-109">Properties</span></span>
|<span data-ttu-id="62246-110">属性</span><span class="sxs-lookup"><span data-stu-id="62246-110">Property</span></span>|<span data-ttu-id="62246-111">类型</span><span class="sxs-lookup"><span data-stu-id="62246-111">Type</span></span>|<span data-ttu-id="62246-112">说明</span><span class="sxs-lookup"><span data-stu-id="62246-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62246-113">displayName</span><span class="sxs-lookup"><span data-stu-id="62246-113">displayName</span></span>|<span data-ttu-id="62246-114">字符串</span><span class="sxs-lookup"><span data-stu-id="62246-114">String</span></span>|<span data-ttu-id="62246-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="62246-115">Display Name.</span></span> <span data-ttu-id="62246-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="62246-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="62246-117">description</span><span class="sxs-lookup"><span data-stu-id="62246-117">description</span></span>|<span data-ttu-id="62246-118">字符串</span><span class="sxs-lookup"><span data-stu-id="62246-118">String</span></span>|<span data-ttu-id="62246-119">说明。</span><span class="sxs-lookup"><span data-stu-id="62246-119">Description.</span></span> <span data-ttu-id="62246-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="62246-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="62246-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="62246-121">omaUri</span></span>|<span data-ttu-id="62246-122">String</span><span class="sxs-lookup"><span data-stu-id="62246-122">String</span></span>|<span data-ttu-id="62246-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="62246-123">OMA.</span></span> <span data-ttu-id="62246-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="62246-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="62246-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="62246-125">isEncrypted</span></span>|<span data-ttu-id="62246-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="62246-126">Boolean</span></span>|<span data-ttu-id="62246-127">指示是否对值字段进行加密。</span><span class="sxs-lookup"><span data-stu-id="62246-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="62246-128">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="62246-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="62246-129">fileName</span><span class="sxs-lookup"><span data-stu-id="62246-129">fileName</span></span>|<span data-ttu-id="62246-130">String</span><span class="sxs-lookup"><span data-stu-id="62246-130">String</span></span>|<span data-ttu-id="62246-131">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="62246-131">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="62246-132">\* .crt</span><span class="sxs-lookup"><span data-stu-id="62246-132">\*.crt</span></span> | <span data-ttu-id="62246-133">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="62246-133">\*.p7b</span></span> | <span data-ttu-id="62246-134">\* bin) 。</span><span class="sxs-lookup"><span data-stu-id="62246-134">\*.bin).</span></span>|
|<span data-ttu-id="62246-135">value</span><span class="sxs-lookup"><span data-stu-id="62246-135">value</span></span>|<span data-ttu-id="62246-136">String</span><span class="sxs-lookup"><span data-stu-id="62246-136">String</span></span>|<span data-ttu-id="62246-137">值。</span><span class="sxs-lookup"><span data-stu-id="62246-137">Value.</span></span> <span data-ttu-id="62246-138">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="62246-138">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="62246-139">关系</span><span class="sxs-lookup"><span data-stu-id="62246-139">Relationships</span></span>
<span data-ttu-id="62246-140">无</span><span class="sxs-lookup"><span data-stu-id="62246-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62246-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62246-141">JSON Representation</span></span>
<span data-ttu-id="62246-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62246-142">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```




