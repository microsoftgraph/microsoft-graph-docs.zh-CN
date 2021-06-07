---
title: win32LobAppMsiInformation 资源类型
description: 包含 Win32 应用的 MSI 应用属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9c610711f58a9d1929d0e708e127e2b337396f8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752194"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="ff068-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff068-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="ff068-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff068-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff068-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff068-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff068-106">包含 Win32 应用的 MSI 应用属性。</span><span class="sxs-lookup"><span data-stu-id="ff068-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="ff068-107">属性</span><span class="sxs-lookup"><span data-stu-id="ff068-107">Properties</span></span>
|<span data-ttu-id="ff068-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff068-108">Property</span></span>|<span data-ttu-id="ff068-109">类型</span><span class="sxs-lookup"><span data-stu-id="ff068-109">Type</span></span>|<span data-ttu-id="ff068-110">Description</span><span class="sxs-lookup"><span data-stu-id="ff068-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff068-111">productCode</span><span class="sxs-lookup"><span data-stu-id="ff068-111">productCode</span></span>|<span data-ttu-id="ff068-112">String</span><span class="sxs-lookup"><span data-stu-id="ff068-112">String</span></span>|<span data-ttu-id="ff068-113">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="ff068-113">The MSI product code.</span></span>|
|<span data-ttu-id="ff068-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="ff068-114">productVersion</span></span>|<span data-ttu-id="ff068-115">String</span><span class="sxs-lookup"><span data-stu-id="ff068-115">String</span></span>|<span data-ttu-id="ff068-116">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="ff068-116">The MSI product version.</span></span>|
|<span data-ttu-id="ff068-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="ff068-117">upgradeCode</span></span>|<span data-ttu-id="ff068-118">String</span><span class="sxs-lookup"><span data-stu-id="ff068-118">String</span></span>|<span data-ttu-id="ff068-119">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="ff068-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="ff068-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="ff068-120">requiresReboot</span></span>|<span data-ttu-id="ff068-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff068-121">Boolean</span></span>|<span data-ttu-id="ff068-122">MSI 应用是否需要计算机重新启动才能完成安装。</span><span class="sxs-lookup"><span data-stu-id="ff068-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="ff068-123">packageType</span><span class="sxs-lookup"><span data-stu-id="ff068-123">packageType</span></span>|[<span data-ttu-id="ff068-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="ff068-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="ff068-125">MSI 程序包类型。</span><span class="sxs-lookup"><span data-stu-id="ff068-125">The MSI package type.</span></span> <span data-ttu-id="ff068-126">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="ff068-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="ff068-127">productName</span><span class="sxs-lookup"><span data-stu-id="ff068-127">productName</span></span>|<span data-ttu-id="ff068-128">String</span><span class="sxs-lookup"><span data-stu-id="ff068-128">String</span></span>|<span data-ttu-id="ff068-129">MSI 产品名称。</span><span class="sxs-lookup"><span data-stu-id="ff068-129">The MSI product name.</span></span>|
|<span data-ttu-id="ff068-130">发布者</span><span class="sxs-lookup"><span data-stu-id="ff068-130">publisher</span></span>|<span data-ttu-id="ff068-131">String</span><span class="sxs-lookup"><span data-stu-id="ff068-131">String</span></span>|<span data-ttu-id="ff068-132">MSI 发布者。</span><span class="sxs-lookup"><span data-stu-id="ff068-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff068-133">关系</span><span class="sxs-lookup"><span data-stu-id="ff068-133">Relationships</span></span>
<span data-ttu-id="ff068-134">无</span><span class="sxs-lookup"><span data-stu-id="ff068-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff068-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff068-135">JSON Representation</span></span>
<span data-ttu-id="ff068-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ff068-136">Here is a JSON representation of the resource.</span></span>
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




