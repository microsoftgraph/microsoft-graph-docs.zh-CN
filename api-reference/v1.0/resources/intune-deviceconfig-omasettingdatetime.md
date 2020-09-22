---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6291fc5b81de9dea1bfa67515f4df296d9e3001e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978151"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="b4be6-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4be6-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="b4be6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4be6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4be6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4be6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4be6-106">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="b4be6-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="b4be6-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b4be6-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4be6-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4be6-108">Properties</span></span>
|<span data-ttu-id="b4be6-109">属性</span><span class="sxs-lookup"><span data-stu-id="b4be6-109">Property</span></span>|<span data-ttu-id="b4be6-110">类型</span><span class="sxs-lookup"><span data-stu-id="b4be6-110">Type</span></span>|<span data-ttu-id="b4be6-111">说明</span><span class="sxs-lookup"><span data-stu-id="b4be6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4be6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b4be6-112">displayName</span></span>|<span data-ttu-id="b4be6-113">String</span><span class="sxs-lookup"><span data-stu-id="b4be6-113">String</span></span>|<span data-ttu-id="b4be6-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b4be6-114">Display Name.</span></span> <span data-ttu-id="b4be6-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b4be6-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b4be6-116">description</span><span class="sxs-lookup"><span data-stu-id="b4be6-116">description</span></span>|<span data-ttu-id="b4be6-117">String</span><span class="sxs-lookup"><span data-stu-id="b4be6-117">String</span></span>|<span data-ttu-id="b4be6-118">说明。</span><span class="sxs-lookup"><span data-stu-id="b4be6-118">Description.</span></span> <span data-ttu-id="b4be6-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b4be6-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b4be6-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="b4be6-120">omaUri</span></span>|<span data-ttu-id="b4be6-121">String</span><span class="sxs-lookup"><span data-stu-id="b4be6-121">String</span></span>|<span data-ttu-id="b4be6-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="b4be6-122">OMA.</span></span> <span data-ttu-id="b4be6-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="b4be6-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="b4be6-124">value</span><span class="sxs-lookup"><span data-stu-id="b4be6-124">value</span></span>|<span data-ttu-id="b4be6-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b4be6-125">DateTimeOffset</span></span>|<span data-ttu-id="b4be6-126">值。</span><span class="sxs-lookup"><span data-stu-id="b4be6-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4be6-127">关系</span><span class="sxs-lookup"><span data-stu-id="b4be6-127">Relationships</span></span>
<span data-ttu-id="b4be6-128">无</span><span class="sxs-lookup"><span data-stu-id="b4be6-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4be6-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4be6-129">JSON Representation</span></span>
<span data-ttu-id="b4be6-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4be6-130">Here is a JSON representation of the resource.</span></span>
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









