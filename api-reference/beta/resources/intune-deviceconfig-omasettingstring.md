---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b20f71bb7d5e188303c742efce96b23f89f698c0
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867376"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="42bcb-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="42bcb-103">omaSettingString resource type</span></span>

<span data-ttu-id="42bcb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42bcb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42bcb-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42bcb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42bcb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42bcb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42bcb-107">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="42bcb-107">OMA Settings String definition.</span></span>


<span data-ttu-id="42bcb-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42bcb-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42bcb-109">属性</span><span class="sxs-lookup"><span data-stu-id="42bcb-109">Properties</span></span>
|<span data-ttu-id="42bcb-110">属性</span><span class="sxs-lookup"><span data-stu-id="42bcb-110">Property</span></span>|<span data-ttu-id="42bcb-111">类型</span><span class="sxs-lookup"><span data-stu-id="42bcb-111">Type</span></span>|<span data-ttu-id="42bcb-112">说明</span><span class="sxs-lookup"><span data-stu-id="42bcb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42bcb-113">displayName</span><span class="sxs-lookup"><span data-stu-id="42bcb-113">displayName</span></span>|<span data-ttu-id="42bcb-114">String</span><span class="sxs-lookup"><span data-stu-id="42bcb-114">String</span></span>|<span data-ttu-id="42bcb-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="42bcb-115">Display Name.</span></span> <span data-ttu-id="42bcb-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42bcb-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42bcb-117">说明</span><span class="sxs-lookup"><span data-stu-id="42bcb-117">description</span></span>|<span data-ttu-id="42bcb-118">String</span><span class="sxs-lookup"><span data-stu-id="42bcb-118">String</span></span>|<span data-ttu-id="42bcb-119">说明。</span><span class="sxs-lookup"><span data-stu-id="42bcb-119">Description.</span></span> <span data-ttu-id="42bcb-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42bcb-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42bcb-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="42bcb-121">omaUri</span></span>|<span data-ttu-id="42bcb-122">String</span><span class="sxs-lookup"><span data-stu-id="42bcb-122">String</span></span>|<span data-ttu-id="42bcb-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="42bcb-123">OMA.</span></span> <span data-ttu-id="42bcb-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42bcb-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42bcb-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="42bcb-125">secretReferenceValueId</span></span>|<span data-ttu-id="42bcb-126">String</span><span class="sxs-lookup"><span data-stu-id="42bcb-126">String</span></span>|<span data-ttu-id="42bcb-127">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="42bcb-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="42bcb-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="42bcb-128">This property is read-only.</span></span> <span data-ttu-id="42bcb-129">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42bcb-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42bcb-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="42bcb-130">isEncrypted</span></span>|<span data-ttu-id="42bcb-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="42bcb-131">Boolean</span></span>|<span data-ttu-id="42bcb-132">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="42bcb-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="42bcb-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="42bcb-133">This property is read-only.</span></span> <span data-ttu-id="42bcb-134">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="42bcb-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="42bcb-135">value</span><span class="sxs-lookup"><span data-stu-id="42bcb-135">value</span></span>|<span data-ttu-id="42bcb-136">String</span><span class="sxs-lookup"><span data-stu-id="42bcb-136">String</span></span>|<span data-ttu-id="42bcb-137">值。</span><span class="sxs-lookup"><span data-stu-id="42bcb-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42bcb-138">关系</span><span class="sxs-lookup"><span data-stu-id="42bcb-138">Relationships</span></span>
<span data-ttu-id="42bcb-139">无</span><span class="sxs-lookup"><span data-stu-id="42bcb-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42bcb-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42bcb-140">JSON Representation</span></span>
<span data-ttu-id="42bcb-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42bcb-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": "String"
}
```




