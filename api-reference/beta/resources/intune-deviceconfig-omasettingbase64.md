---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cba87b6ce02f9683de9e4013585b2a960f8df512
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529569"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="e5a96-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5a96-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="e5a96-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e5a96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5a96-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5a96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5a96-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5a96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5a96-107">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="e5a96-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="e5a96-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5a96-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e5a96-109">属性</span><span class="sxs-lookup"><span data-stu-id="e5a96-109">Properties</span></span>
|<span data-ttu-id="e5a96-110">属性</span><span class="sxs-lookup"><span data-stu-id="e5a96-110">Property</span></span>|<span data-ttu-id="e5a96-111">类型</span><span class="sxs-lookup"><span data-stu-id="e5a96-111">Type</span></span>|<span data-ttu-id="e5a96-112">说明</span><span class="sxs-lookup"><span data-stu-id="e5a96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5a96-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e5a96-113">displayName</span></span>|<span data-ttu-id="e5a96-114">字符串</span><span class="sxs-lookup"><span data-stu-id="e5a96-114">String</span></span>|<span data-ttu-id="e5a96-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e5a96-115">Display Name.</span></span> <span data-ttu-id="e5a96-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5a96-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e5a96-117">说明</span><span class="sxs-lookup"><span data-stu-id="e5a96-117">description</span></span>|<span data-ttu-id="e5a96-118">String</span><span class="sxs-lookup"><span data-stu-id="e5a96-118">String</span></span>|<span data-ttu-id="e5a96-119">说明。</span><span class="sxs-lookup"><span data-stu-id="e5a96-119">Description.</span></span> <span data-ttu-id="e5a96-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5a96-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e5a96-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="e5a96-121">omaUri</span></span>|<span data-ttu-id="e5a96-122">String</span><span class="sxs-lookup"><span data-stu-id="e5a96-122">String</span></span>|<span data-ttu-id="e5a96-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="e5a96-123">OMA.</span></span> <span data-ttu-id="e5a96-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e5a96-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e5a96-125">fileName</span><span class="sxs-lookup"><span data-stu-id="e5a96-125">fileName</span></span>|<span data-ttu-id="e5a96-126">String</span><span class="sxs-lookup"><span data-stu-id="e5a96-126">String</span></span>|<span data-ttu-id="e5a96-127">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="e5a96-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="e5a96-128">\* .crt</span><span class="sxs-lookup"><span data-stu-id="e5a96-128">\*.crt</span></span> | <span data-ttu-id="e5a96-129">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="e5a96-129">\*.p7b</span></span> | <span data-ttu-id="e5a96-130">\* bin）。</span><span class="sxs-lookup"><span data-stu-id="e5a96-130">\*.bin).</span></span>|
|<span data-ttu-id="e5a96-131">value</span><span class="sxs-lookup"><span data-stu-id="e5a96-131">value</span></span>|<span data-ttu-id="e5a96-132">String</span><span class="sxs-lookup"><span data-stu-id="e5a96-132">String</span></span>|<span data-ttu-id="e5a96-133">值。</span><span class="sxs-lookup"><span data-stu-id="e5a96-133">Value.</span></span> <span data-ttu-id="e5a96-134">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="e5a96-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5a96-135">关系</span><span class="sxs-lookup"><span data-stu-id="e5a96-135">Relationships</span></span>
<span data-ttu-id="e5a96-136">无</span><span class="sxs-lookup"><span data-stu-id="e5a96-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5a96-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5a96-137">JSON Representation</span></span>
<span data-ttu-id="e5a96-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5a96-138">Here is a JSON representation of the resource.</span></span>
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



