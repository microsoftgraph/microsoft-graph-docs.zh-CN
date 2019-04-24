---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20bc82e88480dca1df727e299e62c4274002176f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585396"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="9cbe1-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="9cbe1-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="9cbe1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9cbe1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cbe1-105">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="9cbe1-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="9cbe1-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9cbe1-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9cbe1-107">属性</span><span class="sxs-lookup"><span data-stu-id="9cbe1-107">Properties</span></span>
|<span data-ttu-id="9cbe1-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cbe1-108">Property</span></span>|<span data-ttu-id="9cbe1-109">类型</span><span class="sxs-lookup"><span data-stu-id="9cbe1-109">Type</span></span>|<span data-ttu-id="9cbe1-110">说明</span><span class="sxs-lookup"><span data-stu-id="9cbe1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cbe1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9cbe1-111">displayName</span></span>|<span data-ttu-id="9cbe1-112">字符串</span><span class="sxs-lookup"><span data-stu-id="9cbe1-112">String</span></span>|<span data-ttu-id="9cbe1-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="9cbe1-113">Display Name.</span></span> <span data-ttu-id="9cbe1-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9cbe1-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9cbe1-115">description</span><span class="sxs-lookup"><span data-stu-id="9cbe1-115">description</span></span>|<span data-ttu-id="9cbe1-116">字符串</span><span class="sxs-lookup"><span data-stu-id="9cbe1-116">String</span></span>|<span data-ttu-id="9cbe1-117">说明。</span><span class="sxs-lookup"><span data-stu-id="9cbe1-117">Description.</span></span> <span data-ttu-id="9cbe1-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9cbe1-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9cbe1-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="9cbe1-119">omaUri</span></span>|<span data-ttu-id="9cbe1-120">String</span><span class="sxs-lookup"><span data-stu-id="9cbe1-120">String</span></span>|<span data-ttu-id="9cbe1-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="9cbe1-121">OMA.</span></span> <span data-ttu-id="9cbe1-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="9cbe1-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9cbe1-123">value</span><span class="sxs-lookup"><span data-stu-id="9cbe1-123">value</span></span>|<span data-ttu-id="9cbe1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9cbe1-124">DateTimeOffset</span></span>|<span data-ttu-id="9cbe1-125">值。</span><span class="sxs-lookup"><span data-stu-id="9cbe1-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cbe1-126">关系</span><span class="sxs-lookup"><span data-stu-id="9cbe1-126">Relationships</span></span>
<span data-ttu-id="9cbe1-127">无</span><span class="sxs-lookup"><span data-stu-id="9cbe1-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9cbe1-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9cbe1-128">JSON Representation</span></span>
<span data-ttu-id="9cbe1-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9cbe1-129">Here is a JSON representation of the resource.</span></span>
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



