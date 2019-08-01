---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8ab8552205084f41599a37c4a8edf39f329d85d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028040"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="d5e2d-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5e2d-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="d5e2d-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5e2d-105">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="d5e2d-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5e2d-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d5e2d-107">属性</span><span class="sxs-lookup"><span data-stu-id="d5e2d-107">Properties</span></span>
|<span data-ttu-id="d5e2d-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5e2d-108">Property</span></span>|<span data-ttu-id="d5e2d-109">类型</span><span class="sxs-lookup"><span data-stu-id="d5e2d-109">Type</span></span>|<span data-ttu-id="d5e2d-110">说明</span><span class="sxs-lookup"><span data-stu-id="d5e2d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5e2d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d5e2d-111">displayName</span></span>|<span data-ttu-id="d5e2d-112">字符串</span><span class="sxs-lookup"><span data-stu-id="d5e2d-112">String</span></span>|<span data-ttu-id="d5e2d-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-113">Display Name.</span></span> <span data-ttu-id="d5e2d-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5e2d-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d5e2d-115">说明</span><span class="sxs-lookup"><span data-stu-id="d5e2d-115">description</span></span>|<span data-ttu-id="d5e2d-116">String</span><span class="sxs-lookup"><span data-stu-id="d5e2d-116">String</span></span>|<span data-ttu-id="d5e2d-117">说明。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-117">Description.</span></span> <span data-ttu-id="d5e2d-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5e2d-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d5e2d-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="d5e2d-119">omaUri</span></span>|<span data-ttu-id="d5e2d-120">String</span><span class="sxs-lookup"><span data-stu-id="d5e2d-120">String</span></span>|<span data-ttu-id="d5e2d-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-121">OMA.</span></span> <span data-ttu-id="d5e2d-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d5e2d-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d5e2d-123">fileName</span><span class="sxs-lookup"><span data-stu-id="d5e2d-123">fileName</span></span>|<span data-ttu-id="d5e2d-124">String</span><span class="sxs-lookup"><span data-stu-id="d5e2d-124">String</span></span>|<span data-ttu-id="d5e2d-125">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="d5e2d-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="d5e2d-126">\* .crt</span><span class="sxs-lookup"><span data-stu-id="d5e2d-126">\*.crt</span></span> | <span data-ttu-id="d5e2d-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="d5e2d-127">\*.p7b</span></span> | <span data-ttu-id="d5e2d-128">\* bin)。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-128">\*.bin).</span></span>|
|<span data-ttu-id="d5e2d-129">value</span><span class="sxs-lookup"><span data-stu-id="d5e2d-129">value</span></span>|<span data-ttu-id="d5e2d-130">String</span><span class="sxs-lookup"><span data-stu-id="d5e2d-130">String</span></span>|<span data-ttu-id="d5e2d-131">值。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-131">Value.</span></span> <span data-ttu-id="d5e2d-132">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="d5e2d-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5e2d-133">关系</span><span class="sxs-lookup"><span data-stu-id="d5e2d-133">Relationships</span></span>
<span data-ttu-id="d5e2d-134">无</span><span class="sxs-lookup"><span data-stu-id="d5e2d-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5e2d-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5e2d-135">JSON Representation</span></span>
<span data-ttu-id="d5e2d-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5e2d-136">Here is a JSON representation of the resource.</span></span>
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



