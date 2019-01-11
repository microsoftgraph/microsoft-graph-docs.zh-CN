---
title: osVersionCount 资源类型
description: 对每个操作系统版本设备的恶意软件的计数
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 227e802de7226d653d68997268c9bf4eac4aa259
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864146"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="9c181-103">osVersionCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c181-103">osVersionCount resource type</span></span>

> <span data-ttu-id="9c181-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9c181-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c181-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9c181-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c181-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9c181-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c181-107">对每个操作系统版本设备的恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="9c181-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="9c181-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c181-108">Properties</span></span>
|<span data-ttu-id="9c181-109">属性</span><span class="sxs-lookup"><span data-stu-id="9c181-109">Property</span></span>|<span data-ttu-id="9c181-110">类型</span><span class="sxs-lookup"><span data-stu-id="9c181-110">Type</span></span>|<span data-ttu-id="9c181-111">Description</span><span class="sxs-lookup"><span data-stu-id="9c181-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c181-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="9c181-112">osVersion</span></span>|<span data-ttu-id="9c181-113">String</span><span class="sxs-lookup"><span data-stu-id="9c181-113">String</span></span>|<span data-ttu-id="9c181-114">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="9c181-114">OS version</span></span>|
|<span data-ttu-id="9c181-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="9c181-115">deviceCount</span></span>|<span data-ttu-id="9c181-116">Int32</span><span class="sxs-lookup"><span data-stu-id="9c181-116">Int32</span></span>|<span data-ttu-id="9c181-117">设备的操作系统版本恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="9c181-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="9c181-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="9c181-118">lastUpdateDateTime</span></span>|<span data-ttu-id="9c181-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c181-119">DateTimeOffset</span></span>|<span data-ttu-id="9c181-120">上次更新的设备的时间戳计数以 UTC</span><span class="sxs-lookup"><span data-stu-id="9c181-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c181-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="9c181-121">Relationships</span></span>
<span data-ttu-id="9c181-122">无</span><span class="sxs-lookup"><span data-stu-id="9c181-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c181-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c181-123">JSON Representation</span></span>
<span data-ttu-id="9c181-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c181-124">Here is a JSON representation of the resource.</span></span>
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





