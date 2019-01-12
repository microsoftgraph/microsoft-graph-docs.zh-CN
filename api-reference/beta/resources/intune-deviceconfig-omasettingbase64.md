---
title: omaSettingBase64 资源类型
description: OMA 设置 Base64 定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f1c6a488adf2f39b2c415e31c4919380ebda5ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982566"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="073b1-103">omaSettingBase64 资源类型</span><span class="sxs-lookup"><span data-stu-id="073b1-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="073b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="073b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="073b1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="073b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="073b1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="073b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="073b1-107">OMA 设置 Base64 定义。</span><span class="sxs-lookup"><span data-stu-id="073b1-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="073b1-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="073b1-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="073b1-109">属性</span><span class="sxs-lookup"><span data-stu-id="073b1-109">Properties</span></span>
|<span data-ttu-id="073b1-110">属性</span><span class="sxs-lookup"><span data-stu-id="073b1-110">Property</span></span>|<span data-ttu-id="073b1-111">类型</span><span class="sxs-lookup"><span data-stu-id="073b1-111">Type</span></span>|<span data-ttu-id="073b1-112">说明</span><span class="sxs-lookup"><span data-stu-id="073b1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="073b1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="073b1-113">displayName</span></span>|<span data-ttu-id="073b1-114">String</span><span class="sxs-lookup"><span data-stu-id="073b1-114">String</span></span>|<span data-ttu-id="073b1-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="073b1-115">Display Name.</span></span> <span data-ttu-id="073b1-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="073b1-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="073b1-117">description</span><span class="sxs-lookup"><span data-stu-id="073b1-117">description</span></span>|<span data-ttu-id="073b1-118">String</span><span class="sxs-lookup"><span data-stu-id="073b1-118">String</span></span>|<span data-ttu-id="073b1-119">说明。</span><span class="sxs-lookup"><span data-stu-id="073b1-119">Description.</span></span> <span data-ttu-id="073b1-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="073b1-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="073b1-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="073b1-121">omaUri</span></span>|<span data-ttu-id="073b1-122">String</span><span class="sxs-lookup"><span data-stu-id="073b1-122">String</span></span>|<span data-ttu-id="073b1-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="073b1-123">OMA.</span></span> <span data-ttu-id="073b1-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="073b1-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="073b1-125">fileName</span><span class="sxs-lookup"><span data-stu-id="073b1-125">fileName</span></span>|<span data-ttu-id="073b1-126">String</span><span class="sxs-lookup"><span data-stu-id="073b1-126">String</span></span>|<span data-ttu-id="073b1-127">与 Value 属性 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="073b1-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="073b1-128">\*.crt</span><span class="sxs-lookup"><span data-stu-id="073b1-128">\*.crt</span></span> | <span data-ttu-id="073b1-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="073b1-129">\*.p7b</span></span> | <span data-ttu-id="073b1-130">\*.bin)。</span><span class="sxs-lookup"><span data-stu-id="073b1-130">\*.bin).</span></span>|
|<span data-ttu-id="073b1-131">值</span><span class="sxs-lookup"><span data-stu-id="073b1-131">value</span></span>|<span data-ttu-id="073b1-132">String</span><span class="sxs-lookup"><span data-stu-id="073b1-132">String</span></span>|<span data-ttu-id="073b1-133">值。</span><span class="sxs-lookup"><span data-stu-id="073b1-133">Value.</span></span> <span data-ttu-id="073b1-134">（Base64 编码字符串）</span><span class="sxs-lookup"><span data-stu-id="073b1-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="073b1-135">关系</span><span class="sxs-lookup"><span data-stu-id="073b1-135">Relationships</span></span>
<span data-ttu-id="073b1-136">无</span><span class="sxs-lookup"><span data-stu-id="073b1-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="073b1-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="073b1-137">JSON Representation</span></span>
<span data-ttu-id="073b1-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="073b1-138">Here is a JSON representation of the resource.</span></span>
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





