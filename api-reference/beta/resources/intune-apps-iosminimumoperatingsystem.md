---
title: iosMinimumOperatingSystem 资源类型
description: 包含 iOS 移动应用需要的最低操作系统的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 43409d7c4f4eb7bedd4a169c5f56d969e2b9d03d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005938"
---
# <a name="iosminimumoperatingsystem-resource-type"></a><span data-ttu-id="d233a-103">iosMinimumOperatingSystem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d233a-103">iosMinimumOperatingSystem resource type</span></span>

> <span data-ttu-id="d233a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d233a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d233a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d233a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d233a-106">包含 iOS 移动应用需要的最低操作系统的属性。</span><span class="sxs-lookup"><span data-stu-id="d233a-106">Contains properties of the minimum operating system required for an iOS mobile app.</span></span>

## <a name="properties"></a><span data-ttu-id="d233a-107">属性</span><span class="sxs-lookup"><span data-stu-id="d233a-107">Properties</span></span>
|<span data-ttu-id="d233a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d233a-108">Property</span></span>|<span data-ttu-id="d233a-109">类型</span><span class="sxs-lookup"><span data-stu-id="d233a-109">Type</span></span>|<span data-ttu-id="d233a-110">说明</span><span class="sxs-lookup"><span data-stu-id="d233a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d233a-111">v8_0</span><span class="sxs-lookup"><span data-stu-id="d233a-111">v8_0</span></span>|<span data-ttu-id="d233a-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d233a-112">Boolean</span></span>|<span data-ttu-id="d233a-113">版本 8.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="d233a-113">Version 8.0 or later.</span></span>|
|<span data-ttu-id="d233a-114">v9_0</span><span class="sxs-lookup"><span data-stu-id="d233a-114">v9_0</span></span>|<span data-ttu-id="d233a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d233a-115">Boolean</span></span>|<span data-ttu-id="d233a-116">版本 9.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="d233a-116">Version 9.0 or later.</span></span>|
|<span data-ttu-id="d233a-117">v10_0</span><span class="sxs-lookup"><span data-stu-id="d233a-117">v10_0</span></span>|<span data-ttu-id="d233a-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d233a-118">Boolean</span></span>|<span data-ttu-id="d233a-119">版本 10.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="d233a-119">Version 10.0 or later.</span></span>|
|<span data-ttu-id="d233a-120">v11_0</span><span class="sxs-lookup"><span data-stu-id="d233a-120">v11_0</span></span>|<span data-ttu-id="d233a-121">布尔值</span><span class="sxs-lookup"><span data-stu-id="d233a-121">Boolean</span></span>|<span data-ttu-id="d233a-122">版本 11.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="d233a-122">Version 11.0 or later.</span></span>|
|<span data-ttu-id="d233a-123">v12_0</span><span class="sxs-lookup"><span data-stu-id="d233a-123">v12_0</span></span>|<span data-ttu-id="d233a-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="d233a-124">Boolean</span></span>|<span data-ttu-id="d233a-125">版本12.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="d233a-125">Version 12.0 or later.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d233a-126">关系</span><span class="sxs-lookup"><span data-stu-id="d233a-126">Relationships</span></span>
<span data-ttu-id="d233a-127">无</span><span class="sxs-lookup"><span data-stu-id="d233a-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d233a-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d233a-128">JSON Representation</span></span>
<span data-ttu-id="d233a-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d233a-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMinimumOperatingSystem",
  "v8_0": true,
  "v9_0": true,
  "v10_0": true,
  "v11_0": true,
  "v12_0": true
}
```





