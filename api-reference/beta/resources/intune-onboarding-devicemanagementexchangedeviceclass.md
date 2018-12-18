---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
author: tfitzmac
ms.openlocfilehash: 01e0877388391deaebbda18e48247f4e3585a63a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316777"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="5923d-103">deviceManagementExchangeDeviceClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="5923d-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="5923d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5923d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5923d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5923d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5923d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5923d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5923d-107">Exchange 中的设备类。</span><span class="sxs-lookup"><span data-stu-id="5923d-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="5923d-108">属性</span><span class="sxs-lookup"><span data-stu-id="5923d-108">Properties</span></span>
|<span data-ttu-id="5923d-109">属性</span><span class="sxs-lookup"><span data-stu-id="5923d-109">Property</span></span>|<span data-ttu-id="5923d-110">类型</span><span class="sxs-lookup"><span data-stu-id="5923d-110">Type</span></span>|<span data-ttu-id="5923d-111">说明</span><span class="sxs-lookup"><span data-stu-id="5923d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5923d-112">name</span><span class="sxs-lookup"><span data-stu-id="5923d-112">name</span></span>|<span data-ttu-id="5923d-113">字符串</span><span class="sxs-lookup"><span data-stu-id="5923d-113">String</span></span>|<span data-ttu-id="5923d-114">设备类，该类将会受到此规则的名称。</span><span class="sxs-lookup"><span data-stu-id="5923d-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="5923d-115">type</span><span class="sxs-lookup"><span data-stu-id="5923d-115">type</span></span>|[<span data-ttu-id="5923d-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="5923d-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="5923d-117">设备受到此规则的类型例如建模、 系列。</span><span class="sxs-lookup"><span data-stu-id="5923d-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="5923d-118">可取值为：`family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="5923d-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5923d-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="5923d-119">Relationships</span></span>
<span data-ttu-id="5923d-120">无</span><span class="sxs-lookup"><span data-stu-id="5923d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5923d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5923d-121">JSON Representation</span></span>
<span data-ttu-id="5923d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5923d-122">Here is a JSON representation of the resource.</span></span>
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





