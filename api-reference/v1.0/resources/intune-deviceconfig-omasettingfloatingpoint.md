---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: tfitzmac
ms.openlocfilehash: efed2112f85ee0600fcbe499616a7f3e787beb59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360751"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="faef0-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="faef0-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="faef0-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="faef0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faef0-105">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="faef0-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="faef0-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="faef0-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="faef0-107">属性</span><span class="sxs-lookup"><span data-stu-id="faef0-107">Properties</span></span>
|<span data-ttu-id="faef0-108">属性</span><span class="sxs-lookup"><span data-stu-id="faef0-108">Property</span></span>|<span data-ttu-id="faef0-109">类型</span><span class="sxs-lookup"><span data-stu-id="faef0-109">Type</span></span>|<span data-ttu-id="faef0-110">说明</span><span class="sxs-lookup"><span data-stu-id="faef0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faef0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="faef0-111">displayName</span></span>|<span data-ttu-id="faef0-112">String</span><span class="sxs-lookup"><span data-stu-id="faef0-112">String</span></span>|<span data-ttu-id="faef0-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="faef0-113">Display Name.</span></span> <span data-ttu-id="faef0-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="faef0-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="faef0-115">description</span><span class="sxs-lookup"><span data-stu-id="faef0-115">description</span></span>|<span data-ttu-id="faef0-116">String</span><span class="sxs-lookup"><span data-stu-id="faef0-116">String</span></span>|<span data-ttu-id="faef0-117">说明。</span><span class="sxs-lookup"><span data-stu-id="faef0-117">Description.</span></span> <span data-ttu-id="faef0-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="faef0-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="faef0-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="faef0-119">omaUri</span></span>|<span data-ttu-id="faef0-120">String</span><span class="sxs-lookup"><span data-stu-id="faef0-120">String</span></span>|<span data-ttu-id="faef0-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="faef0-121">OMA.</span></span> <span data-ttu-id="faef0-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="faef0-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="faef0-123">value</span><span class="sxs-lookup"><span data-stu-id="faef0-123">value</span></span>|<span data-ttu-id="faef0-124">单个</span><span class="sxs-lookup"><span data-stu-id="faef0-124">Single</span></span>|<span data-ttu-id="faef0-125">值。</span><span class="sxs-lookup"><span data-stu-id="faef0-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faef0-126">关系</span><span class="sxs-lookup"><span data-stu-id="faef0-126">Relationships</span></span>
<span data-ttu-id="faef0-127">无</span><span class="sxs-lookup"><span data-stu-id="faef0-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="faef0-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faef0-128">JSON Representation</span></span>
<span data-ttu-id="faef0-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faef0-129">Here is a JSON representation of the resource.</span></span>
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



