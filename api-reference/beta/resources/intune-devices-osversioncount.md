---
title: osVersionCount 资源类型
description: 对每个操作系统版本设备的恶意软件的计数
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbe0d8ac149ad84ba4cd1286fb0f2303cdfb52a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410460"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="3ddeb-103">osVersionCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ddeb-103">osVersionCount resource type</span></span>

> <span data-ttu-id="3ddeb-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3ddeb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3ddeb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ddeb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ddeb-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ddeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ddeb-107">对每个操作系统版本设备的恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="3ddeb-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="3ddeb-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ddeb-108">Properties</span></span>
|<span data-ttu-id="3ddeb-109">属性</span><span class="sxs-lookup"><span data-stu-id="3ddeb-109">Property</span></span>|<span data-ttu-id="3ddeb-110">类型</span><span class="sxs-lookup"><span data-stu-id="3ddeb-110">Type</span></span>|<span data-ttu-id="3ddeb-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ddeb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ddeb-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="3ddeb-112">osVersion</span></span>|<span data-ttu-id="3ddeb-113">String</span><span class="sxs-lookup"><span data-stu-id="3ddeb-113">String</span></span>|<span data-ttu-id="3ddeb-114">操作系统版本</span><span class="sxs-lookup"><span data-stu-id="3ddeb-114">OS version</span></span>|
|<span data-ttu-id="3ddeb-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="3ddeb-115">deviceCount</span></span>|<span data-ttu-id="3ddeb-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3ddeb-116">Int32</span></span>|<span data-ttu-id="3ddeb-117">设备的操作系统版本恶意软件的计数</span><span class="sxs-lookup"><span data-stu-id="3ddeb-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="3ddeb-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="3ddeb-118">lastUpdateDateTime</span></span>|<span data-ttu-id="3ddeb-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ddeb-119">DateTimeOffset</span></span>|<span data-ttu-id="3ddeb-120">上次更新的设备的时间戳计数以 UTC</span><span class="sxs-lookup"><span data-stu-id="3ddeb-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ddeb-121">关系</span><span class="sxs-lookup"><span data-stu-id="3ddeb-121">Relationships</span></span>
<span data-ttu-id="3ddeb-122">无</span><span class="sxs-lookup"><span data-stu-id="3ddeb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ddeb-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ddeb-123">JSON Representation</span></span>
<span data-ttu-id="3ddeb-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ddeb-124">Here is a JSON representation of the resource.</span></span>
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




