---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 77480c88e6fd210704a47f60293081b1ede2e6ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005928"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="12a56-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="12a56-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="12a56-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="12a56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12a56-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="12a56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a56-106">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="12a56-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="12a56-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="12a56-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="12a56-108">属性</span><span class="sxs-lookup"><span data-stu-id="12a56-108">Properties</span></span>
|<span data-ttu-id="12a56-109">属性</span><span class="sxs-lookup"><span data-stu-id="12a56-109">Property</span></span>|<span data-ttu-id="12a56-110">类型</span><span class="sxs-lookup"><span data-stu-id="12a56-110">Type</span></span>|<span data-ttu-id="12a56-111">说明</span><span class="sxs-lookup"><span data-stu-id="12a56-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a56-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="12a56-112">useDeviceLicensing</span></span>|<span data-ttu-id="12a56-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="12a56-113">Boolean</span></span>|<span data-ttu-id="12a56-114">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="12a56-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="12a56-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="12a56-115">vpnConfigurationId</span></span>|<span data-ttu-id="12a56-116">String</span><span class="sxs-lookup"><span data-stu-id="12a56-116">String</span></span>|<span data-ttu-id="12a56-117">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="12a56-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12a56-118">关系</span><span class="sxs-lookup"><span data-stu-id="12a56-118">Relationships</span></span>
<span data-ttu-id="12a56-119">无</span><span class="sxs-lookup"><span data-stu-id="12a56-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="12a56-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12a56-120">JSON Representation</span></span>
<span data-ttu-id="12a56-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12a56-121">Here is a JSON representation of the resource.</span></span>
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





