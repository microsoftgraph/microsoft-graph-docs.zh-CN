---
title: windowsPackageInformation 资源类型
description: 包含为业务应用程序的 Windows 行的程序包信息的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f7f3cd593670e071ae62bdb287bcebeee01d555
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849530"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="7ee0b-103">windowsPackageInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ee0b-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="7ee0b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7ee0b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7ee0b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ee0b-107">包含为业务应用程序的 Windows 行的程序包信息的属性。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="7ee0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ee0b-108">Properties</span></span>
|<span data-ttu-id="7ee0b-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ee0b-109">Property</span></span>|<span data-ttu-id="7ee0b-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ee0b-110">Type</span></span>|<span data-ttu-id="7ee0b-111">Description</span><span class="sxs-lookup"><span data-stu-id="7ee0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ee0b-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="7ee0b-112">applicableArchitecture</span></span>|[<span data-ttu-id="7ee0b-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7ee0b-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7ee0b-114">运行此应用程序可以为其 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="7ee0b-115">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="7ee0b-116">displayName</span><span class="sxs-lookup"><span data-stu-id="7ee0b-116">displayName</span></span>|<span data-ttu-id="7ee0b-117">字符串</span><span class="sxs-lookup"><span data-stu-id="7ee0b-117">String</span></span>|<span data-ttu-id="7ee0b-118">显示名称。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-118">The Display Name.</span></span>|
|<span data-ttu-id="7ee0b-119">identityName</span><span class="sxs-lookup"><span data-stu-id="7ee0b-119">identityName</span></span>|<span data-ttu-id="7ee0b-120">String</span><span class="sxs-lookup"><span data-stu-id="7ee0b-120">String</span></span>|<span data-ttu-id="7ee0b-121">标识名称。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-121">The Identity Name.</span></span>|
|<span data-ttu-id="7ee0b-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="7ee0b-122">identityPublisher</span></span>|<span data-ttu-id="7ee0b-123">字符串</span><span class="sxs-lookup"><span data-stu-id="7ee0b-123">String</span></span>|<span data-ttu-id="7ee0b-124">标识发布者。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="7ee0b-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7ee0b-125">identityResourceIdentifier</span></span>|<span data-ttu-id="7ee0b-126">String</span><span class="sxs-lookup"><span data-stu-id="7ee0b-126">String</span></span>|<span data-ttu-id="7ee0b-127">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="7ee0b-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7ee0b-128">identityVersion</span></span>|<span data-ttu-id="7ee0b-129">String</span><span class="sxs-lookup"><span data-stu-id="7ee0b-129">String</span></span>|<span data-ttu-id="7ee0b-130">标识版本。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-130">The Identity Version.</span></span>|
|<span data-ttu-id="7ee0b-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ee0b-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7ee0b-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7ee0b-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7ee0b-133">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ee0b-134">关系</span><span class="sxs-lookup"><span data-stu-id="7ee0b-134">Relationships</span></span>
<span data-ttu-id="7ee0b-135">无</span><span class="sxs-lookup"><span data-stu-id="7ee0b-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7ee0b-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ee0b-136">JSON Representation</span></span>
<span data-ttu-id="7ee0b-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ee0b-137">Here is a JSON representation of the resource.</span></span>
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





