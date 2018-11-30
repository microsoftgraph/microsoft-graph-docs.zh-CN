---
title: deviceManagementExchangeDeviceClass 资源类型
description: Exchange 中的设备类。
ms.openlocfilehash: 53234a97ffd2581eea1a4c480161ec9243a710d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048228"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="d06a1-103">deviceManagementExchangeDeviceClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="d06a1-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="d06a1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d06a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d06a1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d06a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d06a1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d06a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d06a1-107">Exchange 中的设备类。</span><span class="sxs-lookup"><span data-stu-id="d06a1-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="d06a1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d06a1-108">Properties</span></span>
|<span data-ttu-id="d06a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="d06a1-109">Property</span></span>|<span data-ttu-id="d06a1-110">类型</span><span class="sxs-lookup"><span data-stu-id="d06a1-110">Type</span></span>|<span data-ttu-id="d06a1-111">说明</span><span class="sxs-lookup"><span data-stu-id="d06a1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d06a1-112">name</span><span class="sxs-lookup"><span data-stu-id="d06a1-112">name</span></span>|<span data-ttu-id="d06a1-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d06a1-113">String</span></span>|<span data-ttu-id="d06a1-114">设备类，该类将会受到此规则的名称。</span><span class="sxs-lookup"><span data-stu-id="d06a1-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="d06a1-115">type</span><span class="sxs-lookup"><span data-stu-id="d06a1-115">type</span></span>|[<span data-ttu-id="d06a1-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="d06a1-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="d06a1-117">设备受到此规则的类型例如建模、 系列。</span><span class="sxs-lookup"><span data-stu-id="d06a1-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="d06a1-118">可取值为：`family`、`model`。</span><span class="sxs-lookup"><span data-stu-id="d06a1-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d06a1-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="d06a1-119">Relationships</span></span>
<span data-ttu-id="d06a1-120">无</span><span class="sxs-lookup"><span data-stu-id="d06a1-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d06a1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d06a1-121">JSON Representation</span></span>
<span data-ttu-id="d06a1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d06a1-122">Here is a JSON representation of the resource.</span></span>
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





