---
title: deviceHealthScriptIntegerParameter 资源类型
description: Integer 脚本参数的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f88f027036c93b62610b9cd6d95821b5115a2334
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178561"
---
# <a name="devicehealthscriptintegerparameter-resource-type"></a><span data-ttu-id="38873-103">deviceHealthScriptIntegerParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="38873-103">deviceHealthScriptIntegerParameter resource type</span></span>

<span data-ttu-id="38873-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38873-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="38873-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="38873-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38873-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38873-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38873-107">Integer 脚本参数的属性。</span><span class="sxs-lookup"><span data-stu-id="38873-107">Properties of the  Integer script parameter.</span></span>


<span data-ttu-id="38873-108">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span><span class="sxs-lookup"><span data-stu-id="38873-108">Inherits from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>

## <a name="properties"></a><span data-ttu-id="38873-109">属性</span><span class="sxs-lookup"><span data-stu-id="38873-109">Properties</span></span>
|<span data-ttu-id="38873-110">属性</span><span class="sxs-lookup"><span data-stu-id="38873-110">Property</span></span>|<span data-ttu-id="38873-111">类型</span><span class="sxs-lookup"><span data-stu-id="38873-111">Type</span></span>|<span data-ttu-id="38873-112">说明</span><span class="sxs-lookup"><span data-stu-id="38873-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38873-113">name</span><span class="sxs-lookup"><span data-stu-id="38873-113">name</span></span>|<span data-ttu-id="38873-114">字符串</span><span class="sxs-lookup"><span data-stu-id="38873-114">String</span></span>|<span data-ttu-id="38873-115">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的 param 的名称</span><span class="sxs-lookup"><span data-stu-id="38873-115">The name of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="38873-116">说明</span><span class="sxs-lookup"><span data-stu-id="38873-116">description</span></span>|<span data-ttu-id="38873-117">String</span><span class="sxs-lookup"><span data-stu-id="38873-117">String</span></span>|<span data-ttu-id="38873-118">继承自[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)的参数的说明</span><span class="sxs-lookup"><span data-stu-id="38873-118">The description of the param Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="38873-119">isRequired</span><span class="sxs-lookup"><span data-stu-id="38873-119">isRequired</span></span>|<span data-ttu-id="38873-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="38873-120">Boolean</span></span>|<span data-ttu-id="38873-121">是否需要从[DeviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)继承 param</span><span class="sxs-lookup"><span data-stu-id="38873-121">Whether the param is required Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="38873-122">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="38873-122">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="38873-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="38873-123">Boolean</span></span>|<span data-ttu-id="38873-124">从[deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)中继承未分配的情况时是否应用 DefaultValue</span><span class="sxs-lookup"><span data-stu-id="38873-124">Whether Apply DefaultValue When Not Assigned Inherited from [deviceHealthScriptParameter](../resources/intune-devices-devicehealthscriptparameter.md)</span></span>|
|<span data-ttu-id="38873-125">默认</span><span class="sxs-lookup"><span data-stu-id="38873-125">defaultValue</span></span>|<span data-ttu-id="38873-126">Int32</span><span class="sxs-lookup"><span data-stu-id="38873-126">Int32</span></span>|<span data-ttu-id="38873-127">Integer 参数的默认值。</span><span class="sxs-lookup"><span data-stu-id="38873-127">The default value of Integer param.</span></span> <span data-ttu-id="38873-128">有效值-2147483648 到2147483647</span><span class="sxs-lookup"><span data-stu-id="38873-128">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="38873-129">关系</span><span class="sxs-lookup"><span data-stu-id="38873-129">Relationships</span></span>
<span data-ttu-id="38873-130">无</span><span class="sxs-lookup"><span data-stu-id="38873-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="38873-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38873-131">JSON Representation</span></span>
<span data-ttu-id="38873-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38873-132">Here is a JSON representation of the resource.</span></span>
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



