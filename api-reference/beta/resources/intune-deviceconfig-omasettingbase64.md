---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1f5089c40e2c79d0a3a2e9a920de10d8e5eb4bc1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402003"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="f3c75-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3c75-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="f3c75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3c75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3c75-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3c75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3c75-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3c75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3c75-107">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="f3c75-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="f3c75-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3c75-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3c75-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3c75-109">Properties</span></span>
|<span data-ttu-id="f3c75-110">属性</span><span class="sxs-lookup"><span data-stu-id="f3c75-110">Property</span></span>|<span data-ttu-id="f3c75-111">类型</span><span class="sxs-lookup"><span data-stu-id="f3c75-111">Type</span></span>|<span data-ttu-id="f3c75-112">说明</span><span class="sxs-lookup"><span data-stu-id="f3c75-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3c75-113">displayName</span><span class="sxs-lookup"><span data-stu-id="f3c75-113">displayName</span></span>|<span data-ttu-id="f3c75-114">字符串</span><span class="sxs-lookup"><span data-stu-id="f3c75-114">String</span></span>|<span data-ttu-id="f3c75-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f3c75-115">Display Name.</span></span> <span data-ttu-id="f3c75-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3c75-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3c75-117">description</span><span class="sxs-lookup"><span data-stu-id="f3c75-117">description</span></span>|<span data-ttu-id="f3c75-118">字符串</span><span class="sxs-lookup"><span data-stu-id="f3c75-118">String</span></span>|<span data-ttu-id="f3c75-119">说明。</span><span class="sxs-lookup"><span data-stu-id="f3c75-119">Description.</span></span> <span data-ttu-id="f3c75-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3c75-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3c75-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="f3c75-121">omaUri</span></span>|<span data-ttu-id="f3c75-122">String</span><span class="sxs-lookup"><span data-stu-id="f3c75-122">String</span></span>|<span data-ttu-id="f3c75-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="f3c75-123">OMA.</span></span> <span data-ttu-id="f3c75-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f3c75-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f3c75-125">fileName</span><span class="sxs-lookup"><span data-stu-id="f3c75-125">fileName</span></span>|<span data-ttu-id="f3c75-126">字符串</span><span class="sxs-lookup"><span data-stu-id="f3c75-126">String</span></span>|<span data-ttu-id="f3c75-127">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="f3c75-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="f3c75-128">\* .crt</span><span class="sxs-lookup"><span data-stu-id="f3c75-128">\*.crt</span></span> | <span data-ttu-id="f3c75-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="f3c75-129">\*.p7b</span></span> | <span data-ttu-id="f3c75-130">\* bin）。</span><span class="sxs-lookup"><span data-stu-id="f3c75-130">\*.bin).</span></span>|
|<span data-ttu-id="f3c75-131">value</span><span class="sxs-lookup"><span data-stu-id="f3c75-131">value</span></span>|<span data-ttu-id="f3c75-132">String</span><span class="sxs-lookup"><span data-stu-id="f3c75-132">String</span></span>|<span data-ttu-id="f3c75-133">值。</span><span class="sxs-lookup"><span data-stu-id="f3c75-133">Value.</span></span> <span data-ttu-id="f3c75-134">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="f3c75-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3c75-135">关系</span><span class="sxs-lookup"><span data-stu-id="f3c75-135">Relationships</span></span>
<span data-ttu-id="f3c75-136">无</span><span class="sxs-lookup"><span data-stu-id="f3c75-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3c75-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3c75-137">JSON Representation</span></span>
<span data-ttu-id="f3c75-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3c75-138">Here is a JSON representation of the resource.</span></span>
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



