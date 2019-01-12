---
title: omaSettingDateTime 资源类型
description: OMA 设置日期时间定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 34c19caee6bab30dbfe0e82abf1a55f20bb5d3b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932292"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="f50a3-103">omaSettingDateTime 资源类型</span><span class="sxs-lookup"><span data-stu-id="f50a3-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="f50a3-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f50a3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f50a3-105">OMA 设置日期时间定义。</span><span class="sxs-lookup"><span data-stu-id="f50a3-105">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="f50a3-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f50a3-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f50a3-107">属性</span><span class="sxs-lookup"><span data-stu-id="f50a3-107">Properties</span></span>
|<span data-ttu-id="f50a3-108">属性</span><span class="sxs-lookup"><span data-stu-id="f50a3-108">Property</span></span>|<span data-ttu-id="f50a3-109">类型</span><span class="sxs-lookup"><span data-stu-id="f50a3-109">Type</span></span>|<span data-ttu-id="f50a3-110">说明</span><span class="sxs-lookup"><span data-stu-id="f50a3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f50a3-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f50a3-111">displayName</span></span>|<span data-ttu-id="f50a3-112">String</span><span class="sxs-lookup"><span data-stu-id="f50a3-112">String</span></span>|<span data-ttu-id="f50a3-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f50a3-113">Display Name.</span></span> <span data-ttu-id="f50a3-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f50a3-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f50a3-115">description</span><span class="sxs-lookup"><span data-stu-id="f50a3-115">description</span></span>|<span data-ttu-id="f50a3-116">String</span><span class="sxs-lookup"><span data-stu-id="f50a3-116">String</span></span>|<span data-ttu-id="f50a3-117">说明。</span><span class="sxs-lookup"><span data-stu-id="f50a3-117">Description.</span></span> <span data-ttu-id="f50a3-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f50a3-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f50a3-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f50a3-119">omaUri</span></span>|<span data-ttu-id="f50a3-120">String</span><span class="sxs-lookup"><span data-stu-id="f50a3-120">String</span></span>|<span data-ttu-id="f50a3-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="f50a3-121">OMA.</span></span> <span data-ttu-id="f50a3-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="f50a3-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f50a3-123">value</span><span class="sxs-lookup"><span data-stu-id="f50a3-123">value</span></span>|<span data-ttu-id="f50a3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f50a3-124">DateTimeOffset</span></span>|<span data-ttu-id="f50a3-125">值。</span><span class="sxs-lookup"><span data-stu-id="f50a3-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f50a3-126">关系</span><span class="sxs-lookup"><span data-stu-id="f50a3-126">Relationships</span></span>
<span data-ttu-id="f50a3-127">无</span><span class="sxs-lookup"><span data-stu-id="f50a3-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f50a3-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f50a3-128">JSON Representation</span></span>
<span data-ttu-id="f50a3-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f50a3-129">Here is a JSON representation of the resource.</span></span>
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



