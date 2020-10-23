---
title: deviceManagementExchangeAccessRule 资源类型
description: Exchange 中的设备访问规则。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a9a7fe3474f53b7107fb7fe35c1a80f743cfb7b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697229"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="c7a98-103">deviceManagementExchangeAccessRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7a98-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="c7a98-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c7a98-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7a98-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7a98-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7a98-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7a98-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7a98-107">Exchange 中的设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="c7a98-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="c7a98-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7a98-108">Properties</span></span>
|<span data-ttu-id="c7a98-109">属性</span><span class="sxs-lookup"><span data-stu-id="c7a98-109">Property</span></span>|<span data-ttu-id="c7a98-110">类型</span><span class="sxs-lookup"><span data-stu-id="c7a98-110">Type</span></span>|<span data-ttu-id="c7a98-111">说明</span><span class="sxs-lookup"><span data-stu-id="c7a98-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7a98-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="c7a98-112">deviceClass</span></span>|[<span data-ttu-id="c7a98-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="c7a98-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="c7a98-114">将受此规则影响的设备类别。</span><span class="sxs-lookup"><span data-stu-id="c7a98-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="c7a98-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="c7a98-115">accessLevel</span></span>|[<span data-ttu-id="c7a98-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="c7a98-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="c7a98-117">此规则授予的 Exchange 访问级别。</span><span class="sxs-lookup"><span data-stu-id="c7a98-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="c7a98-118">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="c7a98-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7a98-119">关系</span><span class="sxs-lookup"><span data-stu-id="c7a98-119">Relationships</span></span>
<span data-ttu-id="c7a98-120">无</span><span class="sxs-lookup"><span data-stu-id="c7a98-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7a98-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7a98-121">JSON Representation</span></span>
<span data-ttu-id="c7a98-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7a98-122">Here is a JSON representation of the resource.</span></span>
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





