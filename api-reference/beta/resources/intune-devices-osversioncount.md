---
title: osVersionCount 资源类型
description: 包含每个 OS 版本的包含恶意软件的设备的计数
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2243c5c9897e108701b1729832562b781d63ec51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081144"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="bc4be-103">osVersionCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc4be-103">osVersionCount resource type</span></span>

<span data-ttu-id="bc4be-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc4be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc4be-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bc4be-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc4be-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc4be-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc4be-107">包含每个 OS 版本的包含恶意软件的设备的计数</span><span class="sxs-lookup"><span data-stu-id="bc4be-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="bc4be-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc4be-108">Properties</span></span>
|<span data-ttu-id="bc4be-109">属性</span><span class="sxs-lookup"><span data-stu-id="bc4be-109">Property</span></span>|<span data-ttu-id="bc4be-110">类型</span><span class="sxs-lookup"><span data-stu-id="bc4be-110">Type</span></span>|<span data-ttu-id="bc4be-111">说明</span><span class="sxs-lookup"><span data-stu-id="bc4be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc4be-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="bc4be-112">osVersion</span></span>|<span data-ttu-id="bc4be-113">String</span><span class="sxs-lookup"><span data-stu-id="bc4be-113">String</span></span>|<span data-ttu-id="bc4be-114">OS 版本</span><span class="sxs-lookup"><span data-stu-id="bc4be-114">OS version</span></span>|
|<span data-ttu-id="bc4be-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="bc4be-115">deviceCount</span></span>|<span data-ttu-id="bc4be-116">Int32</span><span class="sxs-lookup"><span data-stu-id="bc4be-116">Int32</span></span>|<span data-ttu-id="bc4be-117">包含 OS 版本的恶意软件的设备计数</span><span class="sxs-lookup"><span data-stu-id="bc4be-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="bc4be-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="bc4be-118">lastUpdateDateTime</span></span>|<span data-ttu-id="bc4be-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc4be-119">DateTimeOffset</span></span>|<span data-ttu-id="bc4be-120">以 UTC 表示的设备计数的最后更新的时间戳</span><span class="sxs-lookup"><span data-stu-id="bc4be-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc4be-121">关系</span><span class="sxs-lookup"><span data-stu-id="bc4be-121">Relationships</span></span>
<span data-ttu-id="bc4be-122">无</span><span class="sxs-lookup"><span data-stu-id="bc4be-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc4be-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc4be-123">JSON Representation</span></span>
<span data-ttu-id="bc4be-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc4be-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```






