---
title: deviceHealthScriptStringParameter 资源类型
description: 字符串脚本参数的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0515553688e21d63cb52c9883f7da5b7e425b10
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299371"
---
# <a name="devicehealthscriptstringparameter-resource-type"></a><span data-ttu-id="d1d73-103">deviceHealthScriptStringParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1d73-103">deviceHealthScriptStringParameter resource type</span></span>

<span data-ttu-id="d1d73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1d73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1d73-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1d73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1d73-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1d73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1d73-107">字符串脚本参数的属性。</span><span class="sxs-lookup"><span data-stu-id="d1d73-107">Properties of the  String script parameter.</span></span>


<span data-ttu-id="d1d73-108">继承自 [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="d1d73-108">Inherits from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1d73-109">属性</span><span class="sxs-lookup"><span data-stu-id="d1d73-109">Properties</span></span>
|<span data-ttu-id="d1d73-110">属性</span><span class="sxs-lookup"><span data-stu-id="d1d73-110">Property</span></span>|<span data-ttu-id="d1d73-111">类型</span><span class="sxs-lookup"><span data-stu-id="d1d73-111">Type</span></span>|<span data-ttu-id="d1d73-112">Description</span><span class="sxs-lookup"><span data-stu-id="d1d73-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1d73-113">name</span><span class="sxs-lookup"><span data-stu-id="d1d73-113">name</span></span>|<span data-ttu-id="d1d73-114">字符串</span><span class="sxs-lookup"><span data-stu-id="d1d73-114">String</span></span>|<span data-ttu-id="d1d73-115">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的 param 的名称</span><span class="sxs-lookup"><span data-stu-id="d1d73-115">The name of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="d1d73-116">description</span><span class="sxs-lookup"><span data-stu-id="d1d73-116">description</span></span>|<span data-ttu-id="d1d73-117">字符串</span><span class="sxs-lookup"><span data-stu-id="d1d73-117">String</span></span>|<span data-ttu-id="d1d73-118">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的参数的说明</span><span class="sxs-lookup"><span data-stu-id="d1d73-118">The description of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="d1d73-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="d1d73-119">isRequired</span></span>|<span data-ttu-id="d1d73-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1d73-120">Boolean</span></span>|<span data-ttu-id="d1d73-121">是否需要从[DeviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)继承 param</span><span class="sxs-lookup"><span data-stu-id="d1d73-121">Whether the param is required Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="d1d73-122">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="d1d73-122">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="d1d73-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1d73-123">Boolean</span></span>|<span data-ttu-id="d1d73-124">从[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)中继承未分配的情况时是否应用 DefaultValue</span><span class="sxs-lookup"><span data-stu-id="d1d73-124">Whether Apply DefaultValue When Not Assigned Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="d1d73-125">默认</span><span class="sxs-lookup"><span data-stu-id="d1d73-125">defaultValue</span></span>|<span data-ttu-id="d1d73-126">字符串</span><span class="sxs-lookup"><span data-stu-id="d1d73-126">String</span></span>|<span data-ttu-id="d1d73-127">String param 的默认值</span><span class="sxs-lookup"><span data-stu-id="d1d73-127">The default value of string param</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1d73-128">关系</span><span class="sxs-lookup"><span data-stu-id="d1d73-128">Relationships</span></span>
<span data-ttu-id="d1d73-129">无</span><span class="sxs-lookup"><span data-stu-id="d1d73-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1d73-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1d73-130">JSON Representation</span></span>
<span data-ttu-id="d1d73-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1d73-131">Here is a JSON representation of the resource.</span></span>
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




