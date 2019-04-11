---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 54eec27cf91bb1da7790ae1432452ac026bf1683
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781923"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="111e3-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="111e3-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="111e3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="111e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="111e3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="111e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="111e3-106">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="111e3-106">OMA Settings Integer definition.</span></span>


<span data-ttu-id="111e3-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="111e3-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="111e3-108">属性</span><span class="sxs-lookup"><span data-stu-id="111e3-108">Properties</span></span>
|<span data-ttu-id="111e3-109">属性</span><span class="sxs-lookup"><span data-stu-id="111e3-109">Property</span></span>|<span data-ttu-id="111e3-110">类型</span><span class="sxs-lookup"><span data-stu-id="111e3-110">Type</span></span>|<span data-ttu-id="111e3-111">说明</span><span class="sxs-lookup"><span data-stu-id="111e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="111e3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="111e3-112">displayName</span></span>|<span data-ttu-id="111e3-113">字符串</span><span class="sxs-lookup"><span data-stu-id="111e3-113">String</span></span>|<span data-ttu-id="111e3-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="111e3-114">Display Name.</span></span> <span data-ttu-id="111e3-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="111e3-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="111e3-116">description</span><span class="sxs-lookup"><span data-stu-id="111e3-116">description</span></span>|<span data-ttu-id="111e3-117">String</span><span class="sxs-lookup"><span data-stu-id="111e3-117">String</span></span>|<span data-ttu-id="111e3-118">说明。</span><span class="sxs-lookup"><span data-stu-id="111e3-118">Description.</span></span> <span data-ttu-id="111e3-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="111e3-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="111e3-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="111e3-120">omaUri</span></span>|<span data-ttu-id="111e3-121">String</span><span class="sxs-lookup"><span data-stu-id="111e3-121">String</span></span>|<span data-ttu-id="111e3-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="111e3-122">OMA.</span></span> <span data-ttu-id="111e3-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="111e3-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="111e3-124">值</span><span class="sxs-lookup"><span data-stu-id="111e3-124">value</span></span>|<span data-ttu-id="111e3-125">Int32</span><span class="sxs-lookup"><span data-stu-id="111e3-125">Int32</span></span>|<span data-ttu-id="111e3-126">值。</span><span class="sxs-lookup"><span data-stu-id="111e3-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="111e3-127">关系</span><span class="sxs-lookup"><span data-stu-id="111e3-127">Relationships</span></span>
<span data-ttu-id="111e3-128">无</span><span class="sxs-lookup"><span data-stu-id="111e3-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="111e3-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="111e3-129">JSON Representation</span></span>
<span data-ttu-id="111e3-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="111e3-130">Here is a JSON representation of the resource.</span></span>
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





