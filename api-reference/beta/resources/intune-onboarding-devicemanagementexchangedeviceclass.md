---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 384fa172c255ec3f21ec0088c2b9f4ab025768ce
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779028"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="dba96-103">deviceManagementExchangeDeviceClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="dba96-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="dba96-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dba96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dba96-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dba96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dba96-106">Exchange 中的设备类。</span><span class="sxs-lookup"><span data-stu-id="dba96-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="dba96-107">属性</span><span class="sxs-lookup"><span data-stu-id="dba96-107">Properties</span></span>
|<span data-ttu-id="dba96-108">属性</span><span class="sxs-lookup"><span data-stu-id="dba96-108">Property</span></span>|<span data-ttu-id="dba96-109">类型</span><span class="sxs-lookup"><span data-stu-id="dba96-109">Type</span></span>|<span data-ttu-id="dba96-110">说明</span><span class="sxs-lookup"><span data-stu-id="dba96-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dba96-111">name</span><span class="sxs-lookup"><span data-stu-id="dba96-111">name</span></span>|<span data-ttu-id="dba96-112">String</span><span class="sxs-lookup"><span data-stu-id="dba96-112">String</span></span>|<span data-ttu-id="dba96-113">将受此规则影响的设备类别的名称。</span><span class="sxs-lookup"><span data-stu-id="dba96-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="dba96-114">type</span><span class="sxs-lookup"><span data-stu-id="dba96-114">type</span></span>|[<span data-ttu-id="dba96-115">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="dba96-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="dba96-116">受此规则影响的设备类型，例如 Model、Family。</span><span class="sxs-lookup"><span data-stu-id="dba96-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="dba96-117">可取值为：`family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="dba96-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dba96-118">关系</span><span class="sxs-lookup"><span data-stu-id="dba96-118">Relationships</span></span>
<span data-ttu-id="dba96-119">无</span><span class="sxs-lookup"><span data-stu-id="dba96-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dba96-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dba96-120">JSON Representation</span></span>
<span data-ttu-id="dba96-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dba96-121">Here is a JSON representation of the resource.</span></span>
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



