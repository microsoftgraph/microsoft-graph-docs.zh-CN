---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ddb11f40faf9db58fefb984fcc08a9fedd66e97d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951549"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="f92f9-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="f92f9-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="f92f9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f92f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f92f9-105">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="f92f9-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="f92f9-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f92f9-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f92f9-107">属性</span><span class="sxs-lookup"><span data-stu-id="f92f9-107">Properties</span></span>
|<span data-ttu-id="f92f9-108">属性</span><span class="sxs-lookup"><span data-stu-id="f92f9-108">Property</span></span>|<span data-ttu-id="f92f9-109">类型</span><span class="sxs-lookup"><span data-stu-id="f92f9-109">Type</span></span>|<span data-ttu-id="f92f9-110">说明</span><span class="sxs-lookup"><span data-stu-id="f92f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f92f9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f92f9-111">displayName</span></span>|<span data-ttu-id="f92f9-112">String</span><span class="sxs-lookup"><span data-stu-id="f92f9-112">String</span></span>|<span data-ttu-id="f92f9-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f92f9-113">Display Name.</span></span> <span data-ttu-id="f92f9-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f92f9-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f92f9-115">description</span><span class="sxs-lookup"><span data-stu-id="f92f9-115">description</span></span>|<span data-ttu-id="f92f9-116">String</span><span class="sxs-lookup"><span data-stu-id="f92f9-116">String</span></span>|<span data-ttu-id="f92f9-117">说明。</span><span class="sxs-lookup"><span data-stu-id="f92f9-117">Description.</span></span> <span data-ttu-id="f92f9-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f92f9-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f92f9-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f92f9-119">omaUri</span></span>|<span data-ttu-id="f92f9-120">String</span><span class="sxs-lookup"><span data-stu-id="f92f9-120">String</span></span>|<span data-ttu-id="f92f9-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="f92f9-121">OMA.</span></span> <span data-ttu-id="f92f9-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f92f9-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f92f9-123">value</span><span class="sxs-lookup"><span data-stu-id="f92f9-123">value</span></span>|<span data-ttu-id="f92f9-124">单个</span><span class="sxs-lookup"><span data-stu-id="f92f9-124">Single</span></span>|<span data-ttu-id="f92f9-125">值。</span><span class="sxs-lookup"><span data-stu-id="f92f9-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f92f9-126">关系</span><span class="sxs-lookup"><span data-stu-id="f92f9-126">Relationships</span></span>
<span data-ttu-id="f92f9-127">无</span><span class="sxs-lookup"><span data-stu-id="f92f9-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f92f9-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f92f9-128">JSON Representation</span></span>
<span data-ttu-id="f92f9-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f92f9-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



