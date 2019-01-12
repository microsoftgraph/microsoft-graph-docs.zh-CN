---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2acf41d36b4a664166dc2b5ceeb17dc0b6db4495
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949841"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="61d81-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="61d81-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="61d81-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="61d81-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="61d81-105">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="61d81-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="61d81-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="61d81-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="61d81-107">属性</span><span class="sxs-lookup"><span data-stu-id="61d81-107">Properties</span></span>
|<span data-ttu-id="61d81-108">属性</span><span class="sxs-lookup"><span data-stu-id="61d81-108">Property</span></span>|<span data-ttu-id="61d81-109">类型</span><span class="sxs-lookup"><span data-stu-id="61d81-109">Type</span></span>|<span data-ttu-id="61d81-110">说明</span><span class="sxs-lookup"><span data-stu-id="61d81-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61d81-111">displayName</span><span class="sxs-lookup"><span data-stu-id="61d81-111">displayName</span></span>|<span data-ttu-id="61d81-112">String</span><span class="sxs-lookup"><span data-stu-id="61d81-112">String</span></span>|<span data-ttu-id="61d81-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="61d81-113">Display Name.</span></span> <span data-ttu-id="61d81-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="61d81-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="61d81-115">description</span><span class="sxs-lookup"><span data-stu-id="61d81-115">description</span></span>|<span data-ttu-id="61d81-116">String</span><span class="sxs-lookup"><span data-stu-id="61d81-116">String</span></span>|<span data-ttu-id="61d81-117">说明。</span><span class="sxs-lookup"><span data-stu-id="61d81-117">Description.</span></span> <span data-ttu-id="61d81-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="61d81-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="61d81-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="61d81-119">omaUri</span></span>|<span data-ttu-id="61d81-120">String</span><span class="sxs-lookup"><span data-stu-id="61d81-120">String</span></span>|<span data-ttu-id="61d81-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="61d81-121">OMA.</span></span> <span data-ttu-id="61d81-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="61d81-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="61d81-123">fileName</span><span class="sxs-lookup"><span data-stu-id="61d81-123">fileName</span></span>|<span data-ttu-id="61d81-124">String</span><span class="sxs-lookup"><span data-stu-id="61d81-124">String</span></span>|<span data-ttu-id="61d81-125">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="61d81-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="61d81-126">\*.crt</span><span class="sxs-lookup"><span data-stu-id="61d81-126">\*.crt</span></span> | <span data-ttu-id="61d81-127">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="61d81-127">\*.p7b</span></span> | <span data-ttu-id="61d81-128">\*.bin)。</span><span class="sxs-lookup"><span data-stu-id="61d81-128">\*.bin).</span></span>|
|<span data-ttu-id="61d81-129">值</span><span class="sxs-lookup"><span data-stu-id="61d81-129">value</span></span>|<span data-ttu-id="61d81-130">String</span><span class="sxs-lookup"><span data-stu-id="61d81-130">String</span></span>|<span data-ttu-id="61d81-131">值。</span><span class="sxs-lookup"><span data-stu-id="61d81-131">Value.</span></span> <span data-ttu-id="61d81-132">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="61d81-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="61d81-133">关系</span><span class="sxs-lookup"><span data-stu-id="61d81-133">Relationships</span></span>
<span data-ttu-id="61d81-134">无</span><span class="sxs-lookup"><span data-stu-id="61d81-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="61d81-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61d81-135">JSON Representation</span></span>
<span data-ttu-id="61d81-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61d81-136">Here is a JSON representation of the resource.</span></span>
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



