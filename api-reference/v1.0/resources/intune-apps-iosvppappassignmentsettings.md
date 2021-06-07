---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 342f773d48b4918693b6062aba161ce72c82d743
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756062"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="dcacb-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="dcacb-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="dcacb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcacb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dcacb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dcacb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcacb-106">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="dcacb-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="dcacb-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dcacb-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dcacb-108">属性</span><span class="sxs-lookup"><span data-stu-id="dcacb-108">Properties</span></span>
|<span data-ttu-id="dcacb-109">属性</span><span class="sxs-lookup"><span data-stu-id="dcacb-109">Property</span></span>|<span data-ttu-id="dcacb-110">类型</span><span class="sxs-lookup"><span data-stu-id="dcacb-110">Type</span></span>|<span data-ttu-id="dcacb-111">Description</span><span class="sxs-lookup"><span data-stu-id="dcacb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcacb-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="dcacb-112">useDeviceLicensing</span></span>|<span data-ttu-id="dcacb-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="dcacb-113">Boolean</span></span>|<span data-ttu-id="dcacb-114">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="dcacb-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="dcacb-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="dcacb-115">vpnConfigurationId</span></span>|<span data-ttu-id="dcacb-116">String</span><span class="sxs-lookup"><span data-stu-id="dcacb-116">String</span></span>|<span data-ttu-id="dcacb-117">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="dcacb-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcacb-118">关系</span><span class="sxs-lookup"><span data-stu-id="dcacb-118">Relationships</span></span>
<span data-ttu-id="dcacb-119">无</span><span class="sxs-lookup"><span data-stu-id="dcacb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcacb-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dcacb-120">JSON Representation</span></span>
<span data-ttu-id="dcacb-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dcacb-121">Here is a JSON representation of the resource.</span></span>
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




