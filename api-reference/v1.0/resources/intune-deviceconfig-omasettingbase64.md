---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678c6e78070a7aae185a041962083b7908ef1cc1
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258588"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="fa908-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa908-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="fa908-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa908-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa908-105">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="fa908-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="fa908-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa908-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa908-107">属性</span><span class="sxs-lookup"><span data-stu-id="fa908-107">Properties</span></span>
|<span data-ttu-id="fa908-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa908-108">Property</span></span>|<span data-ttu-id="fa908-109">类型</span><span class="sxs-lookup"><span data-stu-id="fa908-109">Type</span></span>|<span data-ttu-id="fa908-110">说明</span><span class="sxs-lookup"><span data-stu-id="fa908-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa908-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fa908-111">displayName</span></span>|<span data-ttu-id="fa908-112">String</span><span class="sxs-lookup"><span data-stu-id="fa908-112">String</span></span>|<span data-ttu-id="fa908-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="fa908-113">Display Name.</span></span> <span data-ttu-id="fa908-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa908-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fa908-115">description</span><span class="sxs-lookup"><span data-stu-id="fa908-115">description</span></span>|<span data-ttu-id="fa908-116">字符串</span><span class="sxs-lookup"><span data-stu-id="fa908-116">String</span></span>|<span data-ttu-id="fa908-117">说明。</span><span class="sxs-lookup"><span data-stu-id="fa908-117">Description.</span></span> <span data-ttu-id="fa908-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa908-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fa908-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="fa908-119">omaUri</span></span>|<span data-ttu-id="fa908-120">String</span><span class="sxs-lookup"><span data-stu-id="fa908-120">String</span></span>|<span data-ttu-id="fa908-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="fa908-121">OMA.</span></span> <span data-ttu-id="fa908-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="fa908-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="fa908-123">fileName</span><span class="sxs-lookup"><span data-stu-id="fa908-123">fileName</span></span>|<span data-ttu-id="fa908-124">String</span><span class="sxs-lookup"><span data-stu-id="fa908-124">String</span></span>|<span data-ttu-id="fa908-125">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="fa908-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="fa908-126">\* .crt</span><span class="sxs-lookup"><span data-stu-id="fa908-126">\*.crt</span></span> | <span data-ttu-id="fa908-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="fa908-127">\*.p7b</span></span> | <span data-ttu-id="fa908-128">\* bin)。</span><span class="sxs-lookup"><span data-stu-id="fa908-128">\*.bin).</span></span>|
|<span data-ttu-id="fa908-129">值</span><span class="sxs-lookup"><span data-stu-id="fa908-129">value</span></span>|<span data-ttu-id="fa908-130">String</span><span class="sxs-lookup"><span data-stu-id="fa908-130">String</span></span>|<span data-ttu-id="fa908-131">值。</span><span class="sxs-lookup"><span data-stu-id="fa908-131">Value.</span></span> <span data-ttu-id="fa908-132">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="fa908-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa908-133">关系</span><span class="sxs-lookup"><span data-stu-id="fa908-133">Relationships</span></span>
<span data-ttu-id="fa908-134">无</span><span class="sxs-lookup"><span data-stu-id="fa908-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa908-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa908-135">JSON Representation</span></span>
<span data-ttu-id="fa908-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa908-136">Here is a JSON representation of the resource.</span></span>
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



