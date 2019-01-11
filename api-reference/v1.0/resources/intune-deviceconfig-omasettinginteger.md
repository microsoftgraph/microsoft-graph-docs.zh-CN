---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f40d5d225c2b4b99573c482b39f886bcd463e9fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860450"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="860bd-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="860bd-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="860bd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="860bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="860bd-105">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="860bd-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="860bd-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="860bd-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="860bd-107">属性</span><span class="sxs-lookup"><span data-stu-id="860bd-107">Properties</span></span>
|<span data-ttu-id="860bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="860bd-108">Property</span></span>|<span data-ttu-id="860bd-109">类型</span><span class="sxs-lookup"><span data-stu-id="860bd-109">Type</span></span>|<span data-ttu-id="860bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="860bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="860bd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="860bd-111">displayName</span></span>|<span data-ttu-id="860bd-112">String</span><span class="sxs-lookup"><span data-stu-id="860bd-112">String</span></span>|<span data-ttu-id="860bd-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="860bd-113">Display Name.</span></span> <span data-ttu-id="860bd-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="860bd-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="860bd-115">description</span><span class="sxs-lookup"><span data-stu-id="860bd-115">description</span></span>|<span data-ttu-id="860bd-116">String</span><span class="sxs-lookup"><span data-stu-id="860bd-116">String</span></span>|<span data-ttu-id="860bd-117">说明。</span><span class="sxs-lookup"><span data-stu-id="860bd-117">Description.</span></span> <span data-ttu-id="860bd-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="860bd-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="860bd-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="860bd-119">omaUri</span></span>|<span data-ttu-id="860bd-120">String</span><span class="sxs-lookup"><span data-stu-id="860bd-120">String</span></span>|<span data-ttu-id="860bd-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="860bd-121">OMA.</span></span> <span data-ttu-id="860bd-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="860bd-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="860bd-123">值</span><span class="sxs-lookup"><span data-stu-id="860bd-123">value</span></span>|<span data-ttu-id="860bd-124">Int32</span><span class="sxs-lookup"><span data-stu-id="860bd-124">Int32</span></span>|<span data-ttu-id="860bd-125">值。</span><span class="sxs-lookup"><span data-stu-id="860bd-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="860bd-126">关系</span><span class="sxs-lookup"><span data-stu-id="860bd-126">Relationships</span></span>
<span data-ttu-id="860bd-127">无</span><span class="sxs-lookup"><span data-stu-id="860bd-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="860bd-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="860bd-128">JSON Representation</span></span>
<span data-ttu-id="860bd-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="860bd-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



