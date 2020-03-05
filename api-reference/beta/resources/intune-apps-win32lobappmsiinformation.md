---
title: win32LobAppMsiInformation 资源类型
description: 包含 Win32 应用程序的 MSI 应用程序属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 92ff70c8b1bbf63ce6fd81321282a0f61f4accc3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490691"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="4b431-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b431-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="4b431-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4b431-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b431-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b431-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b431-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b431-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b431-107">包含 Win32 应用程序的 MSI 应用程序属性。</span><span class="sxs-lookup"><span data-stu-id="4b431-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="4b431-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b431-108">Properties</span></span>
|<span data-ttu-id="4b431-109">属性</span><span class="sxs-lookup"><span data-stu-id="4b431-109">Property</span></span>|<span data-ttu-id="4b431-110">类型</span><span class="sxs-lookup"><span data-stu-id="4b431-110">Type</span></span>|<span data-ttu-id="4b431-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b431-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b431-112">productCode</span><span class="sxs-lookup"><span data-stu-id="4b431-112">productCode</span></span>|<span data-ttu-id="4b431-113">String</span><span class="sxs-lookup"><span data-stu-id="4b431-113">String</span></span>|<span data-ttu-id="4b431-114">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="4b431-114">The MSI product code.</span></span>|
|<span data-ttu-id="4b431-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="4b431-115">productVersion</span></span>|<span data-ttu-id="4b431-116">String</span><span class="sxs-lookup"><span data-stu-id="4b431-116">String</span></span>|<span data-ttu-id="4b431-117">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="4b431-117">The MSI product version.</span></span>|
|<span data-ttu-id="4b431-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="4b431-118">upgradeCode</span></span>|<span data-ttu-id="4b431-119">String</span><span class="sxs-lookup"><span data-stu-id="4b431-119">String</span></span>|<span data-ttu-id="4b431-120">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="4b431-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="4b431-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="4b431-121">requiresReboot</span></span>|<span data-ttu-id="4b431-122">布尔</span><span class="sxs-lookup"><span data-stu-id="4b431-122">Boolean</span></span>|<span data-ttu-id="4b431-123">MSI 应用是否需要计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="4b431-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="4b431-124">packageType</span><span class="sxs-lookup"><span data-stu-id="4b431-124">packageType</span></span>|[<span data-ttu-id="4b431-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="4b431-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="4b431-126">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="4b431-126">The MSI package type.</span></span> <span data-ttu-id="4b431-127">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="4b431-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="4b431-128">productName</span><span class="sxs-lookup"><span data-stu-id="4b431-128">productName</span></span>|<span data-ttu-id="4b431-129">String</span><span class="sxs-lookup"><span data-stu-id="4b431-129">String</span></span>|<span data-ttu-id="4b431-130">MSI 产品名称。</span><span class="sxs-lookup"><span data-stu-id="4b431-130">The MSI product name.</span></span>|
|<span data-ttu-id="4b431-131">发布者</span><span class="sxs-lookup"><span data-stu-id="4b431-131">publisher</span></span>|<span data-ttu-id="4b431-132">String</span><span class="sxs-lookup"><span data-stu-id="4b431-132">String</span></span>|<span data-ttu-id="4b431-133">MSI 发布者。</span><span class="sxs-lookup"><span data-stu-id="4b431-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b431-134">关系</span><span class="sxs-lookup"><span data-stu-id="4b431-134">Relationships</span></span>
<span data-ttu-id="4b431-135">无</span><span class="sxs-lookup"><span data-stu-id="4b431-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b431-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b431-136">JSON Representation</span></span>
<span data-ttu-id="4b431-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b431-137">Here is a JSON representation of the resource.</span></span>
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



