---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 43a7d32cc5ff6fedfd5edd5380a37afbd90e826d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722976"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="362ef-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="362ef-103">omaSettingBoolean resource type</span></span>

<span data-ttu-id="362ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="362ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="362ef-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="362ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="362ef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="362ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="362ef-107">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="362ef-107">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="362ef-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="362ef-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="362ef-109">属性</span><span class="sxs-lookup"><span data-stu-id="362ef-109">Properties</span></span>
|<span data-ttu-id="362ef-110">属性</span><span class="sxs-lookup"><span data-stu-id="362ef-110">Property</span></span>|<span data-ttu-id="362ef-111">类型</span><span class="sxs-lookup"><span data-stu-id="362ef-111">Type</span></span>|<span data-ttu-id="362ef-112">说明</span><span class="sxs-lookup"><span data-stu-id="362ef-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="362ef-113">displayName</span><span class="sxs-lookup"><span data-stu-id="362ef-113">displayName</span></span>|<span data-ttu-id="362ef-114">String</span><span class="sxs-lookup"><span data-stu-id="362ef-114">String</span></span>|<span data-ttu-id="362ef-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="362ef-115">Display Name.</span></span> <span data-ttu-id="362ef-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="362ef-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="362ef-117">说明</span><span class="sxs-lookup"><span data-stu-id="362ef-117">description</span></span>|<span data-ttu-id="362ef-118">String</span><span class="sxs-lookup"><span data-stu-id="362ef-118">String</span></span>|<span data-ttu-id="362ef-119">说明。</span><span class="sxs-lookup"><span data-stu-id="362ef-119">Description.</span></span> <span data-ttu-id="362ef-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="362ef-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="362ef-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="362ef-121">omaUri</span></span>|<span data-ttu-id="362ef-122">String</span><span class="sxs-lookup"><span data-stu-id="362ef-122">String</span></span>|<span data-ttu-id="362ef-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="362ef-123">OMA.</span></span> <span data-ttu-id="362ef-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="362ef-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="362ef-125">value</span><span class="sxs-lookup"><span data-stu-id="362ef-125">value</span></span>|<span data-ttu-id="362ef-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="362ef-126">Boolean</span></span>|<span data-ttu-id="362ef-127">值。</span><span class="sxs-lookup"><span data-stu-id="362ef-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="362ef-128">关系</span><span class="sxs-lookup"><span data-stu-id="362ef-128">Relationships</span></span>
<span data-ttu-id="362ef-129">无</span><span class="sxs-lookup"><span data-stu-id="362ef-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="362ef-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="362ef-130">JSON Representation</span></span>
<span data-ttu-id="362ef-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="362ef-131">Here is a JSON representation of the resource.</span></span>
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





