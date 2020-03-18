---
title: 了 windowspackageinformation 资源类型
description: 包含 Windows 业务线应用程序的包信息的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 31c99e8732f100e7d4797fda7d4c71a5086bd227
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797491"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="4f5a5-103">了 windowspackageinformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4f5a5-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="4f5a5-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f5a5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f5a5-106">包含 Windows 业务线应用程序的包信息的属性。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="4f5a5-107">属性</span><span class="sxs-lookup"><span data-stu-id="4f5a5-107">Properties</span></span>
|<span data-ttu-id="4f5a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="4f5a5-108">Property</span></span>|<span data-ttu-id="4f5a5-109">类型</span><span class="sxs-lookup"><span data-stu-id="4f5a5-109">Type</span></span>|<span data-ttu-id="4f5a5-110">说明</span><span class="sxs-lookup"><span data-stu-id="4f5a5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f5a5-111">将 applicablearchitecture</span><span class="sxs-lookup"><span data-stu-id="4f5a5-111">applicableArchitecture</span></span>|[<span data-ttu-id="4f5a5-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="4f5a5-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="4f5a5-113">可在其上运行此应用程序的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="4f5a5-114">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="4f5a5-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4f5a5-115">displayName</span></span>|<span data-ttu-id="4f5a5-116">String</span><span class="sxs-lookup"><span data-stu-id="4f5a5-116">String</span></span>|<span data-ttu-id="4f5a5-117">显示名称。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-117">The Display Name.</span></span>|
|<span data-ttu-id="4f5a5-118">identityName</span><span class="sxs-lookup"><span data-stu-id="4f5a5-118">identityName</span></span>|<span data-ttu-id="4f5a5-119">String</span><span class="sxs-lookup"><span data-stu-id="4f5a5-119">String</span></span>|<span data-ttu-id="4f5a5-120">标识名称。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-120">The Identity Name.</span></span>|
|<span data-ttu-id="4f5a5-121">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="4f5a5-121">identityPublisher</span></span>|<span data-ttu-id="4f5a5-122">String</span><span class="sxs-lookup"><span data-stu-id="4f5a5-122">String</span></span>|<span data-ttu-id="4f5a5-123">标识发布者。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="4f5a5-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="4f5a5-124">identityResourceIdentifier</span></span>|<span data-ttu-id="4f5a5-125">String</span><span class="sxs-lookup"><span data-stu-id="4f5a5-125">String</span></span>|<span data-ttu-id="4f5a5-126">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="4f5a5-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="4f5a5-127">identityVersion</span></span>|<span data-ttu-id="4f5a5-128">String</span><span class="sxs-lookup"><span data-stu-id="4f5a5-128">String</span></span>|<span data-ttu-id="4f5a5-129">标识版本。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-129">The Identity Version.</span></span>|
|<span data-ttu-id="4f5a5-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f5a5-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4f5a5-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4f5a5-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="4f5a5-132">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f5a5-133">关系</span><span class="sxs-lookup"><span data-stu-id="4f5a5-133">Relationships</span></span>
<span data-ttu-id="4f5a5-134">无</span><span class="sxs-lookup"><span data-stu-id="4f5a5-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f5a5-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4f5a5-135">JSON Representation</span></span>
<span data-ttu-id="4f5a5-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f5a5-136">Here is a JSON representation of the resource.</span></span>
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
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  }
}
```



