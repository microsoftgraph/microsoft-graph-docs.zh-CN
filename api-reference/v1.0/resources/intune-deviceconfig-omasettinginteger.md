---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f46398e43f2a7ea224a07b1637deca2c3a6ed067
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987529"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="05b04-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="05b04-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="05b04-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="05b04-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05b04-105">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="05b04-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="05b04-106">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05b04-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="05b04-107">属性</span><span class="sxs-lookup"><span data-stu-id="05b04-107">Properties</span></span>
|<span data-ttu-id="05b04-108">属性</span><span class="sxs-lookup"><span data-stu-id="05b04-108">Property</span></span>|<span data-ttu-id="05b04-109">类型</span><span class="sxs-lookup"><span data-stu-id="05b04-109">Type</span></span>|<span data-ttu-id="05b04-110">说明</span><span class="sxs-lookup"><span data-stu-id="05b04-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05b04-111">displayName</span><span class="sxs-lookup"><span data-stu-id="05b04-111">displayName</span></span>|<span data-ttu-id="05b04-112">String</span><span class="sxs-lookup"><span data-stu-id="05b04-112">String</span></span>|<span data-ttu-id="05b04-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="05b04-113">Display Name.</span></span> <span data-ttu-id="05b04-114">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05b04-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05b04-115">description</span><span class="sxs-lookup"><span data-stu-id="05b04-115">description</span></span>|<span data-ttu-id="05b04-116">String</span><span class="sxs-lookup"><span data-stu-id="05b04-116">String</span></span>|<span data-ttu-id="05b04-117">说明。</span><span class="sxs-lookup"><span data-stu-id="05b04-117">Description.</span></span> <span data-ttu-id="05b04-118">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05b04-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05b04-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="05b04-119">omaUri</span></span>|<span data-ttu-id="05b04-120">String</span><span class="sxs-lookup"><span data-stu-id="05b04-120">String</span></span>|<span data-ttu-id="05b04-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="05b04-121">OMA.</span></span> <span data-ttu-id="05b04-122">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="05b04-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="05b04-123">值</span><span class="sxs-lookup"><span data-stu-id="05b04-123">value</span></span>|<span data-ttu-id="05b04-124">Int32</span><span class="sxs-lookup"><span data-stu-id="05b04-124">Int32</span></span>|<span data-ttu-id="05b04-125">值。</span><span class="sxs-lookup"><span data-stu-id="05b04-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05b04-126">关系</span><span class="sxs-lookup"><span data-stu-id="05b04-126">Relationships</span></span>
<span data-ttu-id="05b04-127">无</span><span class="sxs-lookup"><span data-stu-id="05b04-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05b04-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05b04-128">JSON Representation</span></span>
<span data-ttu-id="05b04-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05b04-129">Here is a JSON representation of the resource.</span></span>
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



