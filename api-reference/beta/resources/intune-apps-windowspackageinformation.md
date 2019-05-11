---
title: 了 windowspackageinformation 资源类型
description: 包含 Windows 业务线应用程序的包信息的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2803779830d0e2bb88a0a91a96abfc101d15cb66
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949498"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="37a4d-103">了 windowspackageinformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="37a4d-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="37a4d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37a4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37a4d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37a4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37a4d-106">包含 Windows 业务线应用程序的包信息的属性。</span><span class="sxs-lookup"><span data-stu-id="37a4d-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="37a4d-107">属性</span><span class="sxs-lookup"><span data-stu-id="37a4d-107">Properties</span></span>
|<span data-ttu-id="37a4d-108">属性</span><span class="sxs-lookup"><span data-stu-id="37a4d-108">Property</span></span>|<span data-ttu-id="37a4d-109">类型</span><span class="sxs-lookup"><span data-stu-id="37a4d-109">Type</span></span>|<span data-ttu-id="37a4d-110">说明</span><span class="sxs-lookup"><span data-stu-id="37a4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37a4d-111">将 applicablearchitecture</span><span class="sxs-lookup"><span data-stu-id="37a4d-111">applicableArchitecture</span></span>|[<span data-ttu-id="37a4d-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="37a4d-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="37a4d-113">可在其上运行此应用程序的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="37a4d-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="37a4d-114">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="37a4d-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="37a4d-115">displayName</span><span class="sxs-lookup"><span data-stu-id="37a4d-115">displayName</span></span>|<span data-ttu-id="37a4d-116">String</span><span class="sxs-lookup"><span data-stu-id="37a4d-116">String</span></span>|<span data-ttu-id="37a4d-117">显示名称。</span><span class="sxs-lookup"><span data-stu-id="37a4d-117">The Display Name.</span></span>|
|<span data-ttu-id="37a4d-118">identityName</span><span class="sxs-lookup"><span data-stu-id="37a4d-118">identityName</span></span>|<span data-ttu-id="37a4d-119">String</span><span class="sxs-lookup"><span data-stu-id="37a4d-119">String</span></span>|<span data-ttu-id="37a4d-120">标识名称。</span><span class="sxs-lookup"><span data-stu-id="37a4d-120">The Identity Name.</span></span>|
|<span data-ttu-id="37a4d-121">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="37a4d-121">identityPublisher</span></span>|<span data-ttu-id="37a4d-122">String</span><span class="sxs-lookup"><span data-stu-id="37a4d-122">String</span></span>|<span data-ttu-id="37a4d-123">标识发布者。</span><span class="sxs-lookup"><span data-stu-id="37a4d-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="37a4d-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="37a4d-124">identityResourceIdentifier</span></span>|<span data-ttu-id="37a4d-125">String</span><span class="sxs-lookup"><span data-stu-id="37a4d-125">String</span></span>|<span data-ttu-id="37a4d-126">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="37a4d-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="37a4d-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="37a4d-127">identityVersion</span></span>|<span data-ttu-id="37a4d-128">String</span><span class="sxs-lookup"><span data-stu-id="37a4d-128">String</span></span>|<span data-ttu-id="37a4d-129">标识版本。</span><span class="sxs-lookup"><span data-stu-id="37a4d-129">The Identity Version.</span></span>|
|<span data-ttu-id="37a4d-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="37a4d-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="37a4d-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="37a4d-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="37a4d-132">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="37a4d-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37a4d-133">关系</span><span class="sxs-lookup"><span data-stu-id="37a4d-133">Relationships</span></span>
<span data-ttu-id="37a4d-134">无</span><span class="sxs-lookup"><span data-stu-id="37a4d-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37a4d-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37a4d-135">JSON Representation</span></span>
<span data-ttu-id="37a4d-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37a4d-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  }
}
```




