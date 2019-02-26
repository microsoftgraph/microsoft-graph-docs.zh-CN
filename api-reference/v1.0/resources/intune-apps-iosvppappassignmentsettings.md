---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d1ff346b9ae786fdc2158a5386625f808e04c181
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261115"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="0f6a8-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f6a8-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0f6a8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f6a8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f6a8-105">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="0f6a8-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="0f6a8-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0f6a8-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0f6a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f6a8-107">Properties</span></span>
|<span data-ttu-id="0f6a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="0f6a8-108">Property</span></span>|<span data-ttu-id="0f6a8-109">类型</span><span class="sxs-lookup"><span data-stu-id="0f6a8-109">Type</span></span>|<span data-ttu-id="0f6a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="0f6a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f6a8-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="0f6a8-111">useDeviceLicensing</span></span>|<span data-ttu-id="0f6a8-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="0f6a8-112">Boolean</span></span>|<span data-ttu-id="0f6a8-113">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="0f6a8-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="0f6a8-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="0f6a8-114">vpnConfigurationId</span></span>|<span data-ttu-id="0f6a8-115">String</span><span class="sxs-lookup"><span data-stu-id="0f6a8-115">String</span></span>|<span data-ttu-id="0f6a8-116">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="0f6a8-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f6a8-117">关系</span><span class="sxs-lookup"><span data-stu-id="0f6a8-117">Relationships</span></span>
<span data-ttu-id="0f6a8-118">无</span><span class="sxs-lookup"><span data-stu-id="0f6a8-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f6a8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f6a8-119">JSON Representation</span></span>
<span data-ttu-id="0f6a8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f6a8-120">Here is a JSON representation of the resource.</span></span>
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



