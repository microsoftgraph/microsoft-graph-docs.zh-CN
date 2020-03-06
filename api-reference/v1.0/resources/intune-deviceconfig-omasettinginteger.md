---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7e9e45e6153d565c4d56a4112e5e00cafed04f46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532415"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="ba2ed-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba2ed-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="ba2ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba2ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba2ed-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba2ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba2ed-106">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="ba2ed-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="ba2ed-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba2ed-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ba2ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba2ed-108">Properties</span></span>
|<span data-ttu-id="ba2ed-109">属性</span><span class="sxs-lookup"><span data-stu-id="ba2ed-109">Property</span></span>|<span data-ttu-id="ba2ed-110">类型</span><span class="sxs-lookup"><span data-stu-id="ba2ed-110">Type</span></span>|<span data-ttu-id="ba2ed-111">说明</span><span class="sxs-lookup"><span data-stu-id="ba2ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba2ed-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ba2ed-112">displayName</span></span>|<span data-ttu-id="ba2ed-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ba2ed-113">String</span></span>|<span data-ttu-id="ba2ed-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="ba2ed-114">Display Name.</span></span> <span data-ttu-id="ba2ed-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba2ed-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ba2ed-116">说明</span><span class="sxs-lookup"><span data-stu-id="ba2ed-116">description</span></span>|<span data-ttu-id="ba2ed-117">字符串</span><span class="sxs-lookup"><span data-stu-id="ba2ed-117">String</span></span>|<span data-ttu-id="ba2ed-118">说明。</span><span class="sxs-lookup"><span data-stu-id="ba2ed-118">Description.</span></span> <span data-ttu-id="ba2ed-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba2ed-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ba2ed-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="ba2ed-120">omaUri</span></span>|<span data-ttu-id="ba2ed-121">String</span><span class="sxs-lookup"><span data-stu-id="ba2ed-121">String</span></span>|<span data-ttu-id="ba2ed-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="ba2ed-122">OMA.</span></span> <span data-ttu-id="ba2ed-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="ba2ed-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ba2ed-124">值</span><span class="sxs-lookup"><span data-stu-id="ba2ed-124">value</span></span>|<span data-ttu-id="ba2ed-125">Int32</span><span class="sxs-lookup"><span data-stu-id="ba2ed-125">Int32</span></span>|<span data-ttu-id="ba2ed-126">值。</span><span class="sxs-lookup"><span data-stu-id="ba2ed-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba2ed-127">关系</span><span class="sxs-lookup"><span data-stu-id="ba2ed-127">Relationships</span></span>
<span data-ttu-id="ba2ed-128">无</span><span class="sxs-lookup"><span data-stu-id="ba2ed-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba2ed-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba2ed-129">JSON Representation</span></span>
<span data-ttu-id="ba2ed-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba2ed-130">Here is a JSON representation of the resource.</span></span>
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




