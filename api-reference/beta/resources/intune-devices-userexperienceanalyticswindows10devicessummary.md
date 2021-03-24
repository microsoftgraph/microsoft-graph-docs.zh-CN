---
title: userExperienceAnalyticsWindows10DevicesSummary 资源类型
description: 用户体验分析可随时随地使用 Windows 10 设备摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f43c2848902b6d9fbb3e54a2fd9a8ac36edc0793
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146757"
---
# <a name="userexperienceanalyticswindows10devicessummary-resource-type"></a><span data-ttu-id="65778-103">userExperienceAnalyticsWindows10DevicesSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="65778-103">userExperienceAnalyticsWindows10DevicesSummary resource type</span></span>

<span data-ttu-id="65778-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65778-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65778-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65778-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65778-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65778-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65778-107">用户体验分析可随时随地使用 Windows 10 设备摘要。</span><span class="sxs-lookup"><span data-stu-id="65778-107">The user experience analytics work from anywhere Windows 10 devices summary.</span></span>

## <a name="properties"></a><span data-ttu-id="65778-108">属性</span><span class="sxs-lookup"><span data-stu-id="65778-108">Properties</span></span>
|<span data-ttu-id="65778-109">属性</span><span class="sxs-lookup"><span data-stu-id="65778-109">Property</span></span>|<span data-ttu-id="65778-110">类型</span><span class="sxs-lookup"><span data-stu-id="65778-110">Type</span></span>|<span data-ttu-id="65778-111">说明</span><span class="sxs-lookup"><span data-stu-id="65778-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65778-112">unsupportedOSversionDeviceCount</span><span class="sxs-lookup"><span data-stu-id="65778-112">unsupportedOSversionDeviceCount</span></span>|<span data-ttu-id="65778-113">Int32</span><span class="sxs-lookup"><span data-stu-id="65778-113">Int32</span></span>|<span data-ttu-id="65778-114">具有不受支持的操作系统版本的 Windows 10 设备计数。</span><span class="sxs-lookup"><span data-stu-id="65778-114">The count of Windows 10 devices that have unsupported OS versions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65778-115">关系</span><span class="sxs-lookup"><span data-stu-id="65778-115">Relationships</span></span>
<span data-ttu-id="65778-116">无</span><span class="sxs-lookup"><span data-stu-id="65778-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65778-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65778-117">JSON Representation</span></span>
<span data-ttu-id="65778-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65778-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
  "unsupportedOSversionDeviceCount": 1024
}
```




