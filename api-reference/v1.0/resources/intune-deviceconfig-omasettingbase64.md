---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6288803dd87afa7fe45525c20258bdded34482ea
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470751"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="80c72-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="80c72-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="80c72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80c72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80c72-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80c72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80c72-106">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="80c72-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="80c72-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80c72-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80c72-108">属性</span><span class="sxs-lookup"><span data-stu-id="80c72-108">Properties</span></span>
|<span data-ttu-id="80c72-109">属性</span><span class="sxs-lookup"><span data-stu-id="80c72-109">Property</span></span>|<span data-ttu-id="80c72-110">类型</span><span class="sxs-lookup"><span data-stu-id="80c72-110">Type</span></span>|<span data-ttu-id="80c72-111">说明</span><span class="sxs-lookup"><span data-stu-id="80c72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c72-112">displayName</span><span class="sxs-lookup"><span data-stu-id="80c72-112">displayName</span></span>|<span data-ttu-id="80c72-113">String</span><span class="sxs-lookup"><span data-stu-id="80c72-113">String</span></span>|<span data-ttu-id="80c72-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="80c72-114">Display Name.</span></span> <span data-ttu-id="80c72-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80c72-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="80c72-116">说明</span><span class="sxs-lookup"><span data-stu-id="80c72-116">description</span></span>|<span data-ttu-id="80c72-117">String</span><span class="sxs-lookup"><span data-stu-id="80c72-117">String</span></span>|<span data-ttu-id="80c72-118">说明。</span><span class="sxs-lookup"><span data-stu-id="80c72-118">Description.</span></span> <span data-ttu-id="80c72-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80c72-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="80c72-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="80c72-120">omaUri</span></span>|<span data-ttu-id="80c72-121">String</span><span class="sxs-lookup"><span data-stu-id="80c72-121">String</span></span>|<span data-ttu-id="80c72-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="80c72-122">OMA.</span></span> <span data-ttu-id="80c72-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="80c72-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="80c72-124">fileName</span><span class="sxs-lookup"><span data-stu-id="80c72-124">fileName</span></span>|<span data-ttu-id="80c72-125">String</span><span class="sxs-lookup"><span data-stu-id="80c72-125">String</span></span>|<span data-ttu-id="80c72-126">与 Value 属性 (\*.cer \| \*.crt \| \*.p7b \| \*.bin) 。</span><span class="sxs-lookup"><span data-stu-id="80c72-126">File name associated with the Value property (\*.cer \| \*.crt \| \*.p7b \| \*.bin).</span></span>|
|<span data-ttu-id="80c72-127">value</span><span class="sxs-lookup"><span data-stu-id="80c72-127">value</span></span>|<span data-ttu-id="80c72-128">String</span><span class="sxs-lookup"><span data-stu-id="80c72-128">String</span></span>|<span data-ttu-id="80c72-129">值。</span><span class="sxs-lookup"><span data-stu-id="80c72-129">Value.</span></span> <span data-ttu-id="80c72-130">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="80c72-130">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="80c72-131">关系</span><span class="sxs-lookup"><span data-stu-id="80c72-131">Relationships</span></span>
<span data-ttu-id="80c72-132">无</span><span class="sxs-lookup"><span data-stu-id="80c72-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80c72-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80c72-133">JSON Representation</span></span>
<span data-ttu-id="80c72-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80c72-134">Here is a JSON representation of the resource.</span></span>
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
  "fileName": "String",
  "value": "String"
}
```









