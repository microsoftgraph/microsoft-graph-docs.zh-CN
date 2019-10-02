---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 883f81ab29dd2258d57753b792f0a4f1f434ed43
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360207"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="1c596-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c596-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1c596-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c596-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c596-105">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="1c596-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="1c596-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1c596-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c596-107">属性</span><span class="sxs-lookup"><span data-stu-id="1c596-107">Properties</span></span>
|<span data-ttu-id="1c596-108">属性</span><span class="sxs-lookup"><span data-stu-id="1c596-108">Property</span></span>|<span data-ttu-id="1c596-109">类型</span><span class="sxs-lookup"><span data-stu-id="1c596-109">Type</span></span>|<span data-ttu-id="1c596-110">说明</span><span class="sxs-lookup"><span data-stu-id="1c596-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c596-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="1c596-111">useDeviceLicensing</span></span>|<span data-ttu-id="1c596-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="1c596-112">Boolean</span></span>|<span data-ttu-id="1c596-113">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="1c596-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="1c596-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1c596-114">vpnConfigurationId</span></span>|<span data-ttu-id="1c596-115">String</span><span class="sxs-lookup"><span data-stu-id="1c596-115">String</span></span>|<span data-ttu-id="1c596-116">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="1c596-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c596-117">关系</span><span class="sxs-lookup"><span data-stu-id="1c596-117">Relationships</span></span>
<span data-ttu-id="1c596-118">无</span><span class="sxs-lookup"><span data-stu-id="1c596-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c596-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c596-119">JSON Representation</span></span>
<span data-ttu-id="1c596-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c596-120">Here is a JSON representation of the resource.</span></span>
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




