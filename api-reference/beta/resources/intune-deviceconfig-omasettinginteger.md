---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19db5504d276c748d720803ba201c555752e2f33
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867390"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="68e8b-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="68e8b-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="68e8b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68e8b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68e8b-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68e8b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68e8b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68e8b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68e8b-107">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="68e8b-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="68e8b-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="68e8b-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68e8b-109">属性</span><span class="sxs-lookup"><span data-stu-id="68e8b-109">Properties</span></span>
|<span data-ttu-id="68e8b-110">属性</span><span class="sxs-lookup"><span data-stu-id="68e8b-110">Property</span></span>|<span data-ttu-id="68e8b-111">类型</span><span class="sxs-lookup"><span data-stu-id="68e8b-111">Type</span></span>|<span data-ttu-id="68e8b-112">说明</span><span class="sxs-lookup"><span data-stu-id="68e8b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68e8b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="68e8b-113">displayName</span></span>|<span data-ttu-id="68e8b-114">String</span><span class="sxs-lookup"><span data-stu-id="68e8b-114">String</span></span>|<span data-ttu-id="68e8b-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="68e8b-115">Display Name.</span></span> <span data-ttu-id="68e8b-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="68e8b-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68e8b-117">说明</span><span class="sxs-lookup"><span data-stu-id="68e8b-117">description</span></span>|<span data-ttu-id="68e8b-118">String</span><span class="sxs-lookup"><span data-stu-id="68e8b-118">String</span></span>|<span data-ttu-id="68e8b-119">说明。</span><span class="sxs-lookup"><span data-stu-id="68e8b-119">Description.</span></span> <span data-ttu-id="68e8b-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="68e8b-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68e8b-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="68e8b-121">omaUri</span></span>|<span data-ttu-id="68e8b-122">String</span><span class="sxs-lookup"><span data-stu-id="68e8b-122">String</span></span>|<span data-ttu-id="68e8b-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="68e8b-123">OMA.</span></span> <span data-ttu-id="68e8b-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="68e8b-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68e8b-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="68e8b-125">secretReferenceValueId</span></span>|<span data-ttu-id="68e8b-126">String</span><span class="sxs-lookup"><span data-stu-id="68e8b-126">String</span></span>|<span data-ttu-id="68e8b-127">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="68e8b-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="68e8b-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="68e8b-128">This property is read-only.</span></span> <span data-ttu-id="68e8b-129">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="68e8b-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68e8b-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="68e8b-130">isEncrypted</span></span>|<span data-ttu-id="68e8b-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="68e8b-131">Boolean</span></span>|<span data-ttu-id="68e8b-132">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="68e8b-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="68e8b-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="68e8b-133">This property is read-only.</span></span> <span data-ttu-id="68e8b-134">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="68e8b-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68e8b-135">值</span><span class="sxs-lookup"><span data-stu-id="68e8b-135">value</span></span>|<span data-ttu-id="68e8b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="68e8b-136">Int32</span></span>|<span data-ttu-id="68e8b-137">值。</span><span class="sxs-lookup"><span data-stu-id="68e8b-137">Value.</span></span>|
|<span data-ttu-id="68e8b-138">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="68e8b-138">isReadOnly</span></span>|<span data-ttu-id="68e8b-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="68e8b-139">Boolean</span></span>|<span data-ttu-id="68e8b-140">通过设置为 true，CSP (OMA-URI) 的云解决方案提供商将执行获取，而不是设置</span><span class="sxs-lookup"><span data-stu-id="68e8b-140">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="68e8b-141">关系</span><span class="sxs-lookup"><span data-stu-id="68e8b-141">Relationships</span></span>
<span data-ttu-id="68e8b-142">无</span><span class="sxs-lookup"><span data-stu-id="68e8b-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68e8b-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68e8b-143">JSON Representation</span></span>
<span data-ttu-id="68e8b-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68e8b-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": 1024,
  "isReadOnly": true
}
```




