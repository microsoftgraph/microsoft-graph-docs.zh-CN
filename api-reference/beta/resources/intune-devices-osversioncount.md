---
title: osVersionCount 资源类型
description: 包含每个 OS 版本的包含恶意软件的设备的计数
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9302a9604c10db0f462eac1de2caab42a933588
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372529"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="77f8a-103">osVersionCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="77f8a-103">osVersionCount resource type</span></span>

> <span data-ttu-id="77f8a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="77f8a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77f8a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77f8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77f8a-106">包含每个 OS 版本的包含恶意软件的设备的计数</span><span class="sxs-lookup"><span data-stu-id="77f8a-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="77f8a-107">属性</span><span class="sxs-lookup"><span data-stu-id="77f8a-107">Properties</span></span>
|<span data-ttu-id="77f8a-108">属性</span><span class="sxs-lookup"><span data-stu-id="77f8a-108">Property</span></span>|<span data-ttu-id="77f8a-109">类型</span><span class="sxs-lookup"><span data-stu-id="77f8a-109">Type</span></span>|<span data-ttu-id="77f8a-110">说明</span><span class="sxs-lookup"><span data-stu-id="77f8a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77f8a-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="77f8a-111">osVersion</span></span>|<span data-ttu-id="77f8a-112">String</span><span class="sxs-lookup"><span data-stu-id="77f8a-112">String</span></span>|<span data-ttu-id="77f8a-113">OS 版本</span><span class="sxs-lookup"><span data-stu-id="77f8a-113">OS version</span></span>|
|<span data-ttu-id="77f8a-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="77f8a-114">deviceCount</span></span>|<span data-ttu-id="77f8a-115">Int32</span><span class="sxs-lookup"><span data-stu-id="77f8a-115">Int32</span></span>|<span data-ttu-id="77f8a-116">包含 OS 版本的恶意软件的设备计数</span><span class="sxs-lookup"><span data-stu-id="77f8a-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="77f8a-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="77f8a-117">lastUpdateDateTime</span></span>|<span data-ttu-id="77f8a-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77f8a-118">DateTimeOffset</span></span>|<span data-ttu-id="77f8a-119">以 UTC 表示的设备计数的最后更新的时间戳</span><span class="sxs-lookup"><span data-stu-id="77f8a-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="77f8a-120">关系</span><span class="sxs-lookup"><span data-stu-id="77f8a-120">Relationships</span></span>
<span data-ttu-id="77f8a-121">无</span><span class="sxs-lookup"><span data-stu-id="77f8a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77f8a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77f8a-122">JSON Representation</span></span>
<span data-ttu-id="77f8a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77f8a-123">Here is a JSON representation of the resource.</span></span>
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



