---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67fcf5574b3cb4481286ecc7b4448018d64e0f44
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472025"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="dca56-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="dca56-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="dca56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dca56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dca56-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dca56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dca56-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dca56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dca56-107">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="dca56-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="dca56-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca56-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dca56-109">属性</span><span class="sxs-lookup"><span data-stu-id="dca56-109">Properties</span></span>
|<span data-ttu-id="dca56-110">属性</span><span class="sxs-lookup"><span data-stu-id="dca56-110">Property</span></span>|<span data-ttu-id="dca56-111">类型</span><span class="sxs-lookup"><span data-stu-id="dca56-111">Type</span></span>|<span data-ttu-id="dca56-112">说明</span><span class="sxs-lookup"><span data-stu-id="dca56-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dca56-113">displayName</span><span class="sxs-lookup"><span data-stu-id="dca56-113">displayName</span></span>|<span data-ttu-id="dca56-114">String</span><span class="sxs-lookup"><span data-stu-id="dca56-114">String</span></span>|<span data-ttu-id="dca56-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="dca56-115">Display Name.</span></span> <span data-ttu-id="dca56-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca56-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="dca56-117">description</span><span class="sxs-lookup"><span data-stu-id="dca56-117">description</span></span>|<span data-ttu-id="dca56-118">String</span><span class="sxs-lookup"><span data-stu-id="dca56-118">String</span></span>|<span data-ttu-id="dca56-119">说明。</span><span class="sxs-lookup"><span data-stu-id="dca56-119">Description.</span></span> <span data-ttu-id="dca56-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca56-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="dca56-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="dca56-121">omaUri</span></span>|<span data-ttu-id="dca56-122">String</span><span class="sxs-lookup"><span data-stu-id="dca56-122">String</span></span>|<span data-ttu-id="dca56-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="dca56-123">OMA.</span></span> <span data-ttu-id="dca56-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca56-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="dca56-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="dca56-125">isEncrypted</span></span>|<span data-ttu-id="dca56-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="dca56-126">Boolean</span></span>|<span data-ttu-id="dca56-127">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="dca56-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="dca56-128">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="dca56-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="dca56-129">fileName</span><span class="sxs-lookup"><span data-stu-id="dca56-129">fileName</span></span>|<span data-ttu-id="dca56-130">String</span><span class="sxs-lookup"><span data-stu-id="dca56-130">String</span></span>|<span data-ttu-id="dca56-131">与 Value 属性 (\*.cer \| \*.crt \| \*.p7b \| \*.bin) 。</span><span class="sxs-lookup"><span data-stu-id="dca56-131">File name associated with the Value property (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span></span>|
|<span data-ttu-id="dca56-132">value</span><span class="sxs-lookup"><span data-stu-id="dca56-132">value</span></span>|<span data-ttu-id="dca56-133">String</span><span class="sxs-lookup"><span data-stu-id="dca56-133">String</span></span>|<span data-ttu-id="dca56-134">值。</span><span class="sxs-lookup"><span data-stu-id="dca56-134">Value.</span></span> <span data-ttu-id="dca56-135">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="dca56-135">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="dca56-136">关系</span><span class="sxs-lookup"><span data-stu-id="dca56-136">Relationships</span></span>
<span data-ttu-id="dca56-137">无</span><span class="sxs-lookup"><span data-stu-id="dca56-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dca56-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dca56-138">JSON Representation</span></span>
<span data-ttu-id="dca56-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dca56-139">Here is a JSON representation of the resource.</span></span>
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




