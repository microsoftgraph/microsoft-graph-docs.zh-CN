---
title: mobileAppSupportedDeviceType 资源类型
description: 设备属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8e0b0f6232645dfff0e59e8d1ff808e47ff472
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523322"
---
# <a name="mobileappsupporteddevicetype-resource-type"></a><span data-ttu-id="54142-103">mobileAppSupportedDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="54142-103">mobileAppSupportedDeviceType resource type</span></span>

<span data-ttu-id="54142-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="54142-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54142-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54142-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54142-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54142-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54142-107">设备属性</span><span class="sxs-lookup"><span data-stu-id="54142-107">Device properties</span></span>

## <a name="properties"></a><span data-ttu-id="54142-108">属性</span><span class="sxs-lookup"><span data-stu-id="54142-108">Properties</span></span>
|<span data-ttu-id="54142-109">属性</span><span class="sxs-lookup"><span data-stu-id="54142-109">Property</span></span>|<span data-ttu-id="54142-110">类型</span><span class="sxs-lookup"><span data-stu-id="54142-110">Type</span></span>|<span data-ttu-id="54142-111">说明</span><span class="sxs-lookup"><span data-stu-id="54142-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54142-112">类型</span><span class="sxs-lookup"><span data-stu-id="54142-112">type</span></span>|[<span data-ttu-id="54142-113">deviceType</span><span class="sxs-lookup"><span data-stu-id="54142-113">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="54142-114">设备类型。</span><span class="sxs-lookup"><span data-stu-id="54142-114">Device type.</span></span> <span data-ttu-id="54142-115">可能的值为`desktop`： `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `palm` `unknown`、、、、、、、、、、、、、、、、、、、、。 `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `blackberry`</span><span class="sxs-lookup"><span data-stu-id="54142-115">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="54142-116">minimumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="54142-116">minimumOperatingSystemVersion</span></span>|<span data-ttu-id="54142-117">String</span><span class="sxs-lookup"><span data-stu-id="54142-117">String</span></span>|<span data-ttu-id="54142-118">最低操作系统版本</span><span class="sxs-lookup"><span data-stu-id="54142-118">Minimum OS version</span></span>|
|<span data-ttu-id="54142-119">maximumOperatingSystemVersion</span><span class="sxs-lookup"><span data-stu-id="54142-119">maximumOperatingSystemVersion</span></span>|<span data-ttu-id="54142-120">String</span><span class="sxs-lookup"><span data-stu-id="54142-120">String</span></span>|<span data-ttu-id="54142-121">最大 OS 版本</span><span class="sxs-lookup"><span data-stu-id="54142-121">Maximum OS version</span></span>|

## <a name="relationships"></a><span data-ttu-id="54142-122">关系</span><span class="sxs-lookup"><span data-stu-id="54142-122">Relationships</span></span>
<span data-ttu-id="54142-123">无</span><span class="sxs-lookup"><span data-stu-id="54142-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54142-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54142-124">JSON Representation</span></span>
<span data-ttu-id="54142-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54142-125">Here is a JSON representation of the resource.</span></span>
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



