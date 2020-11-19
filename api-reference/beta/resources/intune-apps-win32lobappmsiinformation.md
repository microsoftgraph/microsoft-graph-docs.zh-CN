---
title: win32LobAppMsiInformation 资源类型
description: 包含 Win32 应用程序的 MSI 应用程序属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fb872d970256a795c51570d68b3279fce43506f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274003"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="911bf-103">win32LobAppMsiInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="911bf-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="911bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="911bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="911bf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="911bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="911bf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="911bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="911bf-107">包含 Win32 应用程序的 MSI 应用程序属性。</span><span class="sxs-lookup"><span data-stu-id="911bf-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="911bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="911bf-108">Properties</span></span>
|<span data-ttu-id="911bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="911bf-109">Property</span></span>|<span data-ttu-id="911bf-110">类型</span><span class="sxs-lookup"><span data-stu-id="911bf-110">Type</span></span>|<span data-ttu-id="911bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="911bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="911bf-112">productCode</span><span class="sxs-lookup"><span data-stu-id="911bf-112">productCode</span></span>|<span data-ttu-id="911bf-113">String</span><span class="sxs-lookup"><span data-stu-id="911bf-113">String</span></span>|<span data-ttu-id="911bf-114">MSI 产品代码。</span><span class="sxs-lookup"><span data-stu-id="911bf-114">The MSI product code.</span></span>|
|<span data-ttu-id="911bf-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="911bf-115">productVersion</span></span>|<span data-ttu-id="911bf-116">String</span><span class="sxs-lookup"><span data-stu-id="911bf-116">String</span></span>|<span data-ttu-id="911bf-117">MSI 产品版本。</span><span class="sxs-lookup"><span data-stu-id="911bf-117">The MSI product version.</span></span>|
|<span data-ttu-id="911bf-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="911bf-118">upgradeCode</span></span>|<span data-ttu-id="911bf-119">字符串</span><span class="sxs-lookup"><span data-stu-id="911bf-119">String</span></span>|<span data-ttu-id="911bf-120">MSI 升级代码。</span><span class="sxs-lookup"><span data-stu-id="911bf-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="911bf-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="911bf-121">requiresReboot</span></span>|<span data-ttu-id="911bf-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="911bf-122">Boolean</span></span>|<span data-ttu-id="911bf-123">MSI 应用是否需要计算机重新启动以完成安装。</span><span class="sxs-lookup"><span data-stu-id="911bf-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="911bf-124">packageType</span><span class="sxs-lookup"><span data-stu-id="911bf-124">packageType</span></span>|[<span data-ttu-id="911bf-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="911bf-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="911bf-126">MSI 包类型。</span><span class="sxs-lookup"><span data-stu-id="911bf-126">The MSI package type.</span></span> <span data-ttu-id="911bf-127">可取值为：`perMachine`、`perUser`、`dualPurpose`。</span><span class="sxs-lookup"><span data-stu-id="911bf-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="911bf-128">productName</span><span class="sxs-lookup"><span data-stu-id="911bf-128">productName</span></span>|<span data-ttu-id="911bf-129">String</span><span class="sxs-lookup"><span data-stu-id="911bf-129">String</span></span>|<span data-ttu-id="911bf-130">MSI 产品名称。</span><span class="sxs-lookup"><span data-stu-id="911bf-130">The MSI product name.</span></span>|
|<span data-ttu-id="911bf-131">发布者</span><span class="sxs-lookup"><span data-stu-id="911bf-131">publisher</span></span>|<span data-ttu-id="911bf-132">String</span><span class="sxs-lookup"><span data-stu-id="911bf-132">String</span></span>|<span data-ttu-id="911bf-133">MSI 发布者。</span><span class="sxs-lookup"><span data-stu-id="911bf-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="911bf-134">关系</span><span class="sxs-lookup"><span data-stu-id="911bf-134">Relationships</span></span>
<span data-ttu-id="911bf-135">无</span><span class="sxs-lookup"><span data-stu-id="911bf-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="911bf-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="911bf-136">JSON Representation</span></span>
<span data-ttu-id="911bf-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="911bf-137">Here is a JSON representation of the resource.</span></span>
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




