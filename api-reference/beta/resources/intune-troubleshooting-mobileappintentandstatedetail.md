---
title: mobileAppIntentAndStateDetail 资源类型
description: 给定设备的移动应用意图和安装状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ca3645c5af594e5352e0fcd0dae70516e0548fba
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49271595"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="aef6b-103">mobileAppIntentAndStateDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="aef6b-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="aef6b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aef6b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aef6b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aef6b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aef6b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aef6b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aef6b-107">给定设备的移动应用意图和安装状态。</span><span class="sxs-lookup"><span data-stu-id="aef6b-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="aef6b-108">属性</span><span class="sxs-lookup"><span data-stu-id="aef6b-108">Properties</span></span>
|<span data-ttu-id="aef6b-109">属性</span><span class="sxs-lookup"><span data-stu-id="aef6b-109">Property</span></span>|<span data-ttu-id="aef6b-110">类型</span><span class="sxs-lookup"><span data-stu-id="aef6b-110">Type</span></span>|<span data-ttu-id="aef6b-111">说明</span><span class="sxs-lookup"><span data-stu-id="aef6b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aef6b-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="aef6b-112">applicationId</span></span>|<span data-ttu-id="aef6b-113">String</span><span class="sxs-lookup"><span data-stu-id="aef6b-113">String</span></span>|<span data-ttu-id="aef6b-114">MobieApp 标识符。</span><span class="sxs-lookup"><span data-stu-id="aef6b-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="aef6b-115">displayName</span><span class="sxs-lookup"><span data-stu-id="aef6b-115">displayName</span></span>|<span data-ttu-id="aef6b-116">字符串</span><span class="sxs-lookup"><span data-stu-id="aef6b-116">String</span></span>|<span data-ttu-id="aef6b-117">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="aef6b-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="aef6b-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="aef6b-118">mobileAppIntent</span></span>|[<span data-ttu-id="aef6b-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="aef6b-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="aef6b-120">移动应用程序意向。</span><span class="sxs-lookup"><span data-stu-id="aef6b-120">Mobile App Intent.</span></span> <span data-ttu-id="aef6b-121">可取值为：`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment` 或 `exclude`。</span><span class="sxs-lookup"><span data-stu-id="aef6b-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="aef6b-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="aef6b-122">displayVersion</span></span>|<span data-ttu-id="aef6b-123">字符串</span><span class="sxs-lookup"><span data-stu-id="aef6b-123">String</span></span>|<span data-ttu-id="aef6b-124">人工可读版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="aef6b-124">Human readable version of the application</span></span>|
|<span data-ttu-id="aef6b-125">installState</span><span class="sxs-lookup"><span data-stu-id="aef6b-125">installState</span></span>|[<span data-ttu-id="aef6b-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="aef6b-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="aef6b-127">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="aef6b-127">The install state of the app.</span></span> <span data-ttu-id="aef6b-128">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown` 或 `notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="aef6b-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="aef6b-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="aef6b-129">supportedDeviceTypes</span></span>|<span data-ttu-id="aef6b-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="aef6b-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="aef6b-131">应用程序支持的平台。</span><span class="sxs-lookup"><span data-stu-id="aef6b-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aef6b-132">关系</span><span class="sxs-lookup"><span data-stu-id="aef6b-132">Relationships</span></span>
<span data-ttu-id="aef6b-133">无</span><span class="sxs-lookup"><span data-stu-id="aef6b-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aef6b-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aef6b-134">JSON Representation</span></span>
<span data-ttu-id="aef6b-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aef6b-135">Here is a JSON representation of the resource.</span></span>
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




