---
title: mobileAppIntentAndStateDetail 资源类型
description: 移动应用程序的用途和给定的设备的安装状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ef88a1fa346784ae00a125a487ca844c58d62eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414254"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="5976f-103">mobileAppIntentAndStateDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="5976f-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="5976f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="5976f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5976f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5976f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5976f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5976f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5976f-107">移动应用程序的用途和给定的设备的安装状态。</span><span class="sxs-lookup"><span data-stu-id="5976f-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="5976f-108">属性</span><span class="sxs-lookup"><span data-stu-id="5976f-108">Properties</span></span>
|<span data-ttu-id="5976f-109">属性</span><span class="sxs-lookup"><span data-stu-id="5976f-109">Property</span></span>|<span data-ttu-id="5976f-110">类型</span><span class="sxs-lookup"><span data-stu-id="5976f-110">Type</span></span>|<span data-ttu-id="5976f-111">说明</span><span class="sxs-lookup"><span data-stu-id="5976f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5976f-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="5976f-112">applicationId</span></span>|<span data-ttu-id="5976f-113">String</span><span class="sxs-lookup"><span data-stu-id="5976f-113">String</span></span>|<span data-ttu-id="5976f-114">MobieApp 标识符。</span><span class="sxs-lookup"><span data-stu-id="5976f-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="5976f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5976f-115">displayName</span></span>|<span data-ttu-id="5976f-116">String</span><span class="sxs-lookup"><span data-stu-id="5976f-116">String</span></span>|<span data-ttu-id="5976f-117">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="5976f-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="5976f-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="5976f-118">mobileAppIntent</span></span>|[<span data-ttu-id="5976f-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="5976f-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="5976f-120">移动应用程序用途。</span><span class="sxs-lookup"><span data-stu-id="5976f-120">Mobile App Intent.</span></span> <span data-ttu-id="5976f-121">可取值为：`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="5976f-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="5976f-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="5976f-122">displayVersion</span></span>|<span data-ttu-id="5976f-123">String</span><span class="sxs-lookup"><span data-stu-id="5976f-123">String</span></span>|<span data-ttu-id="5976f-124">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="5976f-124">Human readable version of the application</span></span>|
|<span data-ttu-id="5976f-125">installState</span><span class="sxs-lookup"><span data-stu-id="5976f-125">installState</span></span>|[<span data-ttu-id="5976f-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="5976f-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="5976f-127">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="5976f-127">The install state of the app.</span></span> <span data-ttu-id="5976f-128">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="5976f-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="5976f-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="5976f-129">supportedDeviceTypes</span></span>|<span data-ttu-id="5976f-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)集合</span><span class="sxs-lookup"><span data-stu-id="5976f-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="5976f-131">应用程序的支持的平台。</span><span class="sxs-lookup"><span data-stu-id="5976f-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5976f-132">关系</span><span class="sxs-lookup"><span data-stu-id="5976f-132">Relationships</span></span>
<span data-ttu-id="5976f-133">无</span><span class="sxs-lookup"><span data-stu-id="5976f-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5976f-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5976f-134">JSON Representation</span></span>
<span data-ttu-id="5976f-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5976f-135">Here is a JSON representation of the resource.</span></span>
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




