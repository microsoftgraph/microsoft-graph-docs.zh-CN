---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9df0179b32d6bf60a25ef349b5e4c201a9420a10
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755866"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="a10ba-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="a10ba-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="a10ba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a10ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a10ba-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a10ba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a10ba-106">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="a10ba-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="a10ba-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a10ba-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a10ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="a10ba-108">Properties</span></span>
|<span data-ttu-id="a10ba-109">属性</span><span class="sxs-lookup"><span data-stu-id="a10ba-109">Property</span></span>|<span data-ttu-id="a10ba-110">类型</span><span class="sxs-lookup"><span data-stu-id="a10ba-110">Type</span></span>|<span data-ttu-id="a10ba-111">说明</span><span class="sxs-lookup"><span data-stu-id="a10ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a10ba-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a10ba-112">displayName</span></span>|<span data-ttu-id="a10ba-113">String</span><span class="sxs-lookup"><span data-stu-id="a10ba-113">String</span></span>|<span data-ttu-id="a10ba-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="a10ba-114">Display Name.</span></span> <span data-ttu-id="a10ba-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a10ba-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a10ba-116">说明</span><span class="sxs-lookup"><span data-stu-id="a10ba-116">description</span></span>|<span data-ttu-id="a10ba-117">String</span><span class="sxs-lookup"><span data-stu-id="a10ba-117">String</span></span>|<span data-ttu-id="a10ba-118">说明。</span><span class="sxs-lookup"><span data-stu-id="a10ba-118">Description.</span></span> <span data-ttu-id="a10ba-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a10ba-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a10ba-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="a10ba-120">omaUri</span></span>|<span data-ttu-id="a10ba-121">String</span><span class="sxs-lookup"><span data-stu-id="a10ba-121">String</span></span>|<span data-ttu-id="a10ba-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="a10ba-122">OMA.</span></span> <span data-ttu-id="a10ba-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="a10ba-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="a10ba-124">值</span><span class="sxs-lookup"><span data-stu-id="a10ba-124">value</span></span>|<span data-ttu-id="a10ba-125">Int32</span><span class="sxs-lookup"><span data-stu-id="a10ba-125">Int32</span></span>|<span data-ttu-id="a10ba-126">值。</span><span class="sxs-lookup"><span data-stu-id="a10ba-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a10ba-127">关系</span><span class="sxs-lookup"><span data-stu-id="a10ba-127">Relationships</span></span>
<span data-ttu-id="a10ba-128">无</span><span class="sxs-lookup"><span data-stu-id="a10ba-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a10ba-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a10ba-129">JSON Representation</span></span>
<span data-ttu-id="a10ba-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a10ba-130">Here is a JSON representation of the resource.</span></span>
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




