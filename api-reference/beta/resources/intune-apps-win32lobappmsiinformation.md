---
title: win32LobAppMsiInformation 资源类型
description: 包含 Win32 应用程序的 MSI 应用程序属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd612a5593ef151d4f324f3058c793ce7cd29bf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949631"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="100bd-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="100bd-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="100bd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="100bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="100bd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="100bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="100bd-106">包含 Win32 应用程序的 MSI 应用程序属性。</span><span class="sxs-lookup"><span data-stu-id="100bd-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="100bd-107">属性</span><span class="sxs-lookup"><span data-stu-id="100bd-107">Properties</span></span>
|<span data-ttu-id="100bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="100bd-108">Property</span></span>|<span data-ttu-id="100bd-109">类型</span><span class="sxs-lookup"><span data-stu-id="100bd-109">Type</span></span>|<span data-ttu-id="100bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="100bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="100bd-111">productCode</span><span class="sxs-lookup"><span data-stu-id="100bd-111">productCode</span></span>|<span data-ttu-id="100bd-112">String</span><span class="sxs-lookup"><span data-stu-id="100bd-112">String</span></span>|<span data-ttu-id="100bd-113">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="100bd-113">The MSI product code.</span></span>|
|<span data-ttu-id="100bd-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="100bd-114">productVersion</span></span>|<span data-ttu-id="100bd-115">String</span><span class="sxs-lookup"><span data-stu-id="100bd-115">String</span></span>|<span data-ttu-id="100bd-116">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="100bd-116">The MSI product version.</span></span>|
|<span data-ttu-id="100bd-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="100bd-117">upgradeCode</span></span>|<span data-ttu-id="100bd-118">String</span><span class="sxs-lookup"><span data-stu-id="100bd-118">String</span></span>|<span data-ttu-id="100bd-119">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="100bd-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="100bd-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="100bd-120">requiresReboot</span></span>|<span data-ttu-id="100bd-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="100bd-121">Boolean</span></span>|<span data-ttu-id="100bd-122">MSI 应用是否需要计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="100bd-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="100bd-123">packageType</span><span class="sxs-lookup"><span data-stu-id="100bd-123">packageType</span></span>|[<span data-ttu-id="100bd-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="100bd-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="100bd-125">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="100bd-125">The MSI package type.</span></span> <span data-ttu-id="100bd-126">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="100bd-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="100bd-127">productName</span><span class="sxs-lookup"><span data-stu-id="100bd-127">productName</span></span>|<span data-ttu-id="100bd-128">String</span><span class="sxs-lookup"><span data-stu-id="100bd-128">String</span></span>|<span data-ttu-id="100bd-129">MSI 产品名称。</span><span class="sxs-lookup"><span data-stu-id="100bd-129">The MSI product name.</span></span>|
|<span data-ttu-id="100bd-130">发布者</span><span class="sxs-lookup"><span data-stu-id="100bd-130">publisher</span></span>|<span data-ttu-id="100bd-131">String</span><span class="sxs-lookup"><span data-stu-id="100bd-131">String</span></span>|<span data-ttu-id="100bd-132">MSI 发布者。</span><span class="sxs-lookup"><span data-stu-id="100bd-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="100bd-133">关系</span><span class="sxs-lookup"><span data-stu-id="100bd-133">Relationships</span></span>
<span data-ttu-id="100bd-134">无</span><span class="sxs-lookup"><span data-stu-id="100bd-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="100bd-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="100bd-135">JSON Representation</span></span>
<span data-ttu-id="100bd-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="100bd-136">Here is a JSON representation of the resource.</span></span>
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
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```




