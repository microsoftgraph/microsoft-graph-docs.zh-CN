---
title: 了 windowspackageinformation 资源类型
description: 包含 Windows 业务线应用程序的包信息的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9a7871a101062e9d835c68f37299d83a8bfb5e8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726554"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="f9fb7-103">了 windowspackageinformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9fb7-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="f9fb7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9fb7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9fb7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9fb7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9fb7-107">包含 Windows 业务线应用程序的包信息的属性。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="f9fb7-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9fb7-108">Properties</span></span>
|<span data-ttu-id="f9fb7-109">属性</span><span class="sxs-lookup"><span data-stu-id="f9fb7-109">Property</span></span>|<span data-ttu-id="f9fb7-110">类型</span><span class="sxs-lookup"><span data-stu-id="f9fb7-110">Type</span></span>|<span data-ttu-id="f9fb7-111">说明</span><span class="sxs-lookup"><span data-stu-id="f9fb7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9fb7-112">将 applicablearchitecture</span><span class="sxs-lookup"><span data-stu-id="f9fb7-112">applicableArchitecture</span></span>|[<span data-ttu-id="f9fb7-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f9fb7-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f9fb7-114">可在其上运行此应用程序的 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="f9fb7-115">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="f9fb7-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f9fb7-116">displayName</span></span>|<span data-ttu-id="f9fb7-117">String</span><span class="sxs-lookup"><span data-stu-id="f9fb7-117">String</span></span>|<span data-ttu-id="f9fb7-118">显示名称。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-118">The Display Name.</span></span>|
|<span data-ttu-id="f9fb7-119">identityName</span><span class="sxs-lookup"><span data-stu-id="f9fb7-119">identityName</span></span>|<span data-ttu-id="f9fb7-120">String</span><span class="sxs-lookup"><span data-stu-id="f9fb7-120">String</span></span>|<span data-ttu-id="f9fb7-121">标识名称。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-121">The Identity Name.</span></span>|
|<span data-ttu-id="f9fb7-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="f9fb7-122">identityPublisher</span></span>|<span data-ttu-id="f9fb7-123">String</span><span class="sxs-lookup"><span data-stu-id="f9fb7-123">String</span></span>|<span data-ttu-id="f9fb7-124">标识发布者。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="f9fb7-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f9fb7-125">identityResourceIdentifier</span></span>|<span data-ttu-id="f9fb7-126">String</span><span class="sxs-lookup"><span data-stu-id="f9fb7-126">String</span></span>|<span data-ttu-id="f9fb7-127">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="f9fb7-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f9fb7-128">identityVersion</span></span>|<span data-ttu-id="f9fb7-129">String</span><span class="sxs-lookup"><span data-stu-id="f9fb7-129">String</span></span>|<span data-ttu-id="f9fb7-130">标识版本。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-130">The Identity Version.</span></span>|
|<span data-ttu-id="f9fb7-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f9fb7-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f9fb7-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f9fb7-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f9fb7-133">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9fb7-134">关系</span><span class="sxs-lookup"><span data-stu-id="f9fb7-134">Relationships</span></span>
<span data-ttu-id="f9fb7-135">无</span><span class="sxs-lookup"><span data-stu-id="f9fb7-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9fb7-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9fb7-136">JSON Representation</span></span>
<span data-ttu-id="f9fb7-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9fb7-137">Here is a JSON representation of the resource.</span></span>
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





