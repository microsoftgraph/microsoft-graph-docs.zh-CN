---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 30802cc391958fabec4540fc3256f7c67ec094c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031302"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="e752c-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="e752c-103">omaSettingString resource type</span></span>

> <span data-ttu-id="e752c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e752c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e752c-105">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="e752c-105">OMA Settings String definition.</span></span>


<span data-ttu-id="e752c-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e752c-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e752c-107">属性</span><span class="sxs-lookup"><span data-stu-id="e752c-107">Properties</span></span>
|<span data-ttu-id="e752c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e752c-108">Property</span></span>|<span data-ttu-id="e752c-109">类型</span><span class="sxs-lookup"><span data-stu-id="e752c-109">Type</span></span>|<span data-ttu-id="e752c-110">说明</span><span class="sxs-lookup"><span data-stu-id="e752c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e752c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e752c-111">displayName</span></span>|<span data-ttu-id="e752c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e752c-112">String</span></span>|<span data-ttu-id="e752c-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e752c-113">Display Name.</span></span> <span data-ttu-id="e752c-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e752c-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e752c-115">说明</span><span class="sxs-lookup"><span data-stu-id="e752c-115">description</span></span>|<span data-ttu-id="e752c-116">String</span><span class="sxs-lookup"><span data-stu-id="e752c-116">String</span></span>|<span data-ttu-id="e752c-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e752c-117">Description.</span></span> <span data-ttu-id="e752c-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e752c-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e752c-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e752c-119">omaUri</span></span>|<span data-ttu-id="e752c-120">String</span><span class="sxs-lookup"><span data-stu-id="e752c-120">String</span></span>|<span data-ttu-id="e752c-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e752c-121">OMA.</span></span> <span data-ttu-id="e752c-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e752c-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e752c-123">value</span><span class="sxs-lookup"><span data-stu-id="e752c-123">value</span></span>|<span data-ttu-id="e752c-124">String</span><span class="sxs-lookup"><span data-stu-id="e752c-124">String</span></span>|<span data-ttu-id="e752c-125">值。</span><span class="sxs-lookup"><span data-stu-id="e752c-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e752c-126">关系</span><span class="sxs-lookup"><span data-stu-id="e752c-126">Relationships</span></span>
<span data-ttu-id="e752c-127">无</span><span class="sxs-lookup"><span data-stu-id="e752c-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e752c-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e752c-128">JSON Representation</span></span>
<span data-ttu-id="e752c-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e752c-129">Here is a JSON representation of the resource.</span></span>
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



