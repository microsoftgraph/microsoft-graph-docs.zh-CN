---
title: omaSettingString 资源类型
description: OMA 设置字符串定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d20a88e79a1383789a67883d03aae6b8e4463f4e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788434"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="d3624-103">omaSettingString 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3624-103">omaSettingString resource type</span></span>

> <span data-ttu-id="d3624-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3624-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3624-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3624-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3624-106">OMA 设置字符串定义。</span><span class="sxs-lookup"><span data-stu-id="d3624-106">OMA Settings String definition.</span></span>


<span data-ttu-id="d3624-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3624-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3624-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3624-108">Properties</span></span>
|<span data-ttu-id="d3624-109">属性</span><span class="sxs-lookup"><span data-stu-id="d3624-109">Property</span></span>|<span data-ttu-id="d3624-110">类型</span><span class="sxs-lookup"><span data-stu-id="d3624-110">Type</span></span>|<span data-ttu-id="d3624-111">说明</span><span class="sxs-lookup"><span data-stu-id="d3624-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3624-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d3624-112">displayName</span></span>|<span data-ttu-id="d3624-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d3624-113">String</span></span>|<span data-ttu-id="d3624-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="d3624-114">Display Name.</span></span> <span data-ttu-id="d3624-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3624-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3624-116">说明</span><span class="sxs-lookup"><span data-stu-id="d3624-116">description</span></span>|<span data-ttu-id="d3624-117">String</span><span class="sxs-lookup"><span data-stu-id="d3624-117">String</span></span>|<span data-ttu-id="d3624-118">说明。</span><span class="sxs-lookup"><span data-stu-id="d3624-118">Description.</span></span> <span data-ttu-id="d3624-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3624-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3624-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="d3624-120">omaUri</span></span>|<span data-ttu-id="d3624-121">String</span><span class="sxs-lookup"><span data-stu-id="d3624-121">String</span></span>|<span data-ttu-id="d3624-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="d3624-122">OMA.</span></span> <span data-ttu-id="d3624-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="d3624-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="d3624-124">value</span><span class="sxs-lookup"><span data-stu-id="d3624-124">value</span></span>|<span data-ttu-id="d3624-125">String</span><span class="sxs-lookup"><span data-stu-id="d3624-125">String</span></span>|<span data-ttu-id="d3624-126">值。</span><span class="sxs-lookup"><span data-stu-id="d3624-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3624-127">关系</span><span class="sxs-lookup"><span data-stu-id="d3624-127">Relationships</span></span>
<span data-ttu-id="d3624-128">无</span><span class="sxs-lookup"><span data-stu-id="d3624-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3624-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3624-129">JSON Representation</span></span>
<span data-ttu-id="d3624-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3624-130">Here is a JSON representation of the resource.</span></span>
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



