---
title: deviceManagementExchangeAccessRule 资源类型
description: Exchange 中的设备访问规则。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 832e11829300ccd1ac4e1d4e6b08acafb908f3b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566603"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="5f05a-103">deviceManagementExchangeAccessRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f05a-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="5f05a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f05a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f05a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f05a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f05a-106">Exchange 中的设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="5f05a-106">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="5f05a-107">属性</span><span class="sxs-lookup"><span data-stu-id="5f05a-107">Properties</span></span>
|<span data-ttu-id="5f05a-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f05a-108">Property</span></span>|<span data-ttu-id="5f05a-109">类型</span><span class="sxs-lookup"><span data-stu-id="5f05a-109">Type</span></span>|<span data-ttu-id="5f05a-110">说明</span><span class="sxs-lookup"><span data-stu-id="5f05a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f05a-111">deviceClass</span><span class="sxs-lookup"><span data-stu-id="5f05a-111">deviceClass</span></span>|[<span data-ttu-id="5f05a-112">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="5f05a-112">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="5f05a-113">将受此规则影响的设备类别。</span><span class="sxs-lookup"><span data-stu-id="5f05a-113">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="5f05a-114">accessLevel</span><span class="sxs-lookup"><span data-stu-id="5f05a-114">accessLevel</span></span>|[<span data-ttu-id="5f05a-115">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="5f05a-115">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="5f05a-116">此规则授予的 Exchange 访问级别。</span><span class="sxs-lookup"><span data-stu-id="5f05a-116">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="5f05a-117">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="5f05a-117">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f05a-118">关系</span><span class="sxs-lookup"><span data-stu-id="5f05a-118">Relationships</span></span>
<span data-ttu-id="5f05a-119">无</span><span class="sxs-lookup"><span data-stu-id="5f05a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f05a-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f05a-120">JSON Representation</span></span>
<span data-ttu-id="5f05a-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f05a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```





