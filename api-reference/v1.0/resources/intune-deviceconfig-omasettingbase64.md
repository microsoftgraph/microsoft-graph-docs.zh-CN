---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9aa6dd320fd04c352208692f988ea487eb28a47c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530590"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="43561-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="43561-103">omaSettingBase64 resource type</span></span>

<span data-ttu-id="43561-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43561-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43561-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43561-106">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="43561-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="43561-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43561-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="43561-108">属性</span><span class="sxs-lookup"><span data-stu-id="43561-108">Properties</span></span>
|<span data-ttu-id="43561-109">属性</span><span class="sxs-lookup"><span data-stu-id="43561-109">Property</span></span>|<span data-ttu-id="43561-110">类型</span><span class="sxs-lookup"><span data-stu-id="43561-110">Type</span></span>|<span data-ttu-id="43561-111">说明</span><span class="sxs-lookup"><span data-stu-id="43561-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43561-112">displayName</span><span class="sxs-lookup"><span data-stu-id="43561-112">displayName</span></span>|<span data-ttu-id="43561-113">字符串</span><span class="sxs-lookup"><span data-stu-id="43561-113">String</span></span>|<span data-ttu-id="43561-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="43561-114">Display Name.</span></span> <span data-ttu-id="43561-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43561-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="43561-116">说明</span><span class="sxs-lookup"><span data-stu-id="43561-116">description</span></span>|<span data-ttu-id="43561-117">字符串</span><span class="sxs-lookup"><span data-stu-id="43561-117">String</span></span>|<span data-ttu-id="43561-118">说明。</span><span class="sxs-lookup"><span data-stu-id="43561-118">Description.</span></span> <span data-ttu-id="43561-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43561-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="43561-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="43561-120">omaUri</span></span>|<span data-ttu-id="43561-121">String</span><span class="sxs-lookup"><span data-stu-id="43561-121">String</span></span>|<span data-ttu-id="43561-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="43561-122">OMA.</span></span> <span data-ttu-id="43561-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="43561-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="43561-124">fileName</span><span class="sxs-lookup"><span data-stu-id="43561-124">fileName</span></span>|<span data-ttu-id="43561-125">字符串</span><span class="sxs-lookup"><span data-stu-id="43561-125">String</span></span>|<span data-ttu-id="43561-126">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="43561-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="43561-127">\* .crt</span><span class="sxs-lookup"><span data-stu-id="43561-127">\*.crt</span></span> | <span data-ttu-id="43561-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="43561-128">\*.p7b</span></span> | <span data-ttu-id="43561-129">\* bin）。</span><span class="sxs-lookup"><span data-stu-id="43561-129">\*.bin).</span></span>|
|<span data-ttu-id="43561-130">value</span><span class="sxs-lookup"><span data-stu-id="43561-130">value</span></span>|<span data-ttu-id="43561-131">String</span><span class="sxs-lookup"><span data-stu-id="43561-131">String</span></span>|<span data-ttu-id="43561-132">值。</span><span class="sxs-lookup"><span data-stu-id="43561-132">Value.</span></span> <span data-ttu-id="43561-133">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="43561-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="43561-134">关系</span><span class="sxs-lookup"><span data-stu-id="43561-134">Relationships</span></span>
<span data-ttu-id="43561-135">无</span><span class="sxs-lookup"><span data-stu-id="43561-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43561-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43561-136">JSON Representation</span></span>
<span data-ttu-id="43561-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43561-137">Here is a JSON representation of the resource.</span></span>
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




