---
title: iosAvailableUpdateVersion 资源类型
description: iOS 可用的更新版本详细信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3997ce86c780713849d0e0e4773457ff665b0e0d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255600"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="ea1c9-103">iosAvailableUpdateVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea1c9-103">iosAvailableUpdateVersion resource type</span></span>

<span data-ttu-id="ea1c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea1c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea1c9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea1c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea1c9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea1c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea1c9-107">iOS 可用的更新版本详细信息</span><span class="sxs-lookup"><span data-stu-id="ea1c9-107">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="ea1c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea1c9-108">Properties</span></span>
|<span data-ttu-id="ea1c9-109">属性</span><span class="sxs-lookup"><span data-stu-id="ea1c9-109">Property</span></span>|<span data-ttu-id="ea1c9-110">类型</span><span class="sxs-lookup"><span data-stu-id="ea1c9-110">Type</span></span>|<span data-ttu-id="ea1c9-111">描述</span><span class="sxs-lookup"><span data-stu-id="ea1c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea1c9-112">productVersion</span><span class="sxs-lookup"><span data-stu-id="ea1c9-112">productVersion</span></span>|<span data-ttu-id="ea1c9-113">String</span><span class="sxs-lookup"><span data-stu-id="ea1c9-113">String</span></span>|<span data-ttu-id="ea1c9-114">更新的版本。</span><span class="sxs-lookup"><span data-stu-id="ea1c9-114">The version of the update.</span></span>|
|<span data-ttu-id="ea1c9-115">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="ea1c9-115">postingDateTime</span></span>|<span data-ttu-id="ea1c9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea1c9-116">DateTimeOffset</span></span>|<span data-ttu-id="ea1c9-117">更新的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="ea1c9-117">The posting date of the update.</span></span>|
|<span data-ttu-id="ea1c9-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ea1c9-118">expirationDateTime</span></span>|<span data-ttu-id="ea1c9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea1c9-119">DateTimeOffset</span></span>|<span data-ttu-id="ea1c9-120">更新的到期日期。</span><span class="sxs-lookup"><span data-stu-id="ea1c9-120">The expiration date of the update.</span></span>|
|<span data-ttu-id="ea1c9-121">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="ea1c9-121">supportedDevices</span></span>|<span data-ttu-id="ea1c9-122">String 集合</span><span class="sxs-lookup"><span data-stu-id="ea1c9-122">String collection</span></span>|<span data-ttu-id="ea1c9-123">更新支持的设备的列表。</span><span class="sxs-lookup"><span data-stu-id="ea1c9-123">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea1c9-124">关系</span><span class="sxs-lookup"><span data-stu-id="ea1c9-124">Relationships</span></span>
<span data-ttu-id="ea1c9-125">无</span><span class="sxs-lookup"><span data-stu-id="ea1c9-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea1c9-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea1c9-126">JSON Representation</span></span>
<span data-ttu-id="ea1c9-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea1c9-127">Here is a JSON representation of the resource.</span></span>
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




