---
title: deviceHealthScriptStringParameter 资源类型
description: 字符串脚本参数的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 69c32d284b6c2dcdae1068e81e1b8340d18df147
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729325"
---
# <a name="devicehealthscriptstringparameter-resource-type"></a><span data-ttu-id="8d12d-103">deviceHealthScriptStringParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d12d-103">deviceHealthScriptStringParameter resource type</span></span>

<span data-ttu-id="8d12d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d12d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d12d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8d12d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d12d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d12d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d12d-107">字符串脚本参数的属性。</span><span class="sxs-lookup"><span data-stu-id="8d12d-107">Properties of the  String script parameter.</span></span>


<span data-ttu-id="8d12d-108">继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="8d12d-108">Inherits from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d12d-109">属性</span><span class="sxs-lookup"><span data-stu-id="8d12d-109">Properties</span></span>
|<span data-ttu-id="8d12d-110">属性</span><span class="sxs-lookup"><span data-stu-id="8d12d-110">Property</span></span>|<span data-ttu-id="8d12d-111">类型</span><span class="sxs-lookup"><span data-stu-id="8d12d-111">Type</span></span>|<span data-ttu-id="8d12d-112">说明</span><span class="sxs-lookup"><span data-stu-id="8d12d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d12d-113">name</span><span class="sxs-lookup"><span data-stu-id="8d12d-113">name</span></span>|<span data-ttu-id="8d12d-114">String</span><span class="sxs-lookup"><span data-stu-id="8d12d-114">String</span></span>|<span data-ttu-id="8d12d-115">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的 param 的名称</span><span class="sxs-lookup"><span data-stu-id="8d12d-115">The name of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="8d12d-116">说明</span><span class="sxs-lookup"><span data-stu-id="8d12d-116">description</span></span>|<span data-ttu-id="8d12d-117">String</span><span class="sxs-lookup"><span data-stu-id="8d12d-117">String</span></span>|<span data-ttu-id="8d12d-118">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的参数的说明</span><span class="sxs-lookup"><span data-stu-id="8d12d-118">The description of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="8d12d-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="8d12d-119">isRequired</span></span>|<span data-ttu-id="8d12d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d12d-120">Boolean</span></span>|<span data-ttu-id="8d12d-121">是否需要从[DeviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)继承 param</span><span class="sxs-lookup"><span data-stu-id="8d12d-121">Whether the param is required Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="8d12d-122">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="8d12d-122">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="8d12d-123">布尔</span><span class="sxs-lookup"><span data-stu-id="8d12d-123">Boolean</span></span>|<span data-ttu-id="8d12d-124">从[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)中继承未分配的情况时是否应用 DefaultValue</span><span class="sxs-lookup"><span data-stu-id="8d12d-124">Whether Apply DefaultValue When Not Assigned Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="8d12d-125">默认</span><span class="sxs-lookup"><span data-stu-id="8d12d-125">defaultValue</span></span>|<span data-ttu-id="8d12d-126">String</span><span class="sxs-lookup"><span data-stu-id="8d12d-126">String</span></span>|<span data-ttu-id="8d12d-127">String param 的默认值</span><span class="sxs-lookup"><span data-stu-id="8d12d-127">The default value of string param</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d12d-128">关系</span><span class="sxs-lookup"><span data-stu-id="8d12d-128">Relationships</span></span>
<span data-ttu-id="8d12d-129">无</span><span class="sxs-lookup"><span data-stu-id="8d12d-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d12d-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d12d-130">JSON Representation</span></span>
<span data-ttu-id="8d12d-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d12d-131">Here is a JSON representation of the resource.</span></span>
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





