---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
ms.openlocfilehash: 6a2e6fe6e6782159afa99d91785ae9e854a2e99c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306550"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="e49db-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="e49db-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="e49db-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e49db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e49db-105">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="e49db-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="e49db-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e49db-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e49db-107">属性</span><span class="sxs-lookup"><span data-stu-id="e49db-107">Properties</span></span>
|<span data-ttu-id="e49db-108">属性</span><span class="sxs-lookup"><span data-stu-id="e49db-108">Property</span></span>|<span data-ttu-id="e49db-109">类型</span><span class="sxs-lookup"><span data-stu-id="e49db-109">Type</span></span>|<span data-ttu-id="e49db-110">说明</span><span class="sxs-lookup"><span data-stu-id="e49db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e49db-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e49db-111">displayName</span></span>|<span data-ttu-id="e49db-112">String</span><span class="sxs-lookup"><span data-stu-id="e49db-112">String</span></span>|<span data-ttu-id="e49db-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="e49db-113">Display Name.</span></span> <span data-ttu-id="e49db-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e49db-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e49db-115">description</span><span class="sxs-lookup"><span data-stu-id="e49db-115">description</span></span>|<span data-ttu-id="e49db-116">String</span><span class="sxs-lookup"><span data-stu-id="e49db-116">String</span></span>|<span data-ttu-id="e49db-117">说明。</span><span class="sxs-lookup"><span data-stu-id="e49db-117">Description.</span></span> <span data-ttu-id="e49db-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e49db-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e49db-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e49db-119">omaUri</span></span>|<span data-ttu-id="e49db-120">String</span><span class="sxs-lookup"><span data-stu-id="e49db-120">String</span></span>|<span data-ttu-id="e49db-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e49db-121">OMA.</span></span> <span data-ttu-id="e49db-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="e49db-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e49db-123">值</span><span class="sxs-lookup"><span data-stu-id="e49db-123">value</span></span>|<span data-ttu-id="e49db-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e49db-124">Int32</span></span>|<span data-ttu-id="e49db-125">值。</span><span class="sxs-lookup"><span data-stu-id="e49db-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e49db-126">关系</span><span class="sxs-lookup"><span data-stu-id="e49db-126">Relationships</span></span>
<span data-ttu-id="e49db-127">无</span><span class="sxs-lookup"><span data-stu-id="e49db-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e49db-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e49db-128">JSON Representation</span></span>
<span data-ttu-id="e49db-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e49db-129">Here is a JSON representation of the resource.</span></span>
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



