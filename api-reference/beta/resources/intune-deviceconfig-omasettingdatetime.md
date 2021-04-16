---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30ed623b5fc59b9a96c0e37e8b2b1fcfc77e7b13
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867425"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="b1fc1-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1fc1-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="b1fc1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1fc1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1fc1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1fc1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1fc1-107">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-107">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="b1fc1-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc1-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b1fc1-109">属性</span><span class="sxs-lookup"><span data-stu-id="b1fc1-109">Properties</span></span>
|<span data-ttu-id="b1fc1-110">属性</span><span class="sxs-lookup"><span data-stu-id="b1fc1-110">Property</span></span>|<span data-ttu-id="b1fc1-111">类型</span><span class="sxs-lookup"><span data-stu-id="b1fc1-111">Type</span></span>|<span data-ttu-id="b1fc1-112">说明</span><span class="sxs-lookup"><span data-stu-id="b1fc1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1fc1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b1fc1-113">displayName</span></span>|<span data-ttu-id="b1fc1-114">String</span><span class="sxs-lookup"><span data-stu-id="b1fc1-114">String</span></span>|<span data-ttu-id="b1fc1-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-115">Display Name.</span></span> <span data-ttu-id="b1fc1-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc1-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1fc1-117">说明</span><span class="sxs-lookup"><span data-stu-id="b1fc1-117">description</span></span>|<span data-ttu-id="b1fc1-118">String</span><span class="sxs-lookup"><span data-stu-id="b1fc1-118">String</span></span>|<span data-ttu-id="b1fc1-119">说明。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-119">Description.</span></span> <span data-ttu-id="b1fc1-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc1-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1fc1-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="b1fc1-121">omaUri</span></span>|<span data-ttu-id="b1fc1-122">String</span><span class="sxs-lookup"><span data-stu-id="b1fc1-122">String</span></span>|<span data-ttu-id="b1fc1-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-123">OMA.</span></span> <span data-ttu-id="b1fc1-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc1-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1fc1-125">secretReferenceValueId</span><span class="sxs-lookup"><span data-stu-id="b1fc1-125">secretReferenceValueId</span></span>|<span data-ttu-id="b1fc1-126">String</span><span class="sxs-lookup"><span data-stu-id="b1fc1-126">String</span></span>|<span data-ttu-id="b1fc1-127">用于查找解密密码的 ReferenceId。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-127">ReferenceId for looking up secret for decryption.</span></span> <span data-ttu-id="b1fc1-128">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-128">This property is read-only.</span></span> <span data-ttu-id="b1fc1-129">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc1-129">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1fc1-130">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="b1fc1-130">isEncrypted</span></span>|<span data-ttu-id="b1fc1-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1fc1-131">Boolean</span></span>|<span data-ttu-id="b1fc1-132">指示值字段是否加密。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-132">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="b1fc1-133">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-133">This property is read-only.</span></span> <span data-ttu-id="b1fc1-134">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b1fc1-134">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b1fc1-135">value</span><span class="sxs-lookup"><span data-stu-id="b1fc1-135">value</span></span>|<span data-ttu-id="b1fc1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1fc1-136">DateTimeOffset</span></span>|<span data-ttu-id="b1fc1-137">值。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-137">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1fc1-138">关系</span><span class="sxs-lookup"><span data-stu-id="b1fc1-138">Relationships</span></span>
<span data-ttu-id="b1fc1-139">无</span><span class="sxs-lookup"><span data-stu-id="b1fc1-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1fc1-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1fc1-140">JSON Representation</span></span>
<span data-ttu-id="b1fc1-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1fc1-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "secretReferenceValueId": "String",
  "isEncrypted": true,
  "value": "String (timestamp)"
}
```




