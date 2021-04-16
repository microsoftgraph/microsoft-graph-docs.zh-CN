---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8729dd6251f9dbaf062fbfee3d024de265565020
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867453"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="b5970-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5970-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="b5970-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5970-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5970-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5970-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5970-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5970-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5970-107">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="b5970-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="b5970-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b5970-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5970-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5970-109">Properties</span></span>
|<span data-ttu-id="b5970-110">属性</span><span class="sxs-lookup"><span data-stu-id="b5970-110">Property</span></span>|<span data-ttu-id="b5970-111">类型</span><span class="sxs-lookup"><span data-stu-id="b5970-111">Type</span></span>|<span data-ttu-id="b5970-112">说明</span><span class="sxs-lookup"><span data-stu-id="b5970-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5970-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b5970-113">displayName</span></span>|<span data-ttu-id="b5970-114">String</span><span class="sxs-lookup"><span data-stu-id="b5970-114">String</span></span>|<span data-ttu-id="b5970-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b5970-115">Display Name.</span></span> <span data-ttu-id="b5970-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b5970-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b5970-117">说明</span><span class="sxs-lookup"><span data-stu-id="b5970-117">description</span></span>|<span data-ttu-id="b5970-118">String</span><span class="sxs-lookup"><span data-stu-id="b5970-118">String</span></span>|<span data-ttu-id="b5970-119">说明。</span><span class="sxs-lookup"><span data-stu-id="b5970-119">Description.</span></span> <span data-ttu-id="b5970-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b5970-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b5970-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b5970-121">omaUri</span></span>|<span data-ttu-id="b5970-122">String</span><span class="sxs-lookup"><span data-stu-id="b5970-122">String</span></span>|<span data-ttu-id="b5970-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="b5970-123">OMA.</span></span> <span data-ttu-id="b5970-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b5970-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b5970-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="b5970-125">secretReferenceValueId</span></span>|<span data-ttu-id="b5970-126">String</span><span class="sxs-lookup"><span data-stu-id="b5970-126">String</span></span>|<span data-ttu-id="b5970-127">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="b5970-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="b5970-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b5970-128">This property is read-only.</span></span> <span data-ttu-id="b5970-129">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b5970-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b5970-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="b5970-130">isEncrypted</span></span>|<span data-ttu-id="b5970-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5970-131">Boolean</span></span>|<span data-ttu-id="b5970-132">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="b5970-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="b5970-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b5970-133">This property is read-only.</span></span> <span data-ttu-id="b5970-134">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b5970-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b5970-135">fileName</span><span class="sxs-lookup"><span data-stu-id="b5970-135">fileName</span></span>|<span data-ttu-id="b5970-136">String</span><span class="sxs-lookup"><span data-stu-id="b5970-136">String</span></span>|<span data-ttu-id="b5970-137">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="b5970-137">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="b5970-138">\*.crt</span><span class="sxs-lookup"><span data-stu-id="b5970-138">\*.crt</span></span> | <span data-ttu-id="b5970-139">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="b5970-139">\*.p7b</span></span> | <span data-ttu-id="b5970-140">\*.bin) 。</span><span class="sxs-lookup"><span data-stu-id="b5970-140">\*.bin).</span></span>|
|<span data-ttu-id="b5970-141">value</span><span class="sxs-lookup"><span data-stu-id="b5970-141">value</span></span>|<span data-ttu-id="b5970-142">String</span><span class="sxs-lookup"><span data-stu-id="b5970-142">String</span></span>|<span data-ttu-id="b5970-143">值。</span><span class="sxs-lookup"><span data-stu-id="b5970-143">Value.</span></span> <span data-ttu-id="b5970-144">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="b5970-144">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5970-145">关系</span><span class="sxs-lookup"><span data-stu-id="b5970-145">Relationships</span></span>
<span data-ttu-id="b5970-146">无</span><span class="sxs-lookup"><span data-stu-id="b5970-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5970-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5970-147">JSON Representation</span></span>
<span data-ttu-id="b5970-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5970-148">Here is a JSON representation of the resource.</span></span>
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
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "fileName": "String",
  "value": "String"
}
```




