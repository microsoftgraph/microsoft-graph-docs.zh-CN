---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 43c3c73d01eb5e2e44c5f5a0a9e85c2e6577262e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273121"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="81178-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="81178-103">omaSettingFloatingPoint resource type</span></span>

<span data-ttu-id="81178-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81178-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81178-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81178-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81178-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81178-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81178-107">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="81178-107">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="81178-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81178-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81178-109">属性</span><span class="sxs-lookup"><span data-stu-id="81178-109">Properties</span></span>
|<span data-ttu-id="81178-110">属性</span><span class="sxs-lookup"><span data-stu-id="81178-110">Property</span></span>|<span data-ttu-id="81178-111">类型</span><span class="sxs-lookup"><span data-stu-id="81178-111">Type</span></span>|<span data-ttu-id="81178-112">说明</span><span class="sxs-lookup"><span data-stu-id="81178-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81178-113">displayName</span><span class="sxs-lookup"><span data-stu-id="81178-113">displayName</span></span>|<span data-ttu-id="81178-114">字符串</span><span class="sxs-lookup"><span data-stu-id="81178-114">String</span></span>|<span data-ttu-id="81178-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="81178-115">Display Name.</span></span> <span data-ttu-id="81178-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81178-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81178-117">description</span><span class="sxs-lookup"><span data-stu-id="81178-117">description</span></span>|<span data-ttu-id="81178-118">字符串</span><span class="sxs-lookup"><span data-stu-id="81178-118">String</span></span>|<span data-ttu-id="81178-119">说明。</span><span class="sxs-lookup"><span data-stu-id="81178-119">Description.</span></span> <span data-ttu-id="81178-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81178-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81178-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="81178-121">omaUri</span></span>|<span data-ttu-id="81178-122">String</span><span class="sxs-lookup"><span data-stu-id="81178-122">String</span></span>|<span data-ttu-id="81178-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="81178-123">OMA.</span></span> <span data-ttu-id="81178-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81178-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81178-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="81178-125">isEncrypted</span></span>|<span data-ttu-id="81178-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="81178-126">Boolean</span></span>|<span data-ttu-id="81178-127">指示是否对值字段进行加密。</span><span class="sxs-lookup"><span data-stu-id="81178-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="81178-128">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="81178-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="81178-129">value</span><span class="sxs-lookup"><span data-stu-id="81178-129">value</span></span>|<span data-ttu-id="81178-130">单个</span><span class="sxs-lookup"><span data-stu-id="81178-130">Single</span></span>|<span data-ttu-id="81178-131">值。</span><span class="sxs-lookup"><span data-stu-id="81178-131">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81178-132">关系</span><span class="sxs-lookup"><span data-stu-id="81178-132">Relationships</span></span>
<span data-ttu-id="81178-133">无</span><span class="sxs-lookup"><span data-stu-id="81178-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81178-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81178-134">JSON Representation</span></span>
<span data-ttu-id="81178-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81178-135">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "value": 4.2
}
```




