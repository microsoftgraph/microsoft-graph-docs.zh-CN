---
title: win32LobAppMsiInformation 资源类型
description: 包含 Win32 应用程序的 MSI 应用程序属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a812789a8231731b171edea8e15f7f540266cbde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080078"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="7c745-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c745-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="7c745-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c745-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c745-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c745-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c745-106">包含 Win32 应用程序的 MSI 应用程序属性。</span><span class="sxs-lookup"><span data-stu-id="7c745-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="7c745-107">属性</span><span class="sxs-lookup"><span data-stu-id="7c745-107">Properties</span></span>
|<span data-ttu-id="7c745-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c745-108">Property</span></span>|<span data-ttu-id="7c745-109">类型</span><span class="sxs-lookup"><span data-stu-id="7c745-109">Type</span></span>|<span data-ttu-id="7c745-110">说明</span><span class="sxs-lookup"><span data-stu-id="7c745-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c745-111">productCode</span><span class="sxs-lookup"><span data-stu-id="7c745-111">productCode</span></span>|<span data-ttu-id="7c745-112">String</span><span class="sxs-lookup"><span data-stu-id="7c745-112">String</span></span>|<span data-ttu-id="7c745-113">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="7c745-113">The MSI product code.</span></span>|
|<span data-ttu-id="7c745-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="7c745-114">productVersion</span></span>|<span data-ttu-id="7c745-115">String</span><span class="sxs-lookup"><span data-stu-id="7c745-115">String</span></span>|<span data-ttu-id="7c745-116">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="7c745-116">The MSI product version.</span></span>|
|<span data-ttu-id="7c745-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="7c745-117">upgradeCode</span></span>|<span data-ttu-id="7c745-118">String</span><span class="sxs-lookup"><span data-stu-id="7c745-118">String</span></span>|<span data-ttu-id="7c745-119">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="7c745-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="7c745-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="7c745-120">requiresReboot</span></span>|<span data-ttu-id="7c745-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="7c745-121">Boolean</span></span>|<span data-ttu-id="7c745-122">MSI 应用是否需要计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="7c745-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="7c745-123">packageType</span><span class="sxs-lookup"><span data-stu-id="7c745-123">packageType</span></span>|[<span data-ttu-id="7c745-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="7c745-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="7c745-125">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="7c745-125">The MSI package type.</span></span> <span data-ttu-id="7c745-126">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="7c745-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="7c745-127">productName</span><span class="sxs-lookup"><span data-stu-id="7c745-127">productName</span></span>|<span data-ttu-id="7c745-128">String</span><span class="sxs-lookup"><span data-stu-id="7c745-128">String</span></span>|<span data-ttu-id="7c745-129">MSI 产品名称。</span><span class="sxs-lookup"><span data-stu-id="7c745-129">The MSI product name.</span></span>|
|<span data-ttu-id="7c745-130">发布者</span><span class="sxs-lookup"><span data-stu-id="7c745-130">publisher</span></span>|<span data-ttu-id="7c745-131">String</span><span class="sxs-lookup"><span data-stu-id="7c745-131">String</span></span>|<span data-ttu-id="7c745-132">MSI 发布者。</span><span class="sxs-lookup"><span data-stu-id="7c745-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c745-133">关系</span><span class="sxs-lookup"><span data-stu-id="7c745-133">Relationships</span></span>
<span data-ttu-id="7c745-134">无</span><span class="sxs-lookup"><span data-stu-id="7c745-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c745-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c745-135">JSON Representation</span></span>
<span data-ttu-id="7c745-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c745-136">Here is a JSON representation of the resource.</span></span>
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





