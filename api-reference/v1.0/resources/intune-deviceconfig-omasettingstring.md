---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a647b532704af6892af7d65714d47ad16eb00eaf
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755859"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="0af62-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="0af62-103">omaSettingString resource type</span></span>

<span data-ttu-id="0af62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0af62-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0af62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0af62-106">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="0af62-106">OMA Settings String definition.</span></span>


<span data-ttu-id="0af62-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0af62-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0af62-108">属性</span><span class="sxs-lookup"><span data-stu-id="0af62-108">Properties</span></span>
|<span data-ttu-id="0af62-109">属性</span><span class="sxs-lookup"><span data-stu-id="0af62-109">Property</span></span>|<span data-ttu-id="0af62-110">类型</span><span class="sxs-lookup"><span data-stu-id="0af62-110">Type</span></span>|<span data-ttu-id="0af62-111">说明</span><span class="sxs-lookup"><span data-stu-id="0af62-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0af62-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0af62-112">displayName</span></span>|<span data-ttu-id="0af62-113">String</span><span class="sxs-lookup"><span data-stu-id="0af62-113">String</span></span>|<span data-ttu-id="0af62-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="0af62-114">Display Name.</span></span> <span data-ttu-id="0af62-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0af62-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0af62-116">说明</span><span class="sxs-lookup"><span data-stu-id="0af62-116">description</span></span>|<span data-ttu-id="0af62-117">String</span><span class="sxs-lookup"><span data-stu-id="0af62-117">String</span></span>|<span data-ttu-id="0af62-118">说明。</span><span class="sxs-lookup"><span data-stu-id="0af62-118">Description.</span></span> <span data-ttu-id="0af62-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0af62-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0af62-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="0af62-120">omaUri</span></span>|<span data-ttu-id="0af62-121">String</span><span class="sxs-lookup"><span data-stu-id="0af62-121">String</span></span>|<span data-ttu-id="0af62-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="0af62-122">OMA.</span></span> <span data-ttu-id="0af62-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="0af62-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="0af62-124">value</span><span class="sxs-lookup"><span data-stu-id="0af62-124">value</span></span>|<span data-ttu-id="0af62-125">String</span><span class="sxs-lookup"><span data-stu-id="0af62-125">String</span></span>|<span data-ttu-id="0af62-126">值。</span><span class="sxs-lookup"><span data-stu-id="0af62-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0af62-127">关系</span><span class="sxs-lookup"><span data-stu-id="0af62-127">Relationships</span></span>
<span data-ttu-id="0af62-128">无</span><span class="sxs-lookup"><span data-stu-id="0af62-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0af62-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0af62-129">JSON Representation</span></span>
<span data-ttu-id="0af62-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0af62-130">Here is a JSON representation of the resource.</span></span>
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




