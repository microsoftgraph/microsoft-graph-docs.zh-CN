---
title: windowsPackageInformation 资源类型
description: 包含为业务应用程序的 Windows 行的程序包信息的属性。
ms.openlocfilehash: a7676320d5aa2eeab1140e6cc631c4061d2c5d14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045888"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="b0904-103">windowsPackageInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b0904-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="b0904-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b0904-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0904-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b0904-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0904-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b0904-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0904-107">包含为业务应用程序的 Windows 行的程序包信息的属性。</span><span class="sxs-lookup"><span data-stu-id="b0904-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="b0904-108">属性</span><span class="sxs-lookup"><span data-stu-id="b0904-108">Properties</span></span>
|<span data-ttu-id="b0904-109">属性</span><span class="sxs-lookup"><span data-stu-id="b0904-109">Property</span></span>|<span data-ttu-id="b0904-110">类型</span><span class="sxs-lookup"><span data-stu-id="b0904-110">Type</span></span>|<span data-ttu-id="b0904-111">说明</span><span class="sxs-lookup"><span data-stu-id="b0904-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0904-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="b0904-112">applicableArchitecture</span></span>|[<span data-ttu-id="b0904-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b0904-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b0904-114">运行此应用程序可以为其 Windows 体系结构。</span><span class="sxs-lookup"><span data-stu-id="b0904-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="b0904-115">可取值为：`none`、`x86`、`x64`、`arm`、`neutral`。</span><span class="sxs-lookup"><span data-stu-id="b0904-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="b0904-116">displayName</span><span class="sxs-lookup"><span data-stu-id="b0904-116">displayName</span></span>|<span data-ttu-id="b0904-117">字符串</span><span class="sxs-lookup"><span data-stu-id="b0904-117">String</span></span>|<span data-ttu-id="b0904-118">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b0904-118">The Display Name.</span></span>|
|<span data-ttu-id="b0904-119">identityName</span><span class="sxs-lookup"><span data-stu-id="b0904-119">identityName</span></span>|<span data-ttu-id="b0904-120">String</span><span class="sxs-lookup"><span data-stu-id="b0904-120">String</span></span>|<span data-ttu-id="b0904-121">标识名称。</span><span class="sxs-lookup"><span data-stu-id="b0904-121">The Identity Name.</span></span>|
|<span data-ttu-id="b0904-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="b0904-122">identityPublisher</span></span>|<span data-ttu-id="b0904-123">字符串</span><span class="sxs-lookup"><span data-stu-id="b0904-123">String</span></span>|<span data-ttu-id="b0904-124">标识发布者。</span><span class="sxs-lookup"><span data-stu-id="b0904-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="b0904-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0904-125">identityResourceIdentifier</span></span>|<span data-ttu-id="b0904-126">String</span><span class="sxs-lookup"><span data-stu-id="b0904-126">String</span></span>|<span data-ttu-id="b0904-127">标识资源标识符。</span><span class="sxs-lookup"><span data-stu-id="b0904-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="b0904-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b0904-128">identityVersion</span></span>|<span data-ttu-id="b0904-129">String</span><span class="sxs-lookup"><span data-stu-id="b0904-129">String</span></span>|<span data-ttu-id="b0904-130">标识版本。</span><span class="sxs-lookup"><span data-stu-id="b0904-130">The Identity Version.</span></span>|
|<span data-ttu-id="b0904-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b0904-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b0904-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b0904-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b0904-133">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="b0904-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0904-134">关系</span><span class="sxs-lookup"><span data-stu-id="b0904-134">Relationships</span></span>
<span data-ttu-id="b0904-135">无</span><span class="sxs-lookup"><span data-stu-id="b0904-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0904-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b0904-136">JSON Representation</span></span>
<span data-ttu-id="b0904-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0904-137">Here is a JSON representation of the resource.</span></span>
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





