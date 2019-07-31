---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f5fd4df9b5deb49745d337632cfe103fdaad0581
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011426"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="ce153-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce153-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="ce153-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce153-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce153-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce153-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce153-106">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="ce153-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="ce153-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce153-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce153-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce153-108">Properties</span></span>
|<span data-ttu-id="ce153-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce153-109">Property</span></span>|<span data-ttu-id="ce153-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce153-110">Type</span></span>|<span data-ttu-id="ce153-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce153-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce153-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ce153-112">displayName</span></span>|<span data-ttu-id="ce153-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ce153-113">String</span></span>|<span data-ttu-id="ce153-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ce153-114">Display Name.</span></span> <span data-ttu-id="ce153-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce153-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce153-116">说明</span><span class="sxs-lookup"><span data-stu-id="ce153-116">description</span></span>|<span data-ttu-id="ce153-117">String</span><span class="sxs-lookup"><span data-stu-id="ce153-117">String</span></span>|<span data-ttu-id="ce153-118">说明。</span><span class="sxs-lookup"><span data-stu-id="ce153-118">Description.</span></span> <span data-ttu-id="ce153-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce153-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce153-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="ce153-120">omaUri</span></span>|<span data-ttu-id="ce153-121">String</span><span class="sxs-lookup"><span data-stu-id="ce153-121">String</span></span>|<span data-ttu-id="ce153-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="ce153-122">OMA.</span></span> <span data-ttu-id="ce153-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ce153-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ce153-124">fileName</span><span class="sxs-lookup"><span data-stu-id="ce153-124">fileName</span></span>|<span data-ttu-id="ce153-125">String</span><span class="sxs-lookup"><span data-stu-id="ce153-125">String</span></span>|<span data-ttu-id="ce153-126">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="ce153-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="ce153-127">\* .crt</span><span class="sxs-lookup"><span data-stu-id="ce153-127">\*.crt</span></span> | <span data-ttu-id="ce153-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="ce153-128">\*.p7b</span></span> | <span data-ttu-id="ce153-129">\* bin)。</span><span class="sxs-lookup"><span data-stu-id="ce153-129">\*.bin).</span></span>|
|<span data-ttu-id="ce153-130">value</span><span class="sxs-lookup"><span data-stu-id="ce153-130">value</span></span>|<span data-ttu-id="ce153-131">String</span><span class="sxs-lookup"><span data-stu-id="ce153-131">String</span></span>|<span data-ttu-id="ce153-132">值。</span><span class="sxs-lookup"><span data-stu-id="ce153-132">Value.</span></span> <span data-ttu-id="ce153-133">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="ce153-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce153-134">关系</span><span class="sxs-lookup"><span data-stu-id="ce153-134">Relationships</span></span>
<span data-ttu-id="ce153-135">无</span><span class="sxs-lookup"><span data-stu-id="ce153-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce153-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce153-136">JSON Representation</span></span>
<span data-ttu-id="ce153-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce153-137">Here is a JSON representation of the resource.</span></span>
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





