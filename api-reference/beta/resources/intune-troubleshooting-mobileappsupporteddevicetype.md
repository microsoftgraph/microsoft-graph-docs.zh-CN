---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9dfe596ef2a9564554682b3d5e9408b667b191fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967196"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="bb556-103">mobileAppSupportedDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb556-103">mobileAppSupportedDeviceType resource type</span></span>

> <span data-ttu-id="bb556-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb556-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb556-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb556-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb556-106">设备属性</span><span class="sxs-lookup"><span data-stu-id="bb556-106">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="bb556-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb556-107">Properties</span></span>
|<span data-ttu-id="bb556-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb556-108">Property</span></span>|<span data-ttu-id="bb556-109">类型</span><span class="sxs-lookup"><span data-stu-id="bb556-109">Type</span></span>|<span data-ttu-id="bb556-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb556-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb556-111">类型</span><span class="sxs-lookup"><span data-stu-id="bb556-111">type</span></span>|[<span data-ttu-id="bb556-112">deviceType</span><span class="sxs-lookup"><span data-stu-id="bb556-112">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="bb556-113">设备类型。</span><span class="sxs-lookup"><span data-stu-id="bb556-113">Device type.</span></span> <span data-ttu-id="bb556-114">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="bb556-114">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="bb556-115">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="bb556-115">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="bb556-116">String</span><span class="sxs-lookup"><span data-stu-id="bb556-116">String</span></span>|<span data-ttu-id="bb556-117">最低操作系统版本</span><span class="sxs-lookup"><span data-stu-id="bb556-117">Minimum OS version</span></span>|
|<span data-ttu-id="bb556-118">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="bb556-118">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="bb556-119">String</span><span class="sxs-lookup"><span data-stu-id="bb556-119">String</span></span>|<span data-ttu-id="bb556-120">最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="bb556-120">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb556-121">关系</span><span class="sxs-lookup"><span data-stu-id="bb556-121">Relationships</span></span>
<span data-ttu-id="bb556-122">无</span><span class="sxs-lookup"><span data-stu-id="bb556-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb556-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb556-123">JSON Representation</span></span>
<span data-ttu-id="bb556-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb556-124">Here is a JSON representation of the resource.</span></span>
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





