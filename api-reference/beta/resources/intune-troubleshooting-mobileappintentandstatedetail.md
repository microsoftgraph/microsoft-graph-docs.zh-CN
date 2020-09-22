---
title: mobileAppIntentAndStateDetail 资源类型
description: 给定设备的移动应用意图和安装状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fa57fb4218d961d8d3e58eb284062998903325b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003589"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="1ebec-103">mobileAppIntentAndStateDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ebec-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="1ebec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ebec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ebec-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ebec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ebec-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ebec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ebec-107">给定设备的移动应用意图和安装状态。</span><span class="sxs-lookup"><span data-stu-id="1ebec-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="1ebec-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ebec-108">Properties</span></span>
|<span data-ttu-id="1ebec-109">属性</span><span class="sxs-lookup"><span data-stu-id="1ebec-109">Property</span></span>|<span data-ttu-id="1ebec-110">类型</span><span class="sxs-lookup"><span data-stu-id="1ebec-110">Type</span></span>|<span data-ttu-id="1ebec-111">说明</span><span class="sxs-lookup"><span data-stu-id="1ebec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ebec-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="1ebec-112">applicationId</span></span>|<span data-ttu-id="1ebec-113">String</span><span class="sxs-lookup"><span data-stu-id="1ebec-113">String</span></span>|<span data-ttu-id="1ebec-114">MobieApp 标识符。</span><span class="sxs-lookup"><span data-stu-id="1ebec-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="1ebec-115">displayName</span><span class="sxs-lookup"><span data-stu-id="1ebec-115">displayName</span></span>|<span data-ttu-id="1ebec-116">String</span><span class="sxs-lookup"><span data-stu-id="1ebec-116">String</span></span>|<span data-ttu-id="1ebec-117">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="1ebec-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="1ebec-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="1ebec-118">mobileAppIntent</span></span>|[<span data-ttu-id="1ebec-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="1ebec-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="1ebec-120">移动应用程序意向。</span><span class="sxs-lookup"><span data-stu-id="1ebec-120">Mobile App Intent.</span></span> <span data-ttu-id="1ebec-121">可取值为：`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment` 或 `exclude`。</span><span class="sxs-lookup"><span data-stu-id="1ebec-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="1ebec-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="1ebec-122">displayVersion</span></span>|<span data-ttu-id="1ebec-123">String</span><span class="sxs-lookup"><span data-stu-id="1ebec-123">String</span></span>|<span data-ttu-id="1ebec-124">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="1ebec-124">Human readable version of the application</span></span>|
|<span data-ttu-id="1ebec-125">installState</span><span class="sxs-lookup"><span data-stu-id="1ebec-125">installState</span></span>|[<span data-ttu-id="1ebec-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="1ebec-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="1ebec-127">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="1ebec-127">The install state of the app.</span></span> <span data-ttu-id="1ebec-128">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="1ebec-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="1ebec-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="1ebec-129">supportedDeviceTypes</span></span>|<span data-ttu-id="1ebec-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1ebec-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="1ebec-131">应用程序支持的平台。</span><span class="sxs-lookup"><span data-stu-id="1ebec-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ebec-132">关系</span><span class="sxs-lookup"><span data-stu-id="1ebec-132">Relationships</span></span>
<span data-ttu-id="1ebec-133">无</span><span class="sxs-lookup"><span data-stu-id="1ebec-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ebec-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ebec-134">JSON Representation</span></span>
<span data-ttu-id="1ebec-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ebec-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```






