---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8a72f1876d0d0dcd181aee7a9b0322f372838377
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769568"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="d7067-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7067-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d7067-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7067-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7067-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7067-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7067-106">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="d7067-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="d7067-107">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d7067-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7067-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7067-108">Properties</span></span>
|<span data-ttu-id="d7067-109">属性</span><span class="sxs-lookup"><span data-stu-id="d7067-109">Property</span></span>|<span data-ttu-id="d7067-110">类型</span><span class="sxs-lookup"><span data-stu-id="d7067-110">Type</span></span>|<span data-ttu-id="d7067-111">说明</span><span class="sxs-lookup"><span data-stu-id="d7067-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7067-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="d7067-112">useDeviceLicensing</span></span>|<span data-ttu-id="d7067-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="d7067-113">Boolean</span></span>|<span data-ttu-id="d7067-114">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="d7067-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="d7067-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d7067-115">vpnConfigurationId</span></span>|<span data-ttu-id="d7067-116">String</span><span class="sxs-lookup"><span data-stu-id="d7067-116">String</span></span>|<span data-ttu-id="d7067-117">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="d7067-117">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="d7067-118">**应用**</span><span class="sxs-lookup"><span data-stu-id="d7067-118">**Apps**</span></span>|
|<span data-ttu-id="d7067-119">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="d7067-119">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="d7067-120">布尔值</span><span class="sxs-lookup"><span data-stu-id="d7067-120">Boolean</span></span>|<span data-ttu-id="d7067-121">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="d7067-121">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7067-122">关系</span><span class="sxs-lookup"><span data-stu-id="d7067-122">Relationships</span></span>
<span data-ttu-id="d7067-123">无</span><span class="sxs-lookup"><span data-stu-id="d7067-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7067-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7067-124">JSON Representation</span></span>
<span data-ttu-id="d7067-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7067-125">Here is a JSON representation of the resource.</span></span>
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



