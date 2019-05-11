---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7570108ac38b417ca4d1a5213759c071fe8492b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950457"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="29e34-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="29e34-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="29e34-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29e34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29e34-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29e34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29e34-106">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="29e34-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="29e34-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="29e34-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="29e34-108">属性</span><span class="sxs-lookup"><span data-stu-id="29e34-108">Properties</span></span>
|<span data-ttu-id="29e34-109">属性</span><span class="sxs-lookup"><span data-stu-id="29e34-109">Property</span></span>|<span data-ttu-id="29e34-110">类型</span><span class="sxs-lookup"><span data-stu-id="29e34-110">Type</span></span>|<span data-ttu-id="29e34-111">说明</span><span class="sxs-lookup"><span data-stu-id="29e34-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e34-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="29e34-112">useDeviceLicensing</span></span>|<span data-ttu-id="29e34-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="29e34-113">Boolean</span></span>|<span data-ttu-id="29e34-114">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="29e34-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="29e34-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="29e34-115">vpnConfigurationId</span></span>|<span data-ttu-id="29e34-116">String</span><span class="sxs-lookup"><span data-stu-id="29e34-116">String</span></span>|<span data-ttu-id="29e34-117">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="29e34-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29e34-118">关系</span><span class="sxs-lookup"><span data-stu-id="29e34-118">Relationships</span></span>
<span data-ttu-id="29e34-119">无</span><span class="sxs-lookup"><span data-stu-id="29e34-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29e34-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29e34-120">JSON Representation</span></span>
<span data-ttu-id="29e34-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29e34-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```




