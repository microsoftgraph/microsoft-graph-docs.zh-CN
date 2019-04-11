---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36c6e2c60423038f2af10ccdbcfaf94ecd6ec3aa
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806851"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e2680-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2680-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e2680-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2680-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2680-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2680-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2680-106">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="e2680-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="e2680-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e2680-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2680-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2680-108">Properties</span></span>
|<span data-ttu-id="e2680-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2680-109">Property</span></span>|<span data-ttu-id="e2680-110">类型</span><span class="sxs-lookup"><span data-stu-id="e2680-110">Type</span></span>|<span data-ttu-id="e2680-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2680-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2680-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e2680-112">useDeviceLicensing</span></span>|<span data-ttu-id="e2680-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="e2680-113">Boolean</span></span>|<span data-ttu-id="e2680-114">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="e2680-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="e2680-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e2680-115">vpnConfigurationId</span></span>|<span data-ttu-id="e2680-116">String</span><span class="sxs-lookup"><span data-stu-id="e2680-116">String</span></span>|<span data-ttu-id="e2680-117">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="e2680-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2680-118">关系</span><span class="sxs-lookup"><span data-stu-id="e2680-118">Relationships</span></span>
<span data-ttu-id="e2680-119">无</span><span class="sxs-lookup"><span data-stu-id="e2680-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2680-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2680-120">JSON Representation</span></span>
<span data-ttu-id="e2680-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2680-121">Here is a JSON representation of the resource.</span></span>
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





