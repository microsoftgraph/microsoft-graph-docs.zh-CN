---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71347ecd4a566409d1043c788df70601ffc70a2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028026"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="e668f-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="e668f-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="e668f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e668f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e668f-105">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="e668f-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="e668f-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e668f-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e668f-107">属性</span><span class="sxs-lookup"><span data-stu-id="e668f-107">Properties</span></span>
|<span data-ttu-id="e668f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e668f-108">Property</span></span>|<span data-ttu-id="e668f-109">类型</span><span class="sxs-lookup"><span data-stu-id="e668f-109">Type</span></span>|<span data-ttu-id="e668f-110">说明</span><span class="sxs-lookup"><span data-stu-id="e668f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e668f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e668f-111">displayName</span></span>|<span data-ttu-id="e668f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="e668f-112">String</span></span>|<span data-ttu-id="e668f-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e668f-113">Display Name.</span></span> <span data-ttu-id="e668f-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e668f-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e668f-115">说明</span><span class="sxs-lookup"><span data-stu-id="e668f-115">description</span></span>|<span data-ttu-id="e668f-116">String</span><span class="sxs-lookup"><span data-stu-id="e668f-116">String</span></span>|<span data-ttu-id="e668f-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e668f-117">Description.</span></span> <span data-ttu-id="e668f-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e668f-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e668f-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e668f-119">omaUri</span></span>|<span data-ttu-id="e668f-120">String</span><span class="sxs-lookup"><span data-stu-id="e668f-120">String</span></span>|<span data-ttu-id="e668f-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e668f-121">OMA.</span></span> <span data-ttu-id="e668f-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e668f-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e668f-123">value</span><span class="sxs-lookup"><span data-stu-id="e668f-123">value</span></span>|<span data-ttu-id="e668f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e668f-124">DateTimeOffset</span></span>|<span data-ttu-id="e668f-125">值。</span><span class="sxs-lookup"><span data-stu-id="e668f-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e668f-126">关系</span><span class="sxs-lookup"><span data-stu-id="e668f-126">Relationships</span></span>
<span data-ttu-id="e668f-127">无</span><span class="sxs-lookup"><span data-stu-id="e668f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e668f-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e668f-128">JSON Representation</span></span>
<span data-ttu-id="e668f-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e668f-129">Here is a JSON representation of the resource.</span></span>
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



