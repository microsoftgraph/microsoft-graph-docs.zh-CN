---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a3e2fc78712997eebd31a874363f000b4ad761e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863567"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="c6b63-103">mobileAppSupportedDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6b63-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="c6b63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6b63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c6b63-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6b63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6b63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6b63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6b63-107">设备属性</span><span class="sxs-lookup"><span data-stu-id="c6b63-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="c6b63-108">属性</span><span class="sxs-lookup"><span data-stu-id="c6b63-108">Properties</span></span>
|<span data-ttu-id="c6b63-109">属性</span><span class="sxs-lookup"><span data-stu-id="c6b63-109">Property</span></span>|<span data-ttu-id="c6b63-110">类型</span><span class="sxs-lookup"><span data-stu-id="c6b63-110">Type</span></span>|<span data-ttu-id="c6b63-111">说明</span><span class="sxs-lookup"><span data-stu-id="c6b63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6b63-112">类型</span><span class="sxs-lookup"><span data-stu-id="c6b63-112">type</span></span>|[<span data-ttu-id="c6b63-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="c6b63-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c6b63-114">设备类型。</span><span class="sxs-lookup"><span data-stu-id="c6b63-114">Device type.</span></span> <span data-ttu-id="c6b63-115">可能的值是 `desktop` `windowsRT` `winMO6` ：、、、、、、、、、、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `linux` `blackberry` `palm` `unknown` `cloudPC` 、</span><span class="sxs-lookup"><span data-stu-id="c6b63-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.</span></span>|
|<span data-ttu-id="c6b63-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="c6b63-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="c6b63-117">String</span><span class="sxs-lookup"><span data-stu-id="c6b63-117">String</span></span>|<span data-ttu-id="c6b63-118">最低操作系统版本</span><span class="sxs-lookup"><span data-stu-id="c6b63-118">Minimum OS version</span></span>|
|<span data-ttu-id="c6b63-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="c6b63-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="c6b63-120">String</span><span class="sxs-lookup"><span data-stu-id="c6b63-120">String</span></span>|<span data-ttu-id="c6b63-121">最大操作系统版本</span><span class="sxs-lookup"><span data-stu-id="c6b63-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6b63-122">关系</span><span class="sxs-lookup"><span data-stu-id="c6b63-122">Relationships</span></span>
<span data-ttu-id="c6b63-123">无</span><span class="sxs-lookup"><span data-stu-id="c6b63-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6b63-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6b63-124">JSON Representation</span></span>
<span data-ttu-id="c6b63-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6b63-125">Here is a JSON representation of the resource.</span></span>
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




