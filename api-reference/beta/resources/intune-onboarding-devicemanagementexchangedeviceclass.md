---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ec9f0242521bf23b4ed5f1c9f002211d542e48c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566561"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="fe251-103">deviceManagementExchangeDeviceClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe251-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="fe251-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe251-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe251-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe251-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe251-106">Exchange 中的设备类。</span><span class="sxs-lookup"><span data-stu-id="fe251-106">Device Class in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="fe251-107">属性</span><span class="sxs-lookup"><span data-stu-id="fe251-107">Properties</span></span>
|<span data-ttu-id="fe251-108">属性</span><span class="sxs-lookup"><span data-stu-id="fe251-108">Property</span></span>|<span data-ttu-id="fe251-109">类型</span><span class="sxs-lookup"><span data-stu-id="fe251-109">Type</span></span>|<span data-ttu-id="fe251-110">说明</span><span class="sxs-lookup"><span data-stu-id="fe251-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe251-111">name</span><span class="sxs-lookup"><span data-stu-id="fe251-111">name</span></span>|<span data-ttu-id="fe251-112">String</span><span class="sxs-lookup"><span data-stu-id="fe251-112">String</span></span>|<span data-ttu-id="fe251-113">将受此规则影响的设备类别的名称。</span><span class="sxs-lookup"><span data-stu-id="fe251-113">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="fe251-114">type</span><span class="sxs-lookup"><span data-stu-id="fe251-114">type</span></span>|[<span data-ttu-id="fe251-115">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="fe251-115">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="fe251-116">受此规则影响的设备类型, 例如 Model、Family。</span><span class="sxs-lookup"><span data-stu-id="fe251-116">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="fe251-117">可取值为：`family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="fe251-117">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe251-118">关系</span><span class="sxs-lookup"><span data-stu-id="fe251-118">Relationships</span></span>
<span data-ttu-id="fe251-119">无</span><span class="sxs-lookup"><span data-stu-id="fe251-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe251-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe251-120">JSON Representation</span></span>
<span data-ttu-id="fe251-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe251-121">Here is a JSON representation of the resource.</span></span>
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





