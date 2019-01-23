---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c01691b3f6fcb2ed5838c1c9103c99ad6fbe792f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399750"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="4078d-103">mobileAppSupportedDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="4078d-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="4078d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4078d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4078d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4078d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4078d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4078d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4078d-107">设备属性</span><span class="sxs-lookup"><span data-stu-id="4078d-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="4078d-108">属性</span><span class="sxs-lookup"><span data-stu-id="4078d-108">Properties</span></span>
|<span data-ttu-id="4078d-109">属性</span><span class="sxs-lookup"><span data-stu-id="4078d-109">Property</span></span>|<span data-ttu-id="4078d-110">类型</span><span class="sxs-lookup"><span data-stu-id="4078d-110">Type</span></span>|<span data-ttu-id="4078d-111">说明</span><span class="sxs-lookup"><span data-stu-id="4078d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4078d-112">type</span><span class="sxs-lookup"><span data-stu-id="4078d-112">type</span></span>|[<span data-ttu-id="4078d-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="4078d-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="4078d-114">设备类型。</span><span class="sxs-lookup"><span data-stu-id="4078d-114">Device type.</span></span> <span data-ttu-id="4078d-115">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4078d-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="4078d-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="4078d-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="4078d-117">String</span><span class="sxs-lookup"><span data-stu-id="4078d-117">String</span></span>|<span data-ttu-id="4078d-118">最低操作系统版本</span><span class="sxs-lookup"><span data-stu-id="4078d-118">Minimum OS version</span></span>|
|<span data-ttu-id="4078d-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="4078d-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="4078d-120">String</span><span class="sxs-lookup"><span data-stu-id="4078d-120">String</span></span>|<span data-ttu-id="4078d-121">最大操作系统版本</span><span class="sxs-lookup"><span data-stu-id="4078d-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="4078d-122">关系</span><span class="sxs-lookup"><span data-stu-id="4078d-122">Relationships</span></span>
<span data-ttu-id="4078d-123">无</span><span class="sxs-lookup"><span data-stu-id="4078d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4078d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4078d-124">JSON Representation</span></span>
<span data-ttu-id="4078d-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4078d-125">Here is a JSON representation of the resource.</span></span>
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




