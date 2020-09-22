---
title: deviceHealthScriptIntegerParameter 资源类型
description: Integer 脚本参数的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8154284e74cb4563ef881071c2a40ed9ec57adcd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060319"
---
# <a name="devicehealthscriptintegerparameter-resource-type"></a><span data-ttu-id="34342-103">deviceHealthScriptIntegerParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="34342-103">deviceHealthScriptIntegerParameter resource type</span></span>

<span data-ttu-id="34342-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34342-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34342-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34342-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34342-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34342-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34342-107">Integer 脚本参数的属性。</span><span class="sxs-lookup"><span data-stu-id="34342-107">Properties of the  Integer script parameter.</span></span>


<span data-ttu-id="34342-108">继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="34342-108">Inherits from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34342-109">属性</span><span class="sxs-lookup"><span data-stu-id="34342-109">Properties</span></span>
|<span data-ttu-id="34342-110">属性</span><span class="sxs-lookup"><span data-stu-id="34342-110">Property</span></span>|<span data-ttu-id="34342-111">类型</span><span class="sxs-lookup"><span data-stu-id="34342-111">Type</span></span>|<span data-ttu-id="34342-112">说明</span><span class="sxs-lookup"><span data-stu-id="34342-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34342-113">名称</span><span class="sxs-lookup"><span data-stu-id="34342-113">name</span></span>|<span data-ttu-id="34342-114">String</span><span class="sxs-lookup"><span data-stu-id="34342-114">String</span></span>|<span data-ttu-id="34342-115">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的 param 的名称</span><span class="sxs-lookup"><span data-stu-id="34342-115">The name of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="34342-116">说明</span><span class="sxs-lookup"><span data-stu-id="34342-116">description</span></span>|<span data-ttu-id="34342-117">String</span><span class="sxs-lookup"><span data-stu-id="34342-117">String</span></span>|<span data-ttu-id="34342-118">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的参数的说明</span><span class="sxs-lookup"><span data-stu-id="34342-118">The description of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="34342-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="34342-119">isRequired</span></span>|<span data-ttu-id="34342-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="34342-120">Boolean</span></span>|<span data-ttu-id="34342-121">是否需要从[DeviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)继承 param</span><span class="sxs-lookup"><span data-stu-id="34342-121">Whether the param is required Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="34342-122">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="34342-122">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="34342-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="34342-123">Boolean</span></span>|<span data-ttu-id="34342-124">从[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)中继承未分配的情况时是否应用 DefaultValue</span><span class="sxs-lookup"><span data-stu-id="34342-124">Whether Apply DefaultValue When Not Assigned Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="34342-125">默认</span><span class="sxs-lookup"><span data-stu-id="34342-125">defaultValue</span></span>|<span data-ttu-id="34342-126">Int32</span><span class="sxs-lookup"><span data-stu-id="34342-126">Int32</span></span>|<span data-ttu-id="34342-127">Integer 参数的默认值。</span><span class="sxs-lookup"><span data-stu-id="34342-127">The default value of Integer param.</span></span> <span data-ttu-id="34342-128">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="34342-128">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="34342-129">关系</span><span class="sxs-lookup"><span data-stu-id="34342-129">Relationships</span></span>
<span data-ttu-id="34342-130">无</span><span class="sxs-lookup"><span data-stu-id="34342-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34342-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34342-131">JSON Representation</span></span>
<span data-ttu-id="34342-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34342-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptIntegerParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptIntegerParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true,
  "defaultValue": 1024
}
```






