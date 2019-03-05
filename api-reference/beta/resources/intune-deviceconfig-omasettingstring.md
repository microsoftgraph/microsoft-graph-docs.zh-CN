---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ba2da95a8a60ef0cf6d2ba03b024c5200e0c5a8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162046"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="47802-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="47802-103">omaSettingString resource type</span></span>

> <span data-ttu-id="47802-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47802-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47802-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47802-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47802-106">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="47802-106">OMA Settings String definition.</span></span>


<span data-ttu-id="47802-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47802-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47802-108">属性</span><span class="sxs-lookup"><span data-stu-id="47802-108">Properties</span></span>
|<span data-ttu-id="47802-109">属性</span><span class="sxs-lookup"><span data-stu-id="47802-109">Property</span></span>|<span data-ttu-id="47802-110">类型</span><span class="sxs-lookup"><span data-stu-id="47802-110">Type</span></span>|<span data-ttu-id="47802-111">说明</span><span class="sxs-lookup"><span data-stu-id="47802-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47802-112">displayName</span><span class="sxs-lookup"><span data-stu-id="47802-112">displayName</span></span>|<span data-ttu-id="47802-113">String</span><span class="sxs-lookup"><span data-stu-id="47802-113">String</span></span>|<span data-ttu-id="47802-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="47802-114">Display Name.</span></span> <span data-ttu-id="47802-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47802-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47802-116">description</span><span class="sxs-lookup"><span data-stu-id="47802-116">description</span></span>|<span data-ttu-id="47802-117">String</span><span class="sxs-lookup"><span data-stu-id="47802-117">String</span></span>|<span data-ttu-id="47802-118">说明。</span><span class="sxs-lookup"><span data-stu-id="47802-118">Description.</span></span> <span data-ttu-id="47802-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47802-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47802-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="47802-120">omaUri</span></span>|<span data-ttu-id="47802-121">String</span><span class="sxs-lookup"><span data-stu-id="47802-121">String</span></span>|<span data-ttu-id="47802-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="47802-122">OMA.</span></span> <span data-ttu-id="47802-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="47802-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="47802-124">值</span><span class="sxs-lookup"><span data-stu-id="47802-124">value</span></span>|<span data-ttu-id="47802-125">String</span><span class="sxs-lookup"><span data-stu-id="47802-125">String</span></span>|<span data-ttu-id="47802-126">值。</span><span class="sxs-lookup"><span data-stu-id="47802-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47802-127">关系</span><span class="sxs-lookup"><span data-stu-id="47802-127">Relationships</span></span>
<span data-ttu-id="47802-128">无</span><span class="sxs-lookup"><span data-stu-id="47802-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47802-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47802-129">JSON Representation</span></span>
<span data-ttu-id="47802-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47802-130">Here is a JSON representation of the resource.</span></span>
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




