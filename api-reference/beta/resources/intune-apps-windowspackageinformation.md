---
title: 了 windowspackageinformation 资源类型
description: 包含 Windows 业务线应用程序的包信息的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e1dda51d5c98cb27ab9e71c7bef9167959c9052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558235"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="176bd-103">了 windowspackageinformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="176bd-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="176bd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="176bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="176bd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="176bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="176bd-106">包含 Windows 业务线应用程序的包信息的属性。</span><span class="sxs-lookup"><span data-stu-id="176bd-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="176bd-107">属性</span><span class="sxs-lookup"><span data-stu-id="176bd-107">Properties</span></span>
|<span data-ttu-id="176bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="176bd-108">Property</span></span>|<span data-ttu-id="176bd-109">类型</span><span class="sxs-lookup"><span data-stu-id="176bd-109">Type</span></span>|<span data-ttu-id="176bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="176bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="176bd-111">将 applicablearchitecture</span><span class="sxs-lookup"><span data-stu-id="176bd-111">applicableArchitecture</span></span>|[<span data-ttu-id="176bd-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="176bd-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="176bd-113">可在其上运行此应用程序的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="176bd-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="176bd-114">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="176bd-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="176bd-115">displayName</span><span class="sxs-lookup"><span data-stu-id="176bd-115">displayName</span></span>|<span data-ttu-id="176bd-116">String</span><span class="sxs-lookup"><span data-stu-id="176bd-116">String</span></span>|<span data-ttu-id="176bd-117">显示名称。</span><span class="sxs-lookup"><span data-stu-id="176bd-117">The Display Name.</span></span>|
|<span data-ttu-id="176bd-118">identityName</span><span class="sxs-lookup"><span data-stu-id="176bd-118">identityName</span></span>|<span data-ttu-id="176bd-119">String</span><span class="sxs-lookup"><span data-stu-id="176bd-119">String</span></span>|<span data-ttu-id="176bd-120">标识名称。</span><span class="sxs-lookup"><span data-stu-id="176bd-120">The Identity Name.</span></span>|
|<span data-ttu-id="176bd-121">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="176bd-121">identityPublisher</span></span>|<span data-ttu-id="176bd-122">String</span><span class="sxs-lookup"><span data-stu-id="176bd-122">String</span></span>|<span data-ttu-id="176bd-123">标识发布者。</span><span class="sxs-lookup"><span data-stu-id="176bd-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="176bd-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="176bd-124">identityResourceIdentifier</span></span>|<span data-ttu-id="176bd-125">String</span><span class="sxs-lookup"><span data-stu-id="176bd-125">String</span></span>|<span data-ttu-id="176bd-126">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="176bd-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="176bd-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="176bd-127">identityVersion</span></span>|<span data-ttu-id="176bd-128">String</span><span class="sxs-lookup"><span data-stu-id="176bd-128">String</span></span>|<span data-ttu-id="176bd-129">标识版本。</span><span class="sxs-lookup"><span data-stu-id="176bd-129">The Identity Version.</span></span>|
|<span data-ttu-id="176bd-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="176bd-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="176bd-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="176bd-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="176bd-132">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="176bd-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="176bd-133">关系</span><span class="sxs-lookup"><span data-stu-id="176bd-133">Relationships</span></span>
<span data-ttu-id="176bd-134">无</span><span class="sxs-lookup"><span data-stu-id="176bd-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="176bd-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="176bd-135">JSON Representation</span></span>
<span data-ttu-id="176bd-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="176bd-136">Here is a JSON representation of the resource.</span></span>
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





