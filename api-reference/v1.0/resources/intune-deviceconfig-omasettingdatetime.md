---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: tfitzmac
ms.openlocfilehash: 9a525d031c9f24cf18495d83e22467e103bca6d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363688"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="967c3-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="967c3-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="967c3-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="967c3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="967c3-105">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="967c3-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="967c3-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="967c3-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="967c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="967c3-107">Properties</span></span>
|<span data-ttu-id="967c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="967c3-108">Property</span></span>|<span data-ttu-id="967c3-109">类型</span><span class="sxs-lookup"><span data-stu-id="967c3-109">Type</span></span>|<span data-ttu-id="967c3-110">说明</span><span class="sxs-lookup"><span data-stu-id="967c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="967c3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="967c3-111">displayName</span></span>|<span data-ttu-id="967c3-112">String</span><span class="sxs-lookup"><span data-stu-id="967c3-112">String</span></span>|<span data-ttu-id="967c3-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="967c3-113">Display Name.</span></span> <span data-ttu-id="967c3-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="967c3-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="967c3-115">description</span><span class="sxs-lookup"><span data-stu-id="967c3-115">description</span></span>|<span data-ttu-id="967c3-116">String</span><span class="sxs-lookup"><span data-stu-id="967c3-116">String</span></span>|<span data-ttu-id="967c3-117">说明。</span><span class="sxs-lookup"><span data-stu-id="967c3-117">Description.</span></span> <span data-ttu-id="967c3-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="967c3-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="967c3-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="967c3-119">omaUri</span></span>|<span data-ttu-id="967c3-120">String</span><span class="sxs-lookup"><span data-stu-id="967c3-120">String</span></span>|<span data-ttu-id="967c3-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="967c3-121">OMA.</span></span> <span data-ttu-id="967c3-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="967c3-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="967c3-123">value</span><span class="sxs-lookup"><span data-stu-id="967c3-123">value</span></span>|<span data-ttu-id="967c3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="967c3-124">DateTimeOffset</span></span>|<span data-ttu-id="967c3-125">值。</span><span class="sxs-lookup"><span data-stu-id="967c3-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="967c3-126">关系</span><span class="sxs-lookup"><span data-stu-id="967c3-126">Relationships</span></span>
<span data-ttu-id="967c3-127">无</span><span class="sxs-lookup"><span data-stu-id="967c3-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="967c3-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="967c3-128">JSON Representation</span></span>
<span data-ttu-id="967c3-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="967c3-129">Here is a JSON representation of the resource.</span></span>
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



