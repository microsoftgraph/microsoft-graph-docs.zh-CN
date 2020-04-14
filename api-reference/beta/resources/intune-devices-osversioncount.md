---
title: osVersionCount 资源类型
description: 包含每个 OS 版本的包含恶意软件的设备的计数
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b727be90c5fab9966b4a81179c8c9fa65279e0a2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443861"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="81012-103">osVersionCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="81012-103">osVersionCount resource type</span></span>

<span data-ttu-id="81012-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81012-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81012-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81012-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81012-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81012-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81012-107">包含每个 OS 版本的包含恶意软件的设备的计数</span><span class="sxs-lookup"><span data-stu-id="81012-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="81012-108">属性</span><span class="sxs-lookup"><span data-stu-id="81012-108">Properties</span></span>
|<span data-ttu-id="81012-109">属性</span><span class="sxs-lookup"><span data-stu-id="81012-109">Property</span></span>|<span data-ttu-id="81012-110">类型</span><span class="sxs-lookup"><span data-stu-id="81012-110">Type</span></span>|<span data-ttu-id="81012-111">说明</span><span class="sxs-lookup"><span data-stu-id="81012-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81012-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="81012-112">osVersion</span></span>|<span data-ttu-id="81012-113">String</span><span class="sxs-lookup"><span data-stu-id="81012-113">String</span></span>|<span data-ttu-id="81012-114">OS 版本</span><span class="sxs-lookup"><span data-stu-id="81012-114">OS version</span></span>|
|<span data-ttu-id="81012-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="81012-115">deviceCount</span></span>|<span data-ttu-id="81012-116">Int32</span><span class="sxs-lookup"><span data-stu-id="81012-116">Int32</span></span>|<span data-ttu-id="81012-117">包含 OS 版本的恶意软件的设备计数</span><span class="sxs-lookup"><span data-stu-id="81012-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="81012-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="81012-118">lastUpdateDateTime</span></span>|<span data-ttu-id="81012-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81012-119">DateTimeOffset</span></span>|<span data-ttu-id="81012-120">以 UTC 表示的设备计数的最后更新的时间戳</span><span class="sxs-lookup"><span data-stu-id="81012-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="81012-121">关系</span><span class="sxs-lookup"><span data-stu-id="81012-121">Relationships</span></span>
<span data-ttu-id="81012-122">无</span><span class="sxs-lookup"><span data-stu-id="81012-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81012-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81012-123">JSON Representation</span></span>
<span data-ttu-id="81012-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81012-124">Here is a JSON representation of the resource.</span></span>
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



