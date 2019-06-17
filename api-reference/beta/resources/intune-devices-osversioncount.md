---
title: osVersionCount 资源类型
description: 包含每个 OS 版本的包含恶意软件的设备的计数
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4b8987017012d4db0756fc3d8a78efe99319d68
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963910"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="2dbe9-103">osVersionCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="2dbe9-103">osVersionCount resource type</span></span>

> <span data-ttu-id="2dbe9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2dbe9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dbe9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2dbe9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dbe9-106">包含每个 OS 版本的包含恶意软件的设备的计数</span><span class="sxs-lookup"><span data-stu-id="2dbe9-106">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="2dbe9-107">属性</span><span class="sxs-lookup"><span data-stu-id="2dbe9-107">Properties</span></span>
|<span data-ttu-id="2dbe9-108">属性</span><span class="sxs-lookup"><span data-stu-id="2dbe9-108">Property</span></span>|<span data-ttu-id="2dbe9-109">类型</span><span class="sxs-lookup"><span data-stu-id="2dbe9-109">Type</span></span>|<span data-ttu-id="2dbe9-110">说明</span><span class="sxs-lookup"><span data-stu-id="2dbe9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dbe9-111">osVersion</span><span class="sxs-lookup"><span data-stu-id="2dbe9-111">osVersion</span></span>|<span data-ttu-id="2dbe9-112">String</span><span class="sxs-lookup"><span data-stu-id="2dbe9-112">String</span></span>|<span data-ttu-id="2dbe9-113">OS 版本</span><span class="sxs-lookup"><span data-stu-id="2dbe9-113">OS version</span></span>|
|<span data-ttu-id="2dbe9-114">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2dbe9-114">deviceCount</span></span>|<span data-ttu-id="2dbe9-115">Int32</span><span class="sxs-lookup"><span data-stu-id="2dbe9-115">Int32</span></span>|<span data-ttu-id="2dbe9-116">包含 OS 版本的恶意软件的设备计数</span><span class="sxs-lookup"><span data-stu-id="2dbe9-116">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="2dbe9-117">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2dbe9-117">lastUpdateDateTime</span></span>|<span data-ttu-id="2dbe9-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dbe9-118">DateTimeOffset</span></span>|<span data-ttu-id="2dbe9-119">以 UTC 表示的设备计数的最后更新的时间戳</span><span class="sxs-lookup"><span data-stu-id="2dbe9-119">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dbe9-120">关系</span><span class="sxs-lookup"><span data-stu-id="2dbe9-120">Relationships</span></span>
<span data-ttu-id="2dbe9-121">无</span><span class="sxs-lookup"><span data-stu-id="2dbe9-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dbe9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2dbe9-122">JSON Representation</span></span>
<span data-ttu-id="2dbe9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dbe9-123">Here is a JSON representation of the resource.</span></span>
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





