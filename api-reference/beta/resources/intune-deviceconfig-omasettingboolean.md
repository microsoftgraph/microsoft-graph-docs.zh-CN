---
title: omaSettingBoolean 资源类型
description: OMA 设置布尔定义。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a5753bbe5c434b8d46d80ed79ab3e995dadfcdba
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407198"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="088d1-103">omaSettingBoolean 资源类型</span><span class="sxs-lookup"><span data-stu-id="088d1-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="088d1-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="088d1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="088d1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="088d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="088d1-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="088d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="088d1-107">OMA 设置布尔定义。</span><span class="sxs-lookup"><span data-stu-id="088d1-107">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="088d1-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="088d1-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="088d1-109">属性</span><span class="sxs-lookup"><span data-stu-id="088d1-109">Properties</span></span>
|<span data-ttu-id="088d1-110">属性</span><span class="sxs-lookup"><span data-stu-id="088d1-110">Property</span></span>|<span data-ttu-id="088d1-111">类型</span><span class="sxs-lookup"><span data-stu-id="088d1-111">Type</span></span>|<span data-ttu-id="088d1-112">说明</span><span class="sxs-lookup"><span data-stu-id="088d1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="088d1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="088d1-113">displayName</span></span>|<span data-ttu-id="088d1-114">String</span><span class="sxs-lookup"><span data-stu-id="088d1-114">String</span></span>|<span data-ttu-id="088d1-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="088d1-115">Display Name.</span></span> <span data-ttu-id="088d1-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="088d1-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="088d1-117">description</span><span class="sxs-lookup"><span data-stu-id="088d1-117">description</span></span>|<span data-ttu-id="088d1-118">String</span><span class="sxs-lookup"><span data-stu-id="088d1-118">String</span></span>|<span data-ttu-id="088d1-119">说明。</span><span class="sxs-lookup"><span data-stu-id="088d1-119">Description.</span></span> <span data-ttu-id="088d1-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="088d1-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="088d1-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="088d1-121">omaUri</span></span>|<span data-ttu-id="088d1-122">String</span><span class="sxs-lookup"><span data-stu-id="088d1-122">String</span></span>|<span data-ttu-id="088d1-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="088d1-123">OMA.</span></span> <span data-ttu-id="088d1-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="088d1-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="088d1-125">value</span><span class="sxs-lookup"><span data-stu-id="088d1-125">value</span></span>|<span data-ttu-id="088d1-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="088d1-126">Boolean</span></span>|<span data-ttu-id="088d1-127">值。</span><span class="sxs-lookup"><span data-stu-id="088d1-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="088d1-128">关系</span><span class="sxs-lookup"><span data-stu-id="088d1-128">Relationships</span></span>
<span data-ttu-id="088d1-129">无</span><span class="sxs-lookup"><span data-stu-id="088d1-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="088d1-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="088d1-130">JSON Representation</span></span>
<span data-ttu-id="088d1-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="088d1-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```




