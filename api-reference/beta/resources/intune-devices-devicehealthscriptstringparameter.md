---
title: deviceHealthScriptStringParameter 资源类型
description: 字符串脚本参数的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60562ff6908d96f5694f5182b66d61fba16f21e6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060200"
---
# <a name="devicehealthscriptstringparameter-resource-type"></a><span data-ttu-id="ede38-103">deviceHealthScriptStringParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="ede38-103">deviceHealthScriptStringParameter resource type</span></span>

<span data-ttu-id="ede38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ede38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ede38-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ede38-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ede38-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ede38-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ede38-107">字符串脚本参数的属性。</span><span class="sxs-lookup"><span data-stu-id="ede38-107">Properties of the  String script parameter.</span></span>


<span data-ttu-id="ede38-108">继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="ede38-108">Inherits from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ede38-109">属性</span><span class="sxs-lookup"><span data-stu-id="ede38-109">Properties</span></span>
|<span data-ttu-id="ede38-110">属性</span><span class="sxs-lookup"><span data-stu-id="ede38-110">Property</span></span>|<span data-ttu-id="ede38-111">类型</span><span class="sxs-lookup"><span data-stu-id="ede38-111">Type</span></span>|<span data-ttu-id="ede38-112">说明</span><span class="sxs-lookup"><span data-stu-id="ede38-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede38-113">名称</span><span class="sxs-lookup"><span data-stu-id="ede38-113">name</span></span>|<span data-ttu-id="ede38-114">String</span><span class="sxs-lookup"><span data-stu-id="ede38-114">String</span></span>|<span data-ttu-id="ede38-115">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的 param 的名称</span><span class="sxs-lookup"><span data-stu-id="ede38-115">The name of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="ede38-116">说明</span><span class="sxs-lookup"><span data-stu-id="ede38-116">description</span></span>|<span data-ttu-id="ede38-117">String</span><span class="sxs-lookup"><span data-stu-id="ede38-117">String</span></span>|<span data-ttu-id="ede38-118">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的参数的说明</span><span class="sxs-lookup"><span data-stu-id="ede38-118">The description of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="ede38-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="ede38-119">isRequired</span></span>|<span data-ttu-id="ede38-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ede38-120">Boolean</span></span>|<span data-ttu-id="ede38-121">是否需要从[DeviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)继承 param</span><span class="sxs-lookup"><span data-stu-id="ede38-121">Whether the param is required Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="ede38-122">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="ede38-122">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="ede38-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="ede38-123">Boolean</span></span>|<span data-ttu-id="ede38-124">从[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)中继承未分配的情况时是否应用 DefaultValue</span><span class="sxs-lookup"><span data-stu-id="ede38-124">Whether Apply DefaultValue When Not Assigned Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="ede38-125">默认</span><span class="sxs-lookup"><span data-stu-id="ede38-125">defaultValue</span></span>|<span data-ttu-id="ede38-126">String</span><span class="sxs-lookup"><span data-stu-id="ede38-126">String</span></span>|<span data-ttu-id="ede38-127">String param 的默认值</span><span class="sxs-lookup"><span data-stu-id="ede38-127">The default value of string param</span></span>|

## <a name="relationships"></a><span data-ttu-id="ede38-128">关系</span><span class="sxs-lookup"><span data-stu-id="ede38-128">Relationships</span></span>
<span data-ttu-id="ede38-129">无</span><span class="sxs-lookup"><span data-stu-id="ede38-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ede38-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ede38-130">JSON Representation</span></span>
<span data-ttu-id="ede38-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ede38-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptStringParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptStringParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": "String"
}
```






