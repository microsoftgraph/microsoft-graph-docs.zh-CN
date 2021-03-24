---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 559dc38a5fc8d2e9b7142efb43d83a97f29db10c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141377"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="d8bb9-103">mobileAppSupportedDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8bb9-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="d8bb9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8bb9-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8bb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8bb9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8bb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8bb9-107">设备属性</span><span class="sxs-lookup"><span data-stu-id="d8bb9-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="d8bb9-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8bb9-108">Properties</span></span>
|<span data-ttu-id="d8bb9-109">属性</span><span class="sxs-lookup"><span data-stu-id="d8bb9-109">Property</span></span>|<span data-ttu-id="d8bb9-110">类型</span><span class="sxs-lookup"><span data-stu-id="d8bb9-110">Type</span></span>|<span data-ttu-id="d8bb9-111">说明</span><span class="sxs-lookup"><span data-stu-id="d8bb9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8bb9-112">类型</span><span class="sxs-lookup"><span data-stu-id="d8bb9-112">type</span></span>|[<span data-ttu-id="d8bb9-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="d8bb9-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d8bb9-114">设备类型。</span><span class="sxs-lookup"><span data-stu-id="d8bb9-114">Device type.</span></span> <span data-ttu-id="d8bb9-115">可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `chromeOS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、</span><span class="sxs-lookup"><span data-stu-id="d8bb9-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="d8bb9-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d8bb9-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="d8bb9-117">String</span><span class="sxs-lookup"><span data-stu-id="d8bb9-117">String</span></span>|<span data-ttu-id="d8bb9-118">最低操作系统版本</span><span class="sxs-lookup"><span data-stu-id="d8bb9-118">Minimum OS version</span></span>|
|<span data-ttu-id="d8bb9-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="d8bb9-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="d8bb9-120">String</span><span class="sxs-lookup"><span data-stu-id="d8bb9-120">String</span></span>|<span data-ttu-id="d8bb9-121">最大操作系统版本</span><span class="sxs-lookup"><span data-stu-id="d8bb9-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8bb9-122">关系</span><span class="sxs-lookup"><span data-stu-id="d8bb9-122">Relationships</span></span>
<span data-ttu-id="d8bb9-123">无</span><span class="sxs-lookup"><span data-stu-id="d8bb9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8bb9-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8bb9-124">JSON Representation</span></span>
<span data-ttu-id="d8bb9-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8bb9-125">Here is a JSON representation of the resource.</span></span>
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




