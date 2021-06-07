---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99fa5ccf0b26ebd04ce232eb8bf4df9a9d4ace81
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755880"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="d930e-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="d930e-103">omaSettingDateTime resource type</span></span>

<span data-ttu-id="d930e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d930e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d930e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d930e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d930e-106">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="d930e-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="d930e-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d930e-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d930e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d930e-108">Properties</span></span>
|<span data-ttu-id="d930e-109">属性</span><span class="sxs-lookup"><span data-stu-id="d930e-109">Property</span></span>|<span data-ttu-id="d930e-110">类型</span><span class="sxs-lookup"><span data-stu-id="d930e-110">Type</span></span>|<span data-ttu-id="d930e-111">说明</span><span class="sxs-lookup"><span data-stu-id="d930e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d930e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d930e-112">displayName</span></span>|<span data-ttu-id="d930e-113">String</span><span class="sxs-lookup"><span data-stu-id="d930e-113">String</span></span>|<span data-ttu-id="d930e-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="d930e-114">Display Name.</span></span> <span data-ttu-id="d930e-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d930e-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d930e-116">说明</span><span class="sxs-lookup"><span data-stu-id="d930e-116">description</span></span>|<span data-ttu-id="d930e-117">String</span><span class="sxs-lookup"><span data-stu-id="d930e-117">String</span></span>|<span data-ttu-id="d930e-118">说明。</span><span class="sxs-lookup"><span data-stu-id="d930e-118">Description.</span></span> <span data-ttu-id="d930e-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d930e-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d930e-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d930e-120">omaUri</span></span>|<span data-ttu-id="d930e-121">String</span><span class="sxs-lookup"><span data-stu-id="d930e-121">String</span></span>|<span data-ttu-id="d930e-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="d930e-122">OMA.</span></span> <span data-ttu-id="d930e-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d930e-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d930e-124">value</span><span class="sxs-lookup"><span data-stu-id="d930e-124">value</span></span>|<span data-ttu-id="d930e-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d930e-125">DateTimeOffset</span></span>|<span data-ttu-id="d930e-126">值。</span><span class="sxs-lookup"><span data-stu-id="d930e-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d930e-127">关系</span><span class="sxs-lookup"><span data-stu-id="d930e-127">Relationships</span></span>
<span data-ttu-id="d930e-128">无</span><span class="sxs-lookup"><span data-stu-id="d930e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d930e-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d930e-129">JSON Representation</span></span>
<span data-ttu-id="d930e-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d930e-130">Here is a JSON representation of the resource.</span></span>
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




