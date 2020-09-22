---
title: omaSettingInteger 资源类型
description: OMA 设置整数定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64fbfca7b5fc101ea7ea64d4545257354d4157e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010169"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="069a1-103">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="069a1-103">omaSettingInteger resource type</span></span>

<span data-ttu-id="069a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="069a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="069a1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="069a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="069a1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="069a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="069a1-107">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="069a1-107">OMA Settings Integer definition.</span></span>


<span data-ttu-id="069a1-108">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="069a1-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="069a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="069a1-109">Properties</span></span>
|<span data-ttu-id="069a1-110">属性</span><span class="sxs-lookup"><span data-stu-id="069a1-110">Property</span></span>|<span data-ttu-id="069a1-111">类型</span><span class="sxs-lookup"><span data-stu-id="069a1-111">Type</span></span>|<span data-ttu-id="069a1-112">说明</span><span class="sxs-lookup"><span data-stu-id="069a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="069a1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="069a1-113">displayName</span></span>|<span data-ttu-id="069a1-114">String</span><span class="sxs-lookup"><span data-stu-id="069a1-114">String</span></span>|<span data-ttu-id="069a1-115">显示名称。</span><span class="sxs-lookup"><span data-stu-id="069a1-115">Display Name.</span></span> <span data-ttu-id="069a1-116">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="069a1-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="069a1-117">description</span><span class="sxs-lookup"><span data-stu-id="069a1-117">description</span></span>|<span data-ttu-id="069a1-118">String</span><span class="sxs-lookup"><span data-stu-id="069a1-118">String</span></span>|<span data-ttu-id="069a1-119">说明。</span><span class="sxs-lookup"><span data-stu-id="069a1-119">Description.</span></span> <span data-ttu-id="069a1-120">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="069a1-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="069a1-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="069a1-121">omaUri</span></span>|<span data-ttu-id="069a1-122">String</span><span class="sxs-lookup"><span data-stu-id="069a1-122">String</span></span>|<span data-ttu-id="069a1-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="069a1-123">OMA.</span></span> <span data-ttu-id="069a1-124">继承自 [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="069a1-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="069a1-125">值</span><span class="sxs-lookup"><span data-stu-id="069a1-125">value</span></span>|<span data-ttu-id="069a1-126">Int32</span><span class="sxs-lookup"><span data-stu-id="069a1-126">Int32</span></span>|<span data-ttu-id="069a1-127">值。</span><span class="sxs-lookup"><span data-stu-id="069a1-127">Value.</span></span>|
|<span data-ttu-id="069a1-128">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="069a1-128">isReadOnly</span></span>|<span data-ttu-id="069a1-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="069a1-129">Boolean</span></span>|<span data-ttu-id="069a1-130">通过将设置为 true，则在 OMA-URI 中指定的 CSP (配置服务提供程序) 将执行 get，而不是设置</span><span class="sxs-lookup"><span data-stu-id="069a1-130">By setting to true, the CSP (configuration service provider) specified in the OMA-URI will perform a get, instead of set</span></span>|

## <a name="relationships"></a><span data-ttu-id="069a1-131">关系</span><span class="sxs-lookup"><span data-stu-id="069a1-131">Relationships</span></span>
<span data-ttu-id="069a1-132">无</span><span class="sxs-lookup"><span data-stu-id="069a1-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="069a1-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="069a1-133">JSON Representation</span></span>
<span data-ttu-id="069a1-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="069a1-134">Here is a JSON representation of the resource.</span></span>
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
  "value": 1024,
  "isReadOnly": true
}
```






