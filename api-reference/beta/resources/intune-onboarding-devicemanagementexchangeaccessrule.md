---
title: deviceManagementExchangeAccessRule 资源类型
description: Exchange 中的设备访问规则。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c46bff30bf5f88723a789bb13160bf5aedb1ef2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409438"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="f6045-103">deviceManagementExchangeAccessRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6045-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="f6045-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f6045-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f6045-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f6045-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f6045-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6045-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6045-107">Exchange 中的设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="f6045-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="f6045-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6045-108">Properties</span></span>
|<span data-ttu-id="f6045-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6045-109">Property</span></span>|<span data-ttu-id="f6045-110">类型</span><span class="sxs-lookup"><span data-stu-id="f6045-110">Type</span></span>|<span data-ttu-id="f6045-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6045-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6045-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="f6045-112">deviceClass</span></span>|[<span data-ttu-id="f6045-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="f6045-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="f6045-114">设备类，该类将会受到此规则。</span><span class="sxs-lookup"><span data-stu-id="f6045-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="f6045-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="f6045-115">accessLevel</span></span>|[<span data-ttu-id="f6045-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f6045-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="f6045-117">Exchange 授予此规则的访问级别。</span><span class="sxs-lookup"><span data-stu-id="f6045-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="f6045-118">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="f6045-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6045-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="f6045-119">Relationships</span></span>
<span data-ttu-id="f6045-120">无</span><span class="sxs-lookup"><span data-stu-id="f6045-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6045-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6045-121">JSON Representation</span></span>
<span data-ttu-id="f6045-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6045-122">Here is a JSON representation of the resource.</span></span>
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




