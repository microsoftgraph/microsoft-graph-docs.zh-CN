---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d4ade59cc6359f4cc9f5bd668882860cf49ff49
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788455"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="95628-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="95628-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="95628-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95628-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95628-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95628-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95628-106">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="95628-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="95628-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95628-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="95628-108">属性</span><span class="sxs-lookup"><span data-stu-id="95628-108">Properties</span></span>
|<span data-ttu-id="95628-109">属性</span><span class="sxs-lookup"><span data-stu-id="95628-109">Property</span></span>|<span data-ttu-id="95628-110">类型</span><span class="sxs-lookup"><span data-stu-id="95628-110">Type</span></span>|<span data-ttu-id="95628-111">说明</span><span class="sxs-lookup"><span data-stu-id="95628-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95628-112">displayName</span><span class="sxs-lookup"><span data-stu-id="95628-112">displayName</span></span>|<span data-ttu-id="95628-113">字符串</span><span class="sxs-lookup"><span data-stu-id="95628-113">String</span></span>|<span data-ttu-id="95628-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="95628-114">Display Name.</span></span> <span data-ttu-id="95628-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95628-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95628-116">说明</span><span class="sxs-lookup"><span data-stu-id="95628-116">description</span></span>|<span data-ttu-id="95628-117">String</span><span class="sxs-lookup"><span data-stu-id="95628-117">String</span></span>|<span data-ttu-id="95628-118">说明。</span><span class="sxs-lookup"><span data-stu-id="95628-118">Description.</span></span> <span data-ttu-id="95628-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95628-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95628-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="95628-120">omaUri</span></span>|<span data-ttu-id="95628-121">String</span><span class="sxs-lookup"><span data-stu-id="95628-121">String</span></span>|<span data-ttu-id="95628-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="95628-122">OMA.</span></span> <span data-ttu-id="95628-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="95628-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="95628-124">value</span><span class="sxs-lookup"><span data-stu-id="95628-124">value</span></span>|<span data-ttu-id="95628-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95628-125">DateTimeOffset</span></span>|<span data-ttu-id="95628-126">值。</span><span class="sxs-lookup"><span data-stu-id="95628-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95628-127">关系</span><span class="sxs-lookup"><span data-stu-id="95628-127">Relationships</span></span>
<span data-ttu-id="95628-128">无</span><span class="sxs-lookup"><span data-stu-id="95628-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95628-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95628-129">JSON Representation</span></span>
<span data-ttu-id="95628-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95628-130">Here is a JSON representation of the resource.</span></span>
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



