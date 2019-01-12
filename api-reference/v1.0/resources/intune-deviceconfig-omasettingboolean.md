---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f0b3f2d04c9476cc10a67c1e68ba9a29288e8875
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986633"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="c7ed9-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7ed9-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="c7ed9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c7ed9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7ed9-105">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="c7ed9-105">OMA Settings Boolean definition.</span></span>

<span data-ttu-id="c7ed9-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed9-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c7ed9-107">属性</span><span class="sxs-lookup"><span data-stu-id="c7ed9-107">Properties</span></span>
|<span data-ttu-id="c7ed9-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7ed9-108">Property</span></span>|<span data-ttu-id="c7ed9-109">类型</span><span class="sxs-lookup"><span data-stu-id="c7ed9-109">Type</span></span>|<span data-ttu-id="c7ed9-110">说明</span><span class="sxs-lookup"><span data-stu-id="c7ed9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7ed9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c7ed9-111">displayName</span></span>|<span data-ttu-id="c7ed9-112">String</span><span class="sxs-lookup"><span data-stu-id="c7ed9-112">String</span></span>|<span data-ttu-id="c7ed9-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="c7ed9-113">Display Name.</span></span> <span data-ttu-id="c7ed9-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed9-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c7ed9-115">description</span><span class="sxs-lookup"><span data-stu-id="c7ed9-115">description</span></span>|<span data-ttu-id="c7ed9-116">String</span><span class="sxs-lookup"><span data-stu-id="c7ed9-116">String</span></span>|<span data-ttu-id="c7ed9-117">说明。</span><span class="sxs-lookup"><span data-stu-id="c7ed9-117">Description.</span></span> <span data-ttu-id="c7ed9-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed9-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c7ed9-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="c7ed9-119">omaUri</span></span>|<span data-ttu-id="c7ed9-120">String</span><span class="sxs-lookup"><span data-stu-id="c7ed9-120">String</span></span>|<span data-ttu-id="c7ed9-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="c7ed9-121">OMA.</span></span> <span data-ttu-id="c7ed9-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="c7ed9-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c7ed9-123">value</span><span class="sxs-lookup"><span data-stu-id="c7ed9-123">value</span></span>|<span data-ttu-id="c7ed9-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7ed9-124">Boolean</span></span>|<span data-ttu-id="c7ed9-125">值。</span><span class="sxs-lookup"><span data-stu-id="c7ed9-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7ed9-126">关系</span><span class="sxs-lookup"><span data-stu-id="c7ed9-126">Relationships</span></span>
<span data-ttu-id="c7ed9-127">无</span><span class="sxs-lookup"><span data-stu-id="c7ed9-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c7ed9-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7ed9-128">JSON Representation</span></span>
<span data-ttu-id="c7ed9-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7ed9-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



