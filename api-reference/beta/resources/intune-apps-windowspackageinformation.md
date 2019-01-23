---
title: windowsPackageInformation 资源类型
description: 包含为业务应用程序的 Windows 行的程序包信息的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 112d84c5bae889e24b889b4598d61a6b3d63db50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403278"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="96875-103">windowsPackageInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="96875-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="96875-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="96875-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="96875-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="96875-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96875-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96875-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96875-107">包含为业务应用程序的 Windows 行的程序包信息的属性。</span><span class="sxs-lookup"><span data-stu-id="96875-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="96875-108">属性</span><span class="sxs-lookup"><span data-stu-id="96875-108">Properties</span></span>
|<span data-ttu-id="96875-109">属性</span><span class="sxs-lookup"><span data-stu-id="96875-109">Property</span></span>|<span data-ttu-id="96875-110">类型</span><span class="sxs-lookup"><span data-stu-id="96875-110">Type</span></span>|<span data-ttu-id="96875-111">说明</span><span class="sxs-lookup"><span data-stu-id="96875-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96875-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="96875-112">applicableArchitecture</span></span>|[<span data-ttu-id="96875-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="96875-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="96875-114">运行此应用程序可以为其 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="96875-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="96875-115">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="96875-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="96875-116">displayName</span><span class="sxs-lookup"><span data-stu-id="96875-116">displayName</span></span>|<span data-ttu-id="96875-117">String</span><span class="sxs-lookup"><span data-stu-id="96875-117">String</span></span>|<span data-ttu-id="96875-118">显示名称。</span><span class="sxs-lookup"><span data-stu-id="96875-118">The Display Name.</span></span>|
|<span data-ttu-id="96875-119">identityName</span><span class="sxs-lookup"><span data-stu-id="96875-119">identityName</span></span>|<span data-ttu-id="96875-120">String</span><span class="sxs-lookup"><span data-stu-id="96875-120">String</span></span>|<span data-ttu-id="96875-121">标识名称。</span><span class="sxs-lookup"><span data-stu-id="96875-121">The Identity Name.</span></span>|
|<span data-ttu-id="96875-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="96875-122">identityPublisher</span></span>|<span data-ttu-id="96875-123">String</span><span class="sxs-lookup"><span data-stu-id="96875-123">String</span></span>|<span data-ttu-id="96875-124">标识发布者。</span><span class="sxs-lookup"><span data-stu-id="96875-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="96875-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="96875-125">identityResourceIdentifier</span></span>|<span data-ttu-id="96875-126">String</span><span class="sxs-lookup"><span data-stu-id="96875-126">String</span></span>|<span data-ttu-id="96875-127">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="96875-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="96875-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="96875-128">identityVersion</span></span>|<span data-ttu-id="96875-129">String</span><span class="sxs-lookup"><span data-stu-id="96875-129">String</span></span>|<span data-ttu-id="96875-130">标识版本。</span><span class="sxs-lookup"><span data-stu-id="96875-130">The Identity Version.</span></span>|
|<span data-ttu-id="96875-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="96875-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="96875-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="96875-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="96875-133">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="96875-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96875-134">关系</span><span class="sxs-lookup"><span data-stu-id="96875-134">Relationships</span></span>
<span data-ttu-id="96875-135">无</span><span class="sxs-lookup"><span data-stu-id="96875-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96875-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96875-136">JSON Representation</span></span>
<span data-ttu-id="96875-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96875-137">Here is a JSON representation of the resource.</span></span>
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




