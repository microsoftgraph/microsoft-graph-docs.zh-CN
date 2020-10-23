---
title: iosAvailableUpdateVersion 资源类型
description: iOS 可用的更新版本详细信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f2b94a098c70b6d4ac4105b31274f406f058c675
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696046"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="0d946-103">iosAvailableUpdateVersion 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d946-103">iosAvailableUpdateVersion resource type</span></span>

<span data-ttu-id="0d946-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d946-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d946-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d946-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d946-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d946-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d946-107">iOS 可用的更新版本详细信息</span><span class="sxs-lookup"><span data-stu-id="0d946-107">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="0d946-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d946-108">Properties</span></span>
|<span data-ttu-id="0d946-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d946-109">Property</span></span>|<span data-ttu-id="0d946-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d946-110">Type</span></span>|<span data-ttu-id="0d946-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d946-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d946-112">productVersion</span><span class="sxs-lookup"><span data-stu-id="0d946-112">productVersion</span></span>|<span data-ttu-id="0d946-113">String</span><span class="sxs-lookup"><span data-stu-id="0d946-113">String</span></span>|<span data-ttu-id="0d946-114">更新的版本。</span><span class="sxs-lookup"><span data-stu-id="0d946-114">The version of the update.</span></span>|
|<span data-ttu-id="0d946-115">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="0d946-115">postingDateTime</span></span>|<span data-ttu-id="0d946-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d946-116">DateTimeOffset</span></span>|<span data-ttu-id="0d946-117">更新的过帐日期。</span><span class="sxs-lookup"><span data-stu-id="0d946-117">The posting date of the update.</span></span>|
|<span data-ttu-id="0d946-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0d946-118">expirationDateTime</span></span>|<span data-ttu-id="0d946-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d946-119">DateTimeOffset</span></span>|<span data-ttu-id="0d946-120">更新的到期日期。</span><span class="sxs-lookup"><span data-stu-id="0d946-120">The expiration date of the update.</span></span>|
|<span data-ttu-id="0d946-121">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="0d946-121">supportedDevices</span></span>|<span data-ttu-id="0d946-122">String collection</span><span class="sxs-lookup"><span data-stu-id="0d946-122">String collection</span></span>|<span data-ttu-id="0d946-123">更新支持的设备的列表。</span><span class="sxs-lookup"><span data-stu-id="0d946-123">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d946-124">关系</span><span class="sxs-lookup"><span data-stu-id="0d946-124">Relationships</span></span>
<span data-ttu-id="0d946-125">无</span><span class="sxs-lookup"><span data-stu-id="0d946-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d946-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d946-126">JSON Representation</span></span>
<span data-ttu-id="0d946-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d946-127">Here is a JSON representation of the resource.</span></span>
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





