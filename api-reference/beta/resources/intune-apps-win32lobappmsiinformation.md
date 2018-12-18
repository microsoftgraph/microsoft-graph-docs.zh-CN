---
title: win32LobAppMsiInformation 资源类型
description: Win32 应用程序包含 MSI 应用程序的属性。
author: tfitzmac
ms.openlocfilehash: 1753df68ab1f4b0e1649c16a4a7fa0ad49941bf9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326136"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="fbbc8-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="fbbc8-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="fbbc8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fbbc8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fbbc8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fbbc8-107">Win32 应用程序包含 MSI 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="fbbc8-108">属性</span><span class="sxs-lookup"><span data-stu-id="fbbc8-108">Properties</span></span>
|<span data-ttu-id="fbbc8-109">属性</span><span class="sxs-lookup"><span data-stu-id="fbbc8-109">Property</span></span>|<span data-ttu-id="fbbc8-110">类型</span><span class="sxs-lookup"><span data-stu-id="fbbc8-110">Type</span></span>|<span data-ttu-id="fbbc8-111">说明</span><span class="sxs-lookup"><span data-stu-id="fbbc8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbbc8-112">productCode</span><span class="sxs-lookup"><span data-stu-id="fbbc8-112">productCode</span></span>|<span data-ttu-id="fbbc8-113">String</span><span class="sxs-lookup"><span data-stu-id="fbbc8-113">String</span></span>|<span data-ttu-id="fbbc8-114">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-114">The MSI product code.</span></span>|
|<span data-ttu-id="fbbc8-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="fbbc8-115">productVersion</span></span>|<span data-ttu-id="fbbc8-116">String</span><span class="sxs-lookup"><span data-stu-id="fbbc8-116">String</span></span>|<span data-ttu-id="fbbc8-117">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-117">The MSI product version.</span></span>|
|<span data-ttu-id="fbbc8-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="fbbc8-118">upgradeCode</span></span>|<span data-ttu-id="fbbc8-119">字符串</span><span class="sxs-lookup"><span data-stu-id="fbbc8-119">String</span></span>|<span data-ttu-id="fbbc8-120">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="fbbc8-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="fbbc8-121">requiresReboot</span></span>|<span data-ttu-id="fbbc8-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="fbbc8-122">Boolean</span></span>|<span data-ttu-id="fbbc8-123">是否 MSI 应用程序要求计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="fbbc8-124">： 键入包</span><span class="sxs-lookup"><span data-stu-id="fbbc8-124">packageType</span></span>|[<span data-ttu-id="fbbc8-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="fbbc8-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="fbbc8-126">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-126">The MSI package type.</span></span> <span data-ttu-id="fbbc8-127">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbbc8-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="fbbc8-128">Relationships</span></span>
<span data-ttu-id="fbbc8-129">无</span><span class="sxs-lookup"><span data-stu-id="fbbc8-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fbbc8-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fbbc8-130">JSON Representation</span></span>
<span data-ttu-id="fbbc8-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fbbc8-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String"
}
```





