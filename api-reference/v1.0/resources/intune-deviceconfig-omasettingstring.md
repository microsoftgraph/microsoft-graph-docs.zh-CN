---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 05f37b94aecadd5e3da1d0e162cd8bf6afe96681
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988266"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="73a18-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="73a18-103">omaSettingString resource type</span></span>

<span data-ttu-id="73a18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73a18-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73a18-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73a18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73a18-106">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="73a18-106">OMA Settings String definition.</span></span>


<span data-ttu-id="73a18-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="73a18-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="73a18-108">属性</span><span class="sxs-lookup"><span data-stu-id="73a18-108">Properties</span></span>
|<span data-ttu-id="73a18-109">属性</span><span class="sxs-lookup"><span data-stu-id="73a18-109">Property</span></span>|<span data-ttu-id="73a18-110">类型</span><span class="sxs-lookup"><span data-stu-id="73a18-110">Type</span></span>|<span data-ttu-id="73a18-111">说明</span><span class="sxs-lookup"><span data-stu-id="73a18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73a18-112">displayName</span><span class="sxs-lookup"><span data-stu-id="73a18-112">displayName</span></span>|<span data-ttu-id="73a18-113">String</span><span class="sxs-lookup"><span data-stu-id="73a18-113">String</span></span>|<span data-ttu-id="73a18-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="73a18-114">Display Name.</span></span> <span data-ttu-id="73a18-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="73a18-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="73a18-116">description</span><span class="sxs-lookup"><span data-stu-id="73a18-116">description</span></span>|<span data-ttu-id="73a18-117">String</span><span class="sxs-lookup"><span data-stu-id="73a18-117">String</span></span>|<span data-ttu-id="73a18-118">说明。</span><span class="sxs-lookup"><span data-stu-id="73a18-118">Description.</span></span> <span data-ttu-id="73a18-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="73a18-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="73a18-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="73a18-120">omaUri</span></span>|<span data-ttu-id="73a18-121">String</span><span class="sxs-lookup"><span data-stu-id="73a18-121">String</span></span>|<span data-ttu-id="73a18-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="73a18-122">OMA.</span></span> <span data-ttu-id="73a18-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="73a18-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="73a18-124">value</span><span class="sxs-lookup"><span data-stu-id="73a18-124">value</span></span>|<span data-ttu-id="73a18-125">String</span><span class="sxs-lookup"><span data-stu-id="73a18-125">String</span></span>|<span data-ttu-id="73a18-126">值。</span><span class="sxs-lookup"><span data-stu-id="73a18-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73a18-127">关系</span><span class="sxs-lookup"><span data-stu-id="73a18-127">Relationships</span></span>
<span data-ttu-id="73a18-128">无</span><span class="sxs-lookup"><span data-stu-id="73a18-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73a18-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73a18-129">JSON Representation</span></span>
<span data-ttu-id="73a18-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73a18-130">Here is a JSON representation of the resource.</span></span>
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









