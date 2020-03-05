---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4304fb138ede5cf35db07bbb08814f3d8fcf532f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527744"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="35486-103">deviceManagementExchangeDeviceClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="35486-103">deviceManagementExchangeDeviceClass resource type</span></span>

<span data-ttu-id="35486-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="35486-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35486-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35486-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35486-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35486-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35486-107">Exchange 中的设备类。</span><span class="sxs-lookup"><span data-stu-id="35486-107">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="35486-108">属性</span><span class="sxs-lookup"><span data-stu-id="35486-108">Properties</span></span>
|<span data-ttu-id="35486-109">属性</span><span class="sxs-lookup"><span data-stu-id="35486-109">Property</span></span>|<span data-ttu-id="35486-110">类型</span><span class="sxs-lookup"><span data-stu-id="35486-110">Type</span></span>|<span data-ttu-id="35486-111">说明</span><span class="sxs-lookup"><span data-stu-id="35486-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35486-112">name</span><span class="sxs-lookup"><span data-stu-id="35486-112">name</span></span>|<span data-ttu-id="35486-113">String</span><span class="sxs-lookup"><span data-stu-id="35486-113">String</span></span>|<span data-ttu-id="35486-114">将受此规则影响的设备类别的名称。</span><span class="sxs-lookup"><span data-stu-id="35486-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="35486-115">type</span><span class="sxs-lookup"><span data-stu-id="35486-115">type</span></span>|[<span data-ttu-id="35486-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="35486-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="35486-117">受此规则影响的设备类型，例如 Model、Family。</span><span class="sxs-lookup"><span data-stu-id="35486-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="35486-118">可取值为：`family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="35486-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35486-119">关系</span><span class="sxs-lookup"><span data-stu-id="35486-119">Relationships</span></span>
<span data-ttu-id="35486-120">无</span><span class="sxs-lookup"><span data-stu-id="35486-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35486-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35486-121">JSON Representation</span></span>
<span data-ttu-id="35486-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35486-122">Here is a JSON representation of the resource.</span></span>
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



