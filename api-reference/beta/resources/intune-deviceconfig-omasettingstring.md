---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f1f17f03a553b5040eab7ac482ad4b13d54bbf69
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279666"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="f3179-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3179-103">omaSettingString resource type</span></span>

<span data-ttu-id="f3179-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3179-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3179-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3179-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3179-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3179-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3179-107">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="f3179-107">OMA Settings String definition.</span></span>


<span data-ttu-id="f3179-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3179-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3179-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3179-109">Properties</span></span>
|<span data-ttu-id="f3179-110">属性</span><span class="sxs-lookup"><span data-stu-id="f3179-110">Property</span></span>|<span data-ttu-id="f3179-111">类型</span><span class="sxs-lookup"><span data-stu-id="f3179-111">Type</span></span>|<span data-ttu-id="f3179-112">说明</span><span class="sxs-lookup"><span data-stu-id="f3179-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3179-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f3179-113">displayName</span></span>|<span data-ttu-id="f3179-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f3179-114">String</span></span>|<span data-ttu-id="f3179-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f3179-115">Display Name.</span></span> <span data-ttu-id="f3179-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3179-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3179-117">description</span><span class="sxs-lookup"><span data-stu-id="f3179-117">description</span></span>|<span data-ttu-id="f3179-118">字符串</span><span class="sxs-lookup"><span data-stu-id="f3179-118">String</span></span>|<span data-ttu-id="f3179-119">说明。</span><span class="sxs-lookup"><span data-stu-id="f3179-119">Description.</span></span> <span data-ttu-id="f3179-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3179-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3179-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="f3179-121">omaUri</span></span>|<span data-ttu-id="f3179-122">String</span><span class="sxs-lookup"><span data-stu-id="f3179-122">String</span></span>|<span data-ttu-id="f3179-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="f3179-123">OMA.</span></span> <span data-ttu-id="f3179-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3179-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3179-125">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="f3179-125">isEncrypted</span></span>|<span data-ttu-id="f3179-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3179-126">Boolean</span></span>|<span data-ttu-id="f3179-127">指示是否对值字段进行加密。</span><span class="sxs-lookup"><span data-stu-id="f3179-127">Indicates whether the value field is encrypted.</span></span> <span data-ttu-id="f3179-128">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3179-128">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3179-129">value</span><span class="sxs-lookup"><span data-stu-id="f3179-129">value</span></span>|<span data-ttu-id="f3179-130">String</span><span class="sxs-lookup"><span data-stu-id="f3179-130">String</span></span>|<span data-ttu-id="f3179-131">值。</span><span class="sxs-lookup"><span data-stu-id="f3179-131">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3179-132">关系</span><span class="sxs-lookup"><span data-stu-id="f3179-132">Relationships</span></span>
<span data-ttu-id="f3179-133">无</span><span class="sxs-lookup"><span data-stu-id="f3179-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3179-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3179-134">JSON Representation</span></span>
<span data-ttu-id="f3179-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3179-135">Here is a JSON representation of the resource.</span></span>
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
  "isEncrypted": true,
  "value": "String"
}
```




