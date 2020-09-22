---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 79c1e7cf50bc0cc87f620ad0b875704005b90435
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029608"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="8c16a-103">deviceManagementExchangeDeviceClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c16a-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="8c16a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c16a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8c16a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8c16a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c16a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8c16a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c16a-107">Exchange 中的设备类。</span><span class="sxs-lookup"><span data-stu-id="8c16a-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="8c16a-108">属性</span><span class="sxs-lookup"><span data-stu-id="8c16a-108">Properties</span></span>
|<span data-ttu-id="8c16a-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c16a-109">Property</span></span>|<span data-ttu-id="8c16a-110">类型</span><span class="sxs-lookup"><span data-stu-id="8c16a-110">Type</span></span>|<span data-ttu-id="8c16a-111">说明</span><span class="sxs-lookup"><span data-stu-id="8c16a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c16a-112">name</span><span class="sxs-lookup"><span data-stu-id="8c16a-112">name</span></span>|<span data-ttu-id="8c16a-113">String</span><span class="sxs-lookup"><span data-stu-id="8c16a-113">String</span></span>|<span data-ttu-id="8c16a-114">将受此规则影响的设备类别的名称。</span><span class="sxs-lookup"><span data-stu-id="8c16a-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="8c16a-115">type</span><span class="sxs-lookup"><span data-stu-id="8c16a-115">type</span></span>|[<span data-ttu-id="8c16a-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="8c16a-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="8c16a-117">受此规则影响的设备类型，例如 Model、Family。</span><span class="sxs-lookup"><span data-stu-id="8c16a-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="8c16a-118">可取值为：`family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="8c16a-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c16a-119">关系</span><span class="sxs-lookup"><span data-stu-id="8c16a-119">Relationships</span></span>
<span data-ttu-id="8c16a-120">无</span><span class="sxs-lookup"><span data-stu-id="8c16a-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c16a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c16a-121">JSON Representation</span></span>
<span data-ttu-id="8c16a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c16a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```






