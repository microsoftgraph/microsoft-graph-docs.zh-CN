---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 890d636afb29fbfb188e9c1b514eecc6360001b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841347"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="6bf83-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="6bf83-103">omaSettingString resource type</span></span>

> <span data-ttu-id="6bf83-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6bf83-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf83-105">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="6bf83-105">OMA Settings String definition.</span></span>

<span data-ttu-id="6bf83-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6bf83-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6bf83-107">属性</span><span class="sxs-lookup"><span data-stu-id="6bf83-107">Properties</span></span>
|<span data-ttu-id="6bf83-108">属性</span><span class="sxs-lookup"><span data-stu-id="6bf83-108">Property</span></span>|<span data-ttu-id="6bf83-109">类型</span><span class="sxs-lookup"><span data-stu-id="6bf83-109">Type</span></span>|<span data-ttu-id="6bf83-110">说明</span><span class="sxs-lookup"><span data-stu-id="6bf83-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf83-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6bf83-111">displayName</span></span>|<span data-ttu-id="6bf83-112">String</span><span class="sxs-lookup"><span data-stu-id="6bf83-112">String</span></span>|<span data-ttu-id="6bf83-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="6bf83-113">Display Name.</span></span> <span data-ttu-id="6bf83-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6bf83-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6bf83-115">description</span><span class="sxs-lookup"><span data-stu-id="6bf83-115">description</span></span>|<span data-ttu-id="6bf83-116">String</span><span class="sxs-lookup"><span data-stu-id="6bf83-116">String</span></span>|<span data-ttu-id="6bf83-117">说明。</span><span class="sxs-lookup"><span data-stu-id="6bf83-117">Description.</span></span> <span data-ttu-id="6bf83-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6bf83-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6bf83-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="6bf83-119">omaUri</span></span>|<span data-ttu-id="6bf83-120">String</span><span class="sxs-lookup"><span data-stu-id="6bf83-120">String</span></span>|<span data-ttu-id="6bf83-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="6bf83-121">OMA.</span></span> <span data-ttu-id="6bf83-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="6bf83-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6bf83-123">值</span><span class="sxs-lookup"><span data-stu-id="6bf83-123">value</span></span>|<span data-ttu-id="6bf83-124">String</span><span class="sxs-lookup"><span data-stu-id="6bf83-124">String</span></span>|<span data-ttu-id="6bf83-125">值。</span><span class="sxs-lookup"><span data-stu-id="6bf83-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6bf83-126">关系</span><span class="sxs-lookup"><span data-stu-id="6bf83-126">Relationships</span></span>
<span data-ttu-id="6bf83-127">无</span><span class="sxs-lookup"><span data-stu-id="6bf83-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6bf83-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6bf83-128">JSON Representation</span></span>
<span data-ttu-id="6bf83-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6bf83-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



