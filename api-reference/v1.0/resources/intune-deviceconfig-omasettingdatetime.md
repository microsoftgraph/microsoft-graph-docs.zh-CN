---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: afd66ce8838abc3ade8857ec5a4bda74144d6792
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865177"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="e1cb5-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1cb5-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="e1cb5-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1cb5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1cb5-105">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="e1cb5-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="e1cb5-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1cb5-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e1cb5-107">属性</span><span class="sxs-lookup"><span data-stu-id="e1cb5-107">Properties</span></span>
|<span data-ttu-id="e1cb5-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1cb5-108">Property</span></span>|<span data-ttu-id="e1cb5-109">类型</span><span class="sxs-lookup"><span data-stu-id="e1cb5-109">Type</span></span>|<span data-ttu-id="e1cb5-110">说明</span><span class="sxs-lookup"><span data-stu-id="e1cb5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1cb5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e1cb5-111">displayName</span></span>|<span data-ttu-id="e1cb5-112">String</span><span class="sxs-lookup"><span data-stu-id="e1cb5-112">String</span></span>|<span data-ttu-id="e1cb5-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e1cb5-113">Display Name.</span></span> <span data-ttu-id="e1cb5-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1cb5-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e1cb5-115">description</span><span class="sxs-lookup"><span data-stu-id="e1cb5-115">description</span></span>|<span data-ttu-id="e1cb5-116">String</span><span class="sxs-lookup"><span data-stu-id="e1cb5-116">String</span></span>|<span data-ttu-id="e1cb5-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e1cb5-117">Description.</span></span> <span data-ttu-id="e1cb5-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1cb5-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e1cb5-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e1cb5-119">omaUri</span></span>|<span data-ttu-id="e1cb5-120">String</span><span class="sxs-lookup"><span data-stu-id="e1cb5-120">String</span></span>|<span data-ttu-id="e1cb5-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e1cb5-121">OMA.</span></span> <span data-ttu-id="e1cb5-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e1cb5-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e1cb5-123">value</span><span class="sxs-lookup"><span data-stu-id="e1cb5-123">value</span></span>|<span data-ttu-id="e1cb5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1cb5-124">DateTimeOffset</span></span>|<span data-ttu-id="e1cb5-125">值。</span><span class="sxs-lookup"><span data-stu-id="e1cb5-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1cb5-126">关系</span><span class="sxs-lookup"><span data-stu-id="e1cb5-126">Relationships</span></span>
<span data-ttu-id="e1cb5-127">无</span><span class="sxs-lookup"><span data-stu-id="e1cb5-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1cb5-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1cb5-128">JSON Representation</span></span>
<span data-ttu-id="e1cb5-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1cb5-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



