---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e512253a9b9bc4228d41c369501bec1e7a5e031
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413729"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="2b340-103">deviceManagementExchangeDeviceClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b340-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="2b340-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2b340-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b340-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b340-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b340-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b340-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b340-107">Exchange 中的设备类。</span><span class="sxs-lookup"><span data-stu-id="2b340-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="2b340-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b340-108">Properties</span></span>
|<span data-ttu-id="2b340-109">属性</span><span class="sxs-lookup"><span data-stu-id="2b340-109">Property</span></span>|<span data-ttu-id="2b340-110">类型</span><span class="sxs-lookup"><span data-stu-id="2b340-110">Type</span></span>|<span data-ttu-id="2b340-111">说明</span><span class="sxs-lookup"><span data-stu-id="2b340-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b340-112">name</span><span class="sxs-lookup"><span data-stu-id="2b340-112">name</span></span>|<span data-ttu-id="2b340-113">String</span><span class="sxs-lookup"><span data-stu-id="2b340-113">String</span></span>|<span data-ttu-id="2b340-114">设备类，该类将会受到此规则的名称。</span><span class="sxs-lookup"><span data-stu-id="2b340-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="2b340-115">type</span><span class="sxs-lookup"><span data-stu-id="2b340-115">type</span></span>|[<span data-ttu-id="2b340-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="2b340-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="2b340-117">设备受到此规则的类型例如建模、 系列。</span><span class="sxs-lookup"><span data-stu-id="2b340-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="2b340-118">可取值为：`family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="2b340-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b340-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="2b340-119">Relationships</span></span>
<span data-ttu-id="2b340-120">无</span><span class="sxs-lookup"><span data-stu-id="2b340-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b340-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b340-121">JSON Representation</span></span>
<span data-ttu-id="2b340-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b340-122">Here is a JSON representation of the resource.</span></span>
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




