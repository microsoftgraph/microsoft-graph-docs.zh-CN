---
title: mobileAppIntentAndStateDetail 资源类型
description: 给定设备的移动应用意图和安装状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 76db364b53c9ccb6b4057835b853705cd49ca410
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146751"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="bade8-103">mobileAppIntentAndStateDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="bade8-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="bade8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bade8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bade8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bade8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bade8-106">给定设备的移动应用意图和安装状态。</span><span class="sxs-lookup"><span data-stu-id="bade8-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="bade8-107">属性</span><span class="sxs-lookup"><span data-stu-id="bade8-107">Properties</span></span>
|<span data-ttu-id="bade8-108">属性</span><span class="sxs-lookup"><span data-stu-id="bade8-108">Property</span></span>|<span data-ttu-id="bade8-109">类型</span><span class="sxs-lookup"><span data-stu-id="bade8-109">Type</span></span>|<span data-ttu-id="bade8-110">说明</span><span class="sxs-lookup"><span data-stu-id="bade8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bade8-111">applicationId</span><span class="sxs-lookup"><span data-stu-id="bade8-111">applicationId</span></span>|<span data-ttu-id="bade8-112">String</span><span class="sxs-lookup"><span data-stu-id="bade8-112">String</span></span>|<span data-ttu-id="bade8-113">MobieApp 标识符。</span><span class="sxs-lookup"><span data-stu-id="bade8-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="bade8-114">displayName</span><span class="sxs-lookup"><span data-stu-id="bade8-114">displayName</span></span>|<span data-ttu-id="bade8-115">String</span><span class="sxs-lookup"><span data-stu-id="bade8-115">String</span></span>|<span data-ttu-id="bade8-116">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="bade8-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="bade8-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="bade8-117">mobileAppIntent</span></span>|[<span data-ttu-id="bade8-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="bade8-118">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="bade8-119">移动应用程序意向。</span><span class="sxs-lookup"><span data-stu-id="bade8-119">Mobile App Intent.</span></span> <span data-ttu-id="bade8-120">可取值为：`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="bade8-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="bade8-121">displayVersion</span><span class="sxs-lookup"><span data-stu-id="bade8-121">displayVersion</span></span>|<span data-ttu-id="bade8-122">字符串</span><span class="sxs-lookup"><span data-stu-id="bade8-122">String</span></span>|<span data-ttu-id="bade8-123">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="bade8-123">Human readable version of the application</span></span>|
|<span data-ttu-id="bade8-124">installState</span><span class="sxs-lookup"><span data-stu-id="bade8-124">installState</span></span>|[<span data-ttu-id="bade8-125">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="bade8-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="bade8-126">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="bade8-126">The install state of the app.</span></span> <span data-ttu-id="bade8-127">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="bade8-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="bade8-128">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="bade8-128">supportedDeviceTypes</span></span>|<span data-ttu-id="bade8-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)集合</span><span class="sxs-lookup"><span data-stu-id="bade8-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="bade8-130">应用程序支持的平台。</span><span class="sxs-lookup"><span data-stu-id="bade8-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bade8-131">关系</span><span class="sxs-lookup"><span data-stu-id="bade8-131">Relationships</span></span>
<span data-ttu-id="bade8-132">无</span><span class="sxs-lookup"><span data-stu-id="bade8-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bade8-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bade8-133">JSON Representation</span></span>
<span data-ttu-id="bade8-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bade8-134">Here is a JSON representation of the resource.</span></span>
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




