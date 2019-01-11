---
title: deviceManagementExchangeAccessRule 资源类型
description: Exchange 中的设备访问规则。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d7f0e649d2c5f2f27a4623fa0f65cf43965f576
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855186"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="04c49-103">deviceManagementExchangeAccessRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="04c49-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="04c49-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04c49-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04c49-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04c49-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04c49-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04c49-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04c49-107">Exchange 中的设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="04c49-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="04c49-108">属性</span><span class="sxs-lookup"><span data-stu-id="04c49-108">Properties</span></span>
|<span data-ttu-id="04c49-109">属性</span><span class="sxs-lookup"><span data-stu-id="04c49-109">Property</span></span>|<span data-ttu-id="04c49-110">类型</span><span class="sxs-lookup"><span data-stu-id="04c49-110">Type</span></span>|<span data-ttu-id="04c49-111">Description</span><span class="sxs-lookup"><span data-stu-id="04c49-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04c49-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="04c49-112">deviceClass</span></span>|[<span data-ttu-id="04c49-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="04c49-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="04c49-114">设备类，该类将会受到此规则。</span><span class="sxs-lookup"><span data-stu-id="04c49-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="04c49-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="04c49-115">accessLevel</span></span>|[<span data-ttu-id="04c49-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="04c49-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="04c49-117">Exchange 授予此规则的访问级别。</span><span class="sxs-lookup"><span data-stu-id="04c49-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="04c49-118">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="04c49-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04c49-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="04c49-119">Relationships</span></span>
<span data-ttu-id="04c49-120">无</span><span class="sxs-lookup"><span data-stu-id="04c49-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04c49-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04c49-121">JSON Representation</span></span>
<span data-ttu-id="04c49-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04c49-122">Here is a JSON representation of the resource.</span></span>
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





