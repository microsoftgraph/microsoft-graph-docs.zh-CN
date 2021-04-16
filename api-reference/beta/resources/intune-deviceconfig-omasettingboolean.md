---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e1118001a06ff19439d5d0b1a3970b358235f4d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867439"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="ceff5-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="ceff5-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="ceff5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ceff5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ceff5-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ceff5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ceff5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ceff5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ceff5-107">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="ceff5-107">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="ceff5-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ceff5-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ceff5-109">属性</span><span class="sxs-lookup"><span data-stu-id="ceff5-109">Properties</span></span>
|<span data-ttu-id="ceff5-110">属性</span><span class="sxs-lookup"><span data-stu-id="ceff5-110">Property</span></span>|<span data-ttu-id="ceff5-111">类型</span><span class="sxs-lookup"><span data-stu-id="ceff5-111">Type</span></span>|<span data-ttu-id="ceff5-112">说明</span><span class="sxs-lookup"><span data-stu-id="ceff5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ceff5-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ceff5-113">displayName</span></span>|<span data-ttu-id="ceff5-114">String</span><span class="sxs-lookup"><span data-stu-id="ceff5-114">String</span></span>|<span data-ttu-id="ceff5-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ceff5-115">Display Name.</span></span> <span data-ttu-id="ceff5-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ceff5-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ceff5-117">说明</span><span class="sxs-lookup"><span data-stu-id="ceff5-117">description</span></span>|<span data-ttu-id="ceff5-118">String</span><span class="sxs-lookup"><span data-stu-id="ceff5-118">String</span></span>|<span data-ttu-id="ceff5-119">说明。</span><span class="sxs-lookup"><span data-stu-id="ceff5-119">Description.</span></span> <span data-ttu-id="ceff5-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ceff5-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ceff5-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="ceff5-121">omaUri</span></span>|<span data-ttu-id="ceff5-122">String</span><span class="sxs-lookup"><span data-stu-id="ceff5-122">String</span></span>|<span data-ttu-id="ceff5-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="ceff5-123">OMA.</span></span> <span data-ttu-id="ceff5-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ceff5-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ceff5-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="ceff5-125">secretReferenceValueId</span></span>|<span data-ttu-id="ceff5-126">String</span><span class="sxs-lookup"><span data-stu-id="ceff5-126">String</span></span>|<span data-ttu-id="ceff5-127">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="ceff5-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="ceff5-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ceff5-128">This property is read-only.</span></span> <span data-ttu-id="ceff5-129">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ceff5-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ceff5-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ceff5-130">isEncrypted</span></span>|<span data-ttu-id="ceff5-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ceff5-131">Boolean</span></span>|<span data-ttu-id="ceff5-132">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="ceff5-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="ceff5-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ceff5-133">This property is read-only.</span></span> <span data-ttu-id="ceff5-134">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ceff5-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ceff5-135">value</span><span class="sxs-lookup"><span data-stu-id="ceff5-135">value</span></span>|<span data-ttu-id="ceff5-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="ceff5-136">Boolean</span></span>|<span data-ttu-id="ceff5-137">值。</span><span class="sxs-lookup"><span data-stu-id="ceff5-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ceff5-138">关系</span><span class="sxs-lookup"><span data-stu-id="ceff5-138">Relationships</span></span>
<span data-ttu-id="ceff5-139">无</span><span class="sxs-lookup"><span data-stu-id="ceff5-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ceff5-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ceff5-140">JSON Representation</span></span>
<span data-ttu-id="ceff5-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ceff5-141">Here is a JSON representation of the resource.</span></span>
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
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": true
}
```




