---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a7934658ede6bed8a50461e9291f614d8e440a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095161"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="09851-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="09851-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="09851-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09851-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09851-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09851-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09851-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09851-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09851-107">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="09851-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="09851-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="09851-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09851-109">属性</span><span class="sxs-lookup"><span data-stu-id="09851-109">Properties</span></span>
|<span data-ttu-id="09851-110">属性</span><span class="sxs-lookup"><span data-stu-id="09851-110">Property</span></span>|<span data-ttu-id="09851-111">类型</span><span class="sxs-lookup"><span data-stu-id="09851-111">Type</span></span>|<span data-ttu-id="09851-112">说明</span><span class="sxs-lookup"><span data-stu-id="09851-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09851-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="09851-113">useDeviceLicensing</span></span>|<span data-ttu-id="09851-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="09851-114">Boolean</span></span>|<span data-ttu-id="09851-115">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="09851-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="09851-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="09851-116">vpnConfigurationId</span></span>|<span data-ttu-id="09851-117">String</span><span class="sxs-lookup"><span data-stu-id="09851-117">String</span></span>|<span data-ttu-id="09851-118">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="09851-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="09851-119">**应用**</span><span class="sxs-lookup"><span data-stu-id="09851-119">**Apps**</span></span>|
|<span data-ttu-id="09851-120">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="09851-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="09851-121">布尔</span><span class="sxs-lookup"><span data-stu-id="09851-121">Boolean</span></span>|<span data-ttu-id="09851-122">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="09851-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09851-123">关系</span><span class="sxs-lookup"><span data-stu-id="09851-123">Relationships</span></span>
<span data-ttu-id="09851-124">无</span><span class="sxs-lookup"><span data-stu-id="09851-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09851-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09851-125">JSON Representation</span></span>
<span data-ttu-id="09851-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09851-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```






