---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e335f0e99b342df6c596900aab8f1a1933703b9f
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867418"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="11b34-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="11b34-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="11b34-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11b34-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11b34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11b34-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11b34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b34-107">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="11b34-107">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="11b34-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="11b34-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="11b34-109">属性</span><span class="sxs-lookup"><span data-stu-id="11b34-109">Properties</span></span>
|<span data-ttu-id="11b34-110">属性</span><span class="sxs-lookup"><span data-stu-id="11b34-110">Property</span></span>|<span data-ttu-id="11b34-111">类型</span><span class="sxs-lookup"><span data-stu-id="11b34-111">Type</span></span>|<span data-ttu-id="11b34-112">说明</span><span class="sxs-lookup"><span data-stu-id="11b34-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11b34-113">displayName</span><span class="sxs-lookup"><span data-stu-id="11b34-113">displayName</span></span>|<span data-ttu-id="11b34-114">String</span><span class="sxs-lookup"><span data-stu-id="11b34-114">String</span></span>|<span data-ttu-id="11b34-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="11b34-115">Display Name.</span></span> <span data-ttu-id="11b34-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="11b34-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="11b34-117">说明</span><span class="sxs-lookup"><span data-stu-id="11b34-117">description</span></span>|<span data-ttu-id="11b34-118">String</span><span class="sxs-lookup"><span data-stu-id="11b34-118">String</span></span>|<span data-ttu-id="11b34-119">说明。</span><span class="sxs-lookup"><span data-stu-id="11b34-119">Description.</span></span> <span data-ttu-id="11b34-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="11b34-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="11b34-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="11b34-121">omaUri</span></span>|<span data-ttu-id="11b34-122">String</span><span class="sxs-lookup"><span data-stu-id="11b34-122">String</span></span>|<span data-ttu-id="11b34-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="11b34-123">OMA.</span></span> <span data-ttu-id="11b34-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="11b34-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="11b34-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="11b34-125">secretReferenceValueId</span></span>|<span data-ttu-id="11b34-126">String</span><span class="sxs-lookup"><span data-stu-id="11b34-126">String</span></span>|<span data-ttu-id="11b34-127">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="11b34-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="11b34-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="11b34-128">This property is read-only.</span></span> <span data-ttu-id="11b34-129">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="11b34-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="11b34-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="11b34-130">isEncrypted</span></span>|<span data-ttu-id="11b34-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="11b34-131">Boolean</span></span>|<span data-ttu-id="11b34-132">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="11b34-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="11b34-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="11b34-133">This property is read-only.</span></span> <span data-ttu-id="11b34-134">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="11b34-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="11b34-135">value</span><span class="sxs-lookup"><span data-stu-id="11b34-135">value</span></span>|<span data-ttu-id="11b34-136">单个</span><span class="sxs-lookup"><span data-stu-id="11b34-136">Single</span></span>|<span data-ttu-id="11b34-137">值。</span><span class="sxs-lookup"><span data-stu-id="11b34-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11b34-138">关系</span><span class="sxs-lookup"><span data-stu-id="11b34-138">Relationships</span></span>
<span data-ttu-id="11b34-139">无</span><span class="sxs-lookup"><span data-stu-id="11b34-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11b34-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11b34-140">JSON Representation</span></span>
<span data-ttu-id="11b34-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11b34-141">Here is a JSON representation of the resource.</span></span>
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
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": 4.2
}
```




