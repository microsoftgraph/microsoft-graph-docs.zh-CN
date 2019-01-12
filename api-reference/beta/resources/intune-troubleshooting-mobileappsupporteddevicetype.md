---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b1b757e9c621f77d1a26251345ee6751eca2ca7c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980221"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="cc2f2-103">mobileAppSupportedDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc2f2-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="cc2f2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cc2f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc2f2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc2f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc2f2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cc2f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc2f2-107">设备属性</span><span class="sxs-lookup"><span data-stu-id="cc2f2-107">Device properties</span></span>
## <a name="properties"></a><span data-ttu-id="cc2f2-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc2f2-108">Properties</span></span>
|<span data-ttu-id="cc2f2-109">属性</span><span class="sxs-lookup"><span data-stu-id="cc2f2-109">Property</span></span>|<span data-ttu-id="cc2f2-110">类型</span><span class="sxs-lookup"><span data-stu-id="cc2f2-110">Type</span></span>|<span data-ttu-id="cc2f2-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc2f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc2f2-112">type</span><span class="sxs-lookup"><span data-stu-id="cc2f2-112">type</span></span>|[<span data-ttu-id="cc2f2-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="cc2f2-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="cc2f2-114">设备类型。</span><span class="sxs-lookup"><span data-stu-id="cc2f2-114">Device type.</span></span> <span data-ttu-id="cc2f2-115">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="cc2f2-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="cc2f2-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="cc2f2-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="cc2f2-117">字符串</span><span class="sxs-lookup"><span data-stu-id="cc2f2-117">String</span></span>|<span data-ttu-id="cc2f2-118">最低操作系统版本</span><span class="sxs-lookup"><span data-stu-id="cc2f2-118">Minimum OS version</span></span>|
|<span data-ttu-id="cc2f2-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="cc2f2-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="cc2f2-120">字符串</span><span class="sxs-lookup"><span data-stu-id="cc2f2-120">String</span></span>|<span data-ttu-id="cc2f2-121">最大操作系统版本</span><span class="sxs-lookup"><span data-stu-id="cc2f2-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc2f2-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="cc2f2-122">Relationships</span></span>
<span data-ttu-id="cc2f2-123">无</span><span class="sxs-lookup"><span data-stu-id="cc2f2-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc2f2-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc2f2-124">JSON Representation</span></span>
<span data-ttu-id="cc2f2-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc2f2-125">Here is a JSON representation of the resource.</span></span>
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





