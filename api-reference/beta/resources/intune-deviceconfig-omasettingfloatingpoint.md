---
title: omaSettingFloatingPoint 资源类型
description: OMA 设置浮点定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e62fc6f4a1f8df657195551f42f83e22168c73b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969931"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="f7912-103">omaSettingFloatingPoint 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7912-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="f7912-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7912-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7912-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7912-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7912-106">OMA 设置浮点定义。</span><span class="sxs-lookup"><span data-stu-id="f7912-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="f7912-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f7912-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f7912-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7912-108">Properties</span></span>
|<span data-ttu-id="f7912-109">属性</span><span class="sxs-lookup"><span data-stu-id="f7912-109">Property</span></span>|<span data-ttu-id="f7912-110">类型</span><span class="sxs-lookup"><span data-stu-id="f7912-110">Type</span></span>|<span data-ttu-id="f7912-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7912-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7912-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f7912-112">displayName</span></span>|<span data-ttu-id="f7912-113">字符串</span><span class="sxs-lookup"><span data-stu-id="f7912-113">String</span></span>|<span data-ttu-id="f7912-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f7912-114">Display Name.</span></span> <span data-ttu-id="f7912-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f7912-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f7912-116">说明</span><span class="sxs-lookup"><span data-stu-id="f7912-116">description</span></span>|<span data-ttu-id="f7912-117">String</span><span class="sxs-lookup"><span data-stu-id="f7912-117">String</span></span>|<span data-ttu-id="f7912-118">说明。</span><span class="sxs-lookup"><span data-stu-id="f7912-118">Description.</span></span> <span data-ttu-id="f7912-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f7912-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f7912-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="f7912-120">omaUri</span></span>|<span data-ttu-id="f7912-121">String</span><span class="sxs-lookup"><span data-stu-id="f7912-121">String</span></span>|<span data-ttu-id="f7912-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="f7912-122">OMA.</span></span> <span data-ttu-id="f7912-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f7912-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f7912-124">value</span><span class="sxs-lookup"><span data-stu-id="f7912-124">value</span></span>|<span data-ttu-id="f7912-125">单个</span><span class="sxs-lookup"><span data-stu-id="f7912-125">Single</span></span>|<span data-ttu-id="f7912-126">值。</span><span class="sxs-lookup"><span data-stu-id="f7912-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7912-127">关系</span><span class="sxs-lookup"><span data-stu-id="f7912-127">Relationships</span></span>
<span data-ttu-id="f7912-128">无</span><span class="sxs-lookup"><span data-stu-id="f7912-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7912-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7912-129">JSON Representation</span></span>
<span data-ttu-id="f7912-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7912-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```





