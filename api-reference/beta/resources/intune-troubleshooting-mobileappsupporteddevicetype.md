---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
ms.openlocfilehash: 7bea84a009d8940608c82bbb551c2d3c8be750ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043842"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="02b2e-103">mobileAppSupportedDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="02b2e-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="02b2e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="02b2e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02b2e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="02b2e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02b2e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="02b2e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02b2e-107">设备属性</span><span class="sxs-lookup"><span data-stu-id="02b2e-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="02b2e-108">属性</span><span class="sxs-lookup"><span data-stu-id="02b2e-108">Properties</span></span>
|<span data-ttu-id="02b2e-109">属性</span><span class="sxs-lookup"><span data-stu-id="02b2e-109">Property</span></span>|<span data-ttu-id="02b2e-110">类型</span><span class="sxs-lookup"><span data-stu-id="02b2e-110">Type</span></span>|<span data-ttu-id="02b2e-111">说明</span><span class="sxs-lookup"><span data-stu-id="02b2e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02b2e-112">type</span><span class="sxs-lookup"><span data-stu-id="02b2e-112">type</span></span>|[<span data-ttu-id="02b2e-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="02b2e-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="02b2e-114">设备类型。</span><span class="sxs-lookup"><span data-stu-id="02b2e-114">Device type.</span></span> <span data-ttu-id="02b2e-115">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="02b2e-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="02b2e-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="02b2e-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="02b2e-117">字符串</span><span class="sxs-lookup"><span data-stu-id="02b2e-117">String</span></span>|<span data-ttu-id="02b2e-118">最低操作系统版本</span><span class="sxs-lookup"><span data-stu-id="02b2e-118">Minimum OS version</span></span>|
|<span data-ttu-id="02b2e-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="02b2e-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="02b2e-120">字符串</span><span class="sxs-lookup"><span data-stu-id="02b2e-120">String</span></span>|<span data-ttu-id="02b2e-121">最大操作系统版本</span><span class="sxs-lookup"><span data-stu-id="02b2e-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="02b2e-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="02b2e-122">Relationships</span></span>
<span data-ttu-id="02b2e-123">无</span><span class="sxs-lookup"><span data-stu-id="02b2e-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02b2e-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="02b2e-124">JSON Representation</span></span>
<span data-ttu-id="02b2e-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02b2e-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppSupportedDeviceType",
  "type": "String",
  "minimumOperatingSystemVersion": "String",
  "maximumOperatingSystemVersion": "String"
}
```





