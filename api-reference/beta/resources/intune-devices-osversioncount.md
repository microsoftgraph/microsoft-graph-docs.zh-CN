---
title: osVersionCount 资源类型
description: 对每个操作系统版本设备的恶意软件的计数
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: de841e679ede22492d26f2a1587e775179c45761
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911838"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="5a1bf-103">osVersionCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a1bf-103">osVersionCount resource type</span></span>

> <span data-ttu-id="5a1bf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a1bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a1bf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a1bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a1bf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5a1bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a1bf-107">对每个操作系统版本设备的恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="5a1bf-107">Count of devices with malware for each OS version</span></span>
## <a name="properties"></a><span data-ttu-id="5a1bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a1bf-108">Properties</span></span>
|<span data-ttu-id="5a1bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="5a1bf-109">Property</span></span>|<span data-ttu-id="5a1bf-110">类型</span><span class="sxs-lookup"><span data-stu-id="5a1bf-110">Type</span></span>|<span data-ttu-id="5a1bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="5a1bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a1bf-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="5a1bf-112">osVersion</span></span>|<span data-ttu-id="5a1bf-113">String</span><span class="sxs-lookup"><span data-stu-id="5a1bf-113">String</span></span>|<span data-ttu-id="5a1bf-114">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="5a1bf-114">OS version</span></span>|
|<span data-ttu-id="5a1bf-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5a1bf-115">deviceCount</span></span>|<span data-ttu-id="5a1bf-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5a1bf-116">Int32</span></span>|<span data-ttu-id="5a1bf-117">设备的操作系统版本恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="5a1bf-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="5a1bf-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="5a1bf-118">lastUpdateDateTime</span></span>|<span data-ttu-id="5a1bf-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a1bf-119">DateTimeOffset</span></span>|<span data-ttu-id="5a1bf-120">上次更新的设备的时间戳计数以 UTC</span><span class="sxs-lookup"><span data-stu-id="5a1bf-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a1bf-121">Relationships</span><span class="sxs-lookup"><span data-stu-id="5a1bf-121">Relationships</span></span>
<span data-ttu-id="5a1bf-122">无</span><span class="sxs-lookup"><span data-stu-id="5a1bf-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a1bf-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a1bf-123">JSON Representation</span></span>
<span data-ttu-id="5a1bf-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a1bf-124">Here is a JSON representation of the resource.</span></span>
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





