---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
ms.openlocfilehash: 6b0835864d3ec8f8364a15ff293a75dfeded3a0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343720"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="49627-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="49627-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="49627-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49627-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49627-105">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="49627-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="49627-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49627-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49627-107">属性</span><span class="sxs-lookup"><span data-stu-id="49627-107">Properties</span></span>
|<span data-ttu-id="49627-108">属性</span><span class="sxs-lookup"><span data-stu-id="49627-108">Property</span></span>|<span data-ttu-id="49627-109">类型</span><span class="sxs-lookup"><span data-stu-id="49627-109">Type</span></span>|<span data-ttu-id="49627-110">说明</span><span class="sxs-lookup"><span data-stu-id="49627-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49627-111">displayName</span><span class="sxs-lookup"><span data-stu-id="49627-111">displayName</span></span>|<span data-ttu-id="49627-112">String</span><span class="sxs-lookup"><span data-stu-id="49627-112">String</span></span>|<span data-ttu-id="49627-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="49627-113">Display Name.</span></span> <span data-ttu-id="49627-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49627-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="49627-115">description</span><span class="sxs-lookup"><span data-stu-id="49627-115">description</span></span>|<span data-ttu-id="49627-116">String</span><span class="sxs-lookup"><span data-stu-id="49627-116">String</span></span>|<span data-ttu-id="49627-117">说明。</span><span class="sxs-lookup"><span data-stu-id="49627-117">Description.</span></span> <span data-ttu-id="49627-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49627-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="49627-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="49627-119">omaUri</span></span>|<span data-ttu-id="49627-120">String</span><span class="sxs-lookup"><span data-stu-id="49627-120">String</span></span>|<span data-ttu-id="49627-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="49627-121">OMA.</span></span> <span data-ttu-id="49627-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="49627-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="49627-123">fileName</span><span class="sxs-lookup"><span data-stu-id="49627-123">fileName</span></span>|<span data-ttu-id="49627-124">String</span><span class="sxs-lookup"><span data-stu-id="49627-124">String</span></span>|<span data-ttu-id="49627-125">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="49627-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="49627-126">\*.crt</span><span class="sxs-lookup"><span data-stu-id="49627-126">\*.crt</span></span> | <span data-ttu-id="49627-127">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="49627-127">\*.p7b</span></span> | <span data-ttu-id="49627-128">\*.bin)。</span><span class="sxs-lookup"><span data-stu-id="49627-128">\*.bin).</span></span>|
|<span data-ttu-id="49627-129">值</span><span class="sxs-lookup"><span data-stu-id="49627-129">value</span></span>|<span data-ttu-id="49627-130">String</span><span class="sxs-lookup"><span data-stu-id="49627-130">String</span></span>|<span data-ttu-id="49627-131">值。</span><span class="sxs-lookup"><span data-stu-id="49627-131">Value.</span></span> <span data-ttu-id="49627-132">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="49627-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="49627-133">关系</span><span class="sxs-lookup"><span data-stu-id="49627-133">Relationships</span></span>
<span data-ttu-id="49627-134">无</span><span class="sxs-lookup"><span data-stu-id="49627-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="49627-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49627-135">JSON Representation</span></span>
<span data-ttu-id="49627-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49627-136">Here is a JSON representation of the resource.</span></span>
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



