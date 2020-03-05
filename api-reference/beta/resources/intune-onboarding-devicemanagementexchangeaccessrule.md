---
title: deviceManagementExchangeAccessRule 资源类型
description: Exchange 中的设备访问规则。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a09d1fdea20583c7f80036ae54ca518df92bd5c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524165"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="d8e44-103">deviceManagementExchangeAccessRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8e44-103">deviceManagementExchangeAccessRule resource type</span></span>

<span data-ttu-id="d8e44-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d8e44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8e44-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8e44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8e44-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8e44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8e44-107">Exchange 中的设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="d8e44-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="d8e44-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8e44-108">Properties</span></span>
|<span data-ttu-id="d8e44-109">属性</span><span class="sxs-lookup"><span data-stu-id="d8e44-109">Property</span></span>|<span data-ttu-id="d8e44-110">类型</span><span class="sxs-lookup"><span data-stu-id="d8e44-110">Type</span></span>|<span data-ttu-id="d8e44-111">说明</span><span class="sxs-lookup"><span data-stu-id="d8e44-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e44-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="d8e44-112">deviceClass</span></span>|[<span data-ttu-id="d8e44-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="d8e44-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="d8e44-114">将受此规则影响的设备类别。</span><span class="sxs-lookup"><span data-stu-id="d8e44-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="d8e44-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="d8e44-115">accessLevel</span></span>|[<span data-ttu-id="d8e44-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="d8e44-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="d8e44-117">此规则授予的 Exchange 访问级别。</span><span class="sxs-lookup"><span data-stu-id="d8e44-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="d8e44-118">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="d8e44-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8e44-119">关系</span><span class="sxs-lookup"><span data-stu-id="d8e44-119">Relationships</span></span>
<span data-ttu-id="d8e44-120">无</span><span class="sxs-lookup"><span data-stu-id="d8e44-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8e44-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8e44-121">JSON Representation</span></span>
<span data-ttu-id="d8e44-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8e44-122">Here is a JSON representation of the resource.</span></span>
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



