---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97ac2092573639db5d46386fe9475df26b136e80
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368497"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="2ac97-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ac97-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="2ac97-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ac97-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ac97-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ac97-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac97-106">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="2ac97-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="2ac97-107">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ac97-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2ac97-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ac97-108">Properties</span></span>
|<span data-ttu-id="2ac97-109">属性</span><span class="sxs-lookup"><span data-stu-id="2ac97-109">Property</span></span>|<span data-ttu-id="2ac97-110">类型</span><span class="sxs-lookup"><span data-stu-id="2ac97-110">Type</span></span>|<span data-ttu-id="2ac97-111">说明</span><span class="sxs-lookup"><span data-stu-id="2ac97-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac97-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2ac97-112">displayName</span></span>|<span data-ttu-id="2ac97-113">字符串</span><span class="sxs-lookup"><span data-stu-id="2ac97-113">String</span></span>|<span data-ttu-id="2ac97-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="2ac97-114">Display Name.</span></span> <span data-ttu-id="2ac97-115">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ac97-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2ac97-116">说明</span><span class="sxs-lookup"><span data-stu-id="2ac97-116">description</span></span>|<span data-ttu-id="2ac97-117">String</span><span class="sxs-lookup"><span data-stu-id="2ac97-117">String</span></span>|<span data-ttu-id="2ac97-118">说明。</span><span class="sxs-lookup"><span data-stu-id="2ac97-118">Description.</span></span> <span data-ttu-id="2ac97-119">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ac97-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2ac97-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="2ac97-120">omaUri</span></span>|<span data-ttu-id="2ac97-121">String</span><span class="sxs-lookup"><span data-stu-id="2ac97-121">String</span></span>|<span data-ttu-id="2ac97-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="2ac97-122">OMA.</span></span> <span data-ttu-id="2ac97-123">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="2ac97-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2ac97-124">value</span><span class="sxs-lookup"><span data-stu-id="2ac97-124">value</span></span>|<span data-ttu-id="2ac97-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac97-125">DateTimeOffset</span></span>|<span data-ttu-id="2ac97-126">值。</span><span class="sxs-lookup"><span data-stu-id="2ac97-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ac97-127">关系</span><span class="sxs-lookup"><span data-stu-id="2ac97-127">Relationships</span></span>
<span data-ttu-id="2ac97-128">无</span><span class="sxs-lookup"><span data-stu-id="2ac97-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ac97-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ac97-129">JSON Representation</span></span>
<span data-ttu-id="2ac97-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ac97-130">Here is a JSON representation of the resource.</span></span>
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



