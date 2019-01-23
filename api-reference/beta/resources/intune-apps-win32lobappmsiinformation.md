---
title: win32LobAppMsiInformation 资源类型
description: Win32 应用程序包含 MSI 应用程序的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ba91c572286020a3e349527f325d22bf0be5d67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399246"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="225f0-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="225f0-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="225f0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="225f0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="225f0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="225f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="225f0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="225f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="225f0-107">Win32 应用程序包含 MSI 应用程序的属性。</span><span class="sxs-lookup"><span data-stu-id="225f0-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="225f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="225f0-108">Properties</span></span>
|<span data-ttu-id="225f0-109">属性</span><span class="sxs-lookup"><span data-stu-id="225f0-109">Property</span></span>|<span data-ttu-id="225f0-110">类型</span><span class="sxs-lookup"><span data-stu-id="225f0-110">Type</span></span>|<span data-ttu-id="225f0-111">说明</span><span class="sxs-lookup"><span data-stu-id="225f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="225f0-112">productCode</span><span class="sxs-lookup"><span data-stu-id="225f0-112">productCode</span></span>|<span data-ttu-id="225f0-113">String</span><span class="sxs-lookup"><span data-stu-id="225f0-113">String</span></span>|<span data-ttu-id="225f0-114">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="225f0-114">The MSI product code.</span></span>|
|<span data-ttu-id="225f0-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="225f0-115">productVersion</span></span>|<span data-ttu-id="225f0-116">String</span><span class="sxs-lookup"><span data-stu-id="225f0-116">String</span></span>|<span data-ttu-id="225f0-117">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="225f0-117">The MSI product version.</span></span>|
|<span data-ttu-id="225f0-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="225f0-118">upgradeCode</span></span>|<span data-ttu-id="225f0-119">String</span><span class="sxs-lookup"><span data-stu-id="225f0-119">String</span></span>|<span data-ttu-id="225f0-120">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="225f0-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="225f0-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="225f0-121">requiresReboot</span></span>|<span data-ttu-id="225f0-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="225f0-122">Boolean</span></span>|<span data-ttu-id="225f0-123">是否 MSI 应用程序要求计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="225f0-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="225f0-124">： 键入包</span><span class="sxs-lookup"><span data-stu-id="225f0-124">packageType</span></span>|[<span data-ttu-id="225f0-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="225f0-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="225f0-126">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="225f0-126">The MSI package type.</span></span> <span data-ttu-id="225f0-127">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="225f0-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="225f0-128">Relationships</span><span class="sxs-lookup"><span data-stu-id="225f0-128">Relationships</span></span>
<span data-ttu-id="225f0-129">无</span><span class="sxs-lookup"><span data-stu-id="225f0-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="225f0-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="225f0-130">JSON Representation</span></span>
<span data-ttu-id="225f0-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="225f0-131">Here is a JSON representation of the resource.</span></span>
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




