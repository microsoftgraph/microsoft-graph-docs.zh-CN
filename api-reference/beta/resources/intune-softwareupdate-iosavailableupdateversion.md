---
title: iosAvailableUpdateVersion 资源类型
description: iOS 可用的更新版本详细信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2113f8ddf34c87be6554bc29d7220881e8c634f6
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160888"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="40f6b-103">iosAvailableUpdateVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="40f6b-103">iosAvailableUpdateVersion resource type</span></span>

> <span data-ttu-id="40f6b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40f6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40f6b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40f6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40f6b-106">iOS 可用的更新版本详细信息</span><span class="sxs-lookup"><span data-stu-id="40f6b-106">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="40f6b-107">属性</span><span class="sxs-lookup"><span data-stu-id="40f6b-107">Properties</span></span>
|<span data-ttu-id="40f6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="40f6b-108">Property</span></span>|<span data-ttu-id="40f6b-109">类型</span><span class="sxs-lookup"><span data-stu-id="40f6b-109">Type</span></span>|<span data-ttu-id="40f6b-110">说明</span><span class="sxs-lookup"><span data-stu-id="40f6b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40f6b-111">productVersion</span><span class="sxs-lookup"><span data-stu-id="40f6b-111">productVersion</span></span>|<span data-ttu-id="40f6b-112">String</span><span class="sxs-lookup"><span data-stu-id="40f6b-112">String</span></span>|<span data-ttu-id="40f6b-113">更新的版本。</span><span class="sxs-lookup"><span data-stu-id="40f6b-113">The version of the update.</span></span>|
|<span data-ttu-id="40f6b-114">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="40f6b-114">postingDateTime</span></span>|<span data-ttu-id="40f6b-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40f6b-115">DateTimeOffset</span></span>|<span data-ttu-id="40f6b-116">更新的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="40f6b-116">The posting date of the update.</span></span>|
|<span data-ttu-id="40f6b-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="40f6b-117">expirationDateTime</span></span>|<span data-ttu-id="40f6b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40f6b-118">DateTimeOffset</span></span>|<span data-ttu-id="40f6b-119">更新的到期日期。</span><span class="sxs-lookup"><span data-stu-id="40f6b-119">The expiration date of the update.</span></span>|
|<span data-ttu-id="40f6b-120">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="40f6b-120">supportedDevices</span></span>|<span data-ttu-id="40f6b-121">String collection</span><span class="sxs-lookup"><span data-stu-id="40f6b-121">String collection</span></span>|<span data-ttu-id="40f6b-122">更新支持的设备的列表。</span><span class="sxs-lookup"><span data-stu-id="40f6b-122">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40f6b-123">关系</span><span class="sxs-lookup"><span data-stu-id="40f6b-123">Relationships</span></span>
<span data-ttu-id="40f6b-124">无</span><span class="sxs-lookup"><span data-stu-id="40f6b-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40f6b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40f6b-125">JSON Representation</span></span>
<span data-ttu-id="40f6b-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40f6b-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```



