---
title: deviceManagementExchangeAccessRule 资源类型
description: Exchange 中的设备访问规则。
ms.openlocfilehash: e59c81fdfe6cb6a0a7f7f952e6bfc8929bbc2633
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044438"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="aa326-103">deviceManagementExchangeAccessRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa326-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="aa326-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aa326-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa326-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aa326-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aa326-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aa326-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa326-107">Exchange 中的设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="aa326-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="aa326-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa326-108">Properties</span></span>
|<span data-ttu-id="aa326-109">属性</span><span class="sxs-lookup"><span data-stu-id="aa326-109">Property</span></span>|<span data-ttu-id="aa326-110">类型</span><span class="sxs-lookup"><span data-stu-id="aa326-110">Type</span></span>|<span data-ttu-id="aa326-111">说明</span><span class="sxs-lookup"><span data-stu-id="aa326-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa326-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="aa326-112">deviceClass</span></span>|[<span data-ttu-id="aa326-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="aa326-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="aa326-114">设备类，该类将会受到此规则。</span><span class="sxs-lookup"><span data-stu-id="aa326-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="aa326-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="aa326-115">accessLevel</span></span>|[<span data-ttu-id="aa326-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="aa326-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="aa326-117">Exchange 授予此规则的访问级别。</span><span class="sxs-lookup"><span data-stu-id="aa326-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="aa326-118">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="aa326-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa326-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="aa326-119">Relationships</span></span>
<span data-ttu-id="aa326-120">无</span><span class="sxs-lookup"><span data-stu-id="aa326-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aa326-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa326-121">JSON Representation</span></span>
<span data-ttu-id="aa326-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa326-122">Here is a JSON representation of the resource.</span></span>
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





