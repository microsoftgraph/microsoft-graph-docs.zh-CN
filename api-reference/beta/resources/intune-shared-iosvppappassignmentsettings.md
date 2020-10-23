---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f815b0530a87dd937a7ff9e88c8ff928865378ef
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684461"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="f0c96-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0c96-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="f0c96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0c96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0c96-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0c96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0c96-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0c96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0c96-107">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="f0c96-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="f0c96-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f0c96-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0c96-109">属性</span><span class="sxs-lookup"><span data-stu-id="f0c96-109">Properties</span></span>
|<span data-ttu-id="f0c96-110">属性</span><span class="sxs-lookup"><span data-stu-id="f0c96-110">Property</span></span>|<span data-ttu-id="f0c96-111">类型</span><span class="sxs-lookup"><span data-stu-id="f0c96-111">Type</span></span>|<span data-ttu-id="f0c96-112">说明</span><span class="sxs-lookup"><span data-stu-id="f0c96-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0c96-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="f0c96-113">useDeviceLicensing</span></span>|<span data-ttu-id="f0c96-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="f0c96-114">Boolean</span></span>|<span data-ttu-id="f0c96-115">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="f0c96-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="f0c96-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f0c96-116">vpnConfigurationId</span></span>|<span data-ttu-id="f0c96-117">String</span><span class="sxs-lookup"><span data-stu-id="f0c96-117">String</span></span>|<span data-ttu-id="f0c96-118">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="f0c96-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="f0c96-119">**应用**</span><span class="sxs-lookup"><span data-stu-id="f0c96-119">**Apps**</span></span>|
|<span data-ttu-id="f0c96-120">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="f0c96-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="f0c96-121">布尔</span><span class="sxs-lookup"><span data-stu-id="f0c96-121">Boolean</span></span>|<span data-ttu-id="f0c96-122">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="f0c96-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0c96-123">关系</span><span class="sxs-lookup"><span data-stu-id="f0c96-123">Relationships</span></span>
<span data-ttu-id="f0c96-124">无</span><span class="sxs-lookup"><span data-stu-id="f0c96-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0c96-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0c96-125">JSON Representation</span></span>
<span data-ttu-id="f0c96-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0c96-126">Here is a JSON representation of the resource.</span></span>
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





