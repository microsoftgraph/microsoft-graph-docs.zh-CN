---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a22c69270126349d8d1d4afca4555abd18768aa3
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803029"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="5b002-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b002-103">omaSettingString resource type</span></span>

> <span data-ttu-id="5b002-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5b002-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b002-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b002-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b002-106">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="5b002-106">OMA Settings String definition.</span></span>


<span data-ttu-id="5b002-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5b002-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b002-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b002-108">Properties</span></span>
|<span data-ttu-id="5b002-109">属性</span><span class="sxs-lookup"><span data-stu-id="5b002-109">Property</span></span>|<span data-ttu-id="5b002-110">类型</span><span class="sxs-lookup"><span data-stu-id="5b002-110">Type</span></span>|<span data-ttu-id="5b002-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b002-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b002-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5b002-112">displayName</span></span>|<span data-ttu-id="5b002-113">字符串</span><span class="sxs-lookup"><span data-stu-id="5b002-113">String</span></span>|<span data-ttu-id="5b002-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="5b002-114">Display Name.</span></span> <span data-ttu-id="5b002-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5b002-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5b002-116">description</span><span class="sxs-lookup"><span data-stu-id="5b002-116">description</span></span>|<span data-ttu-id="5b002-117">String</span><span class="sxs-lookup"><span data-stu-id="5b002-117">String</span></span>|<span data-ttu-id="5b002-118">说明。</span><span class="sxs-lookup"><span data-stu-id="5b002-118">Description.</span></span> <span data-ttu-id="5b002-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5b002-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5b002-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="5b002-120">omaUri</span></span>|<span data-ttu-id="5b002-121">String</span><span class="sxs-lookup"><span data-stu-id="5b002-121">String</span></span>|<span data-ttu-id="5b002-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="5b002-122">OMA.</span></span> <span data-ttu-id="5b002-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="5b002-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="5b002-124">value</span><span class="sxs-lookup"><span data-stu-id="5b002-124">value</span></span>|<span data-ttu-id="5b002-125">String</span><span class="sxs-lookup"><span data-stu-id="5b002-125">String</span></span>|<span data-ttu-id="5b002-126">值。</span><span class="sxs-lookup"><span data-stu-id="5b002-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b002-127">关系</span><span class="sxs-lookup"><span data-stu-id="5b002-127">Relationships</span></span>
<span data-ttu-id="5b002-128">无</span><span class="sxs-lookup"><span data-stu-id="5b002-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b002-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b002-129">JSON Representation</span></span>
<span data-ttu-id="5b002-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b002-130">Here is a JSON representation of the resource.</span></span>
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





