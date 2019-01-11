---
title: mobileAppIntentAndStateDetail 资源类型
description: 移动应用程序的用途和给定的设备的安装状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad20ef00cbc8e5295a96107fbce2f5e7f1cb978a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805808"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="0c468-103">mobileAppIntentAndStateDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="0c468-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="0c468-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0c468-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c468-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0c468-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c468-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0c468-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c468-107">移动应用程序的用途和给定的设备的安装状态。</span><span class="sxs-lookup"><span data-stu-id="0c468-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="0c468-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c468-108">Properties</span></span>
|<span data-ttu-id="0c468-109">属性</span><span class="sxs-lookup"><span data-stu-id="0c468-109">Property</span></span>|<span data-ttu-id="0c468-110">类型</span><span class="sxs-lookup"><span data-stu-id="0c468-110">Type</span></span>|<span data-ttu-id="0c468-111">说明</span><span class="sxs-lookup"><span data-stu-id="0c468-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c468-112">applicationId</span><span class="sxs-lookup"><span data-stu-id="0c468-112">applicationId</span></span>|<span data-ttu-id="0c468-113">String</span><span class="sxs-lookup"><span data-stu-id="0c468-113">String</span></span>|<span data-ttu-id="0c468-114">MobieApp 标识符。</span><span class="sxs-lookup"><span data-stu-id="0c468-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="0c468-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0c468-115">displayName</span></span>|<span data-ttu-id="0c468-116">String</span><span class="sxs-lookup"><span data-stu-id="0c468-116">String</span></span>|<span data-ttu-id="0c468-117">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="0c468-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="0c468-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="0c468-118">mobileAppIntent</span></span>|[<span data-ttu-id="0c468-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="0c468-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="0c468-120">移动应用程序用途。</span><span class="sxs-lookup"><span data-stu-id="0c468-120">Mobile App Intent.</span></span> <span data-ttu-id="0c468-121">可取值为：`available`、`notAvailable`、`requiredInstall`、`requiredUninstall`、`requiredAndAvailableInstall`、`availableInstallWithoutEnrollment`、`exclude`。</span><span class="sxs-lookup"><span data-stu-id="0c468-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="0c468-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="0c468-122">displayVersion</span></span>|<span data-ttu-id="0c468-123">字符串</span><span class="sxs-lookup"><span data-stu-id="0c468-123">String</span></span>|<span data-ttu-id="0c468-124">人力易读的版本的应用程序</span><span class="sxs-lookup"><span data-stu-id="0c468-124">Human readable version of the application</span></span>|
|<span data-ttu-id="0c468-125">installState</span><span class="sxs-lookup"><span data-stu-id="0c468-125">installState</span></span>|[<span data-ttu-id="0c468-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="0c468-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="0c468-127">应用程序的安装状态。</span><span class="sxs-lookup"><span data-stu-id="0c468-127">The install state of the app.</span></span> <span data-ttu-id="0c468-128">可取值为：`installed`、`failed`、`notInstalled`、`uninstallFailed`、`pendingInstall`、`unknown`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="0c468-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="0c468-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="0c468-129">supportedDeviceTypes</span></span>|<span data-ttu-id="0c468-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)集合</span><span class="sxs-lookup"><span data-stu-id="0c468-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="0c468-131">应用程序的支持的平台。</span><span class="sxs-lookup"><span data-stu-id="0c468-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c468-132">Relationships</span><span class="sxs-lookup"><span data-stu-id="0c468-132">Relationships</span></span>
<span data-ttu-id="0c468-133">无</span><span class="sxs-lookup"><span data-stu-id="0c468-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c468-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0c468-134">JSON Representation</span></span>
<span data-ttu-id="0c468-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c468-135">Here is a JSON representation of the resource.</span></span>
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





