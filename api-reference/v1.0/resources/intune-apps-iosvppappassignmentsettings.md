---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 08b711eb4f1d1d79e61879386a24c546b7bda8ef
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018170"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="706db-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="706db-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="706db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="706db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="706db-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="706db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="706db-106">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="706db-106">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="706db-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="706db-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="706db-108">属性</span><span class="sxs-lookup"><span data-stu-id="706db-108">Properties</span></span>
|<span data-ttu-id="706db-109">属性</span><span class="sxs-lookup"><span data-stu-id="706db-109">Property</span></span>|<span data-ttu-id="706db-110">类型</span><span class="sxs-lookup"><span data-stu-id="706db-110">Type</span></span>|<span data-ttu-id="706db-111">说明</span><span class="sxs-lookup"><span data-stu-id="706db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="706db-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="706db-112">useDeviceLicensing</span></span>|<span data-ttu-id="706db-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="706db-113">Boolean</span></span>|<span data-ttu-id="706db-114">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="706db-114">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="706db-115">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="706db-115">vpnConfigurationId</span></span>|<span data-ttu-id="706db-116">String</span><span class="sxs-lookup"><span data-stu-id="706db-116">String</span></span>|<span data-ttu-id="706db-117">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="706db-117">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="706db-118">关系</span><span class="sxs-lookup"><span data-stu-id="706db-118">Relationships</span></span>
<span data-ttu-id="706db-119">无</span><span class="sxs-lookup"><span data-stu-id="706db-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="706db-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="706db-120">JSON Representation</span></span>
<span data-ttu-id="706db-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="706db-121">Here is a JSON representation of the resource.</span></span>
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









