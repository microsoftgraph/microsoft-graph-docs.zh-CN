---
title: win32LobAppMsiInformation 资源类型
description: Win32 应用程序包含 MSI 应用程序的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e43b3dc9e46ed193b7547a7ce85863253445d30c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846513"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="91509-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="91509-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="91509-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="91509-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91509-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="91509-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91509-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="91509-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91509-107">Win32 应用程序包含 MSI 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="91509-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="91509-108">属性</span><span class="sxs-lookup"><span data-stu-id="91509-108">Properties</span></span>
|<span data-ttu-id="91509-109">属性</span><span class="sxs-lookup"><span data-stu-id="91509-109">Property</span></span>|<span data-ttu-id="91509-110">类型</span><span class="sxs-lookup"><span data-stu-id="91509-110">Type</span></span>|<span data-ttu-id="91509-111">Description</span><span class="sxs-lookup"><span data-stu-id="91509-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91509-112">productCode</span><span class="sxs-lookup"><span data-stu-id="91509-112">productCode</span></span>|<span data-ttu-id="91509-113">String</span><span class="sxs-lookup"><span data-stu-id="91509-113">String</span></span>|<span data-ttu-id="91509-114">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="91509-114">The MSI product code.</span></span>|
|<span data-ttu-id="91509-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="91509-115">productVersion</span></span>|<span data-ttu-id="91509-116">String</span><span class="sxs-lookup"><span data-stu-id="91509-116">String</span></span>|<span data-ttu-id="91509-117">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="91509-117">The MSI product version.</span></span>|
|<span data-ttu-id="91509-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="91509-118">upgradeCode</span></span>|<span data-ttu-id="91509-119">字符串</span><span class="sxs-lookup"><span data-stu-id="91509-119">String</span></span>|<span data-ttu-id="91509-120">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="91509-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="91509-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="91509-121">requiresReboot</span></span>|<span data-ttu-id="91509-122">布尔</span><span class="sxs-lookup"><span data-stu-id="91509-122">Boolean</span></span>|<span data-ttu-id="91509-123">是否 MSI 应用程序要求计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="91509-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="91509-124">： 键入包</span><span class="sxs-lookup"><span data-stu-id="91509-124">packageType</span></span>|[<span data-ttu-id="91509-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="91509-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="91509-126">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="91509-126">The MSI package type.</span></span> <span data-ttu-id="91509-127">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="91509-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91509-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="91509-128">Relationships</span></span>
<span data-ttu-id="91509-129">无</span><span class="sxs-lookup"><span data-stu-id="91509-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91509-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91509-130">JSON Representation</span></span>
<span data-ttu-id="91509-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91509-131">Here is a JSON representation of the resource.</span></span>
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





