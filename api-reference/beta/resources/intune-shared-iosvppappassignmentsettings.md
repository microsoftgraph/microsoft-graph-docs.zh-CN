---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 56e19bb10115faaf7386e6f54dc5ca2dc368ee33
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866088"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="34558-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="34558-103">iosVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="34558-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34558-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34558-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34558-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34558-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34558-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34558-107">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="34558-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>


<span data-ttu-id="34558-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="34558-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34558-109">属性</span><span class="sxs-lookup"><span data-stu-id="34558-109">Properties</span></span>
|<span data-ttu-id="34558-110">属性</span><span class="sxs-lookup"><span data-stu-id="34558-110">Property</span></span>|<span data-ttu-id="34558-111">类型</span><span class="sxs-lookup"><span data-stu-id="34558-111">Type</span></span>|<span data-ttu-id="34558-112">说明</span><span class="sxs-lookup"><span data-stu-id="34558-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34558-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="34558-113">useDeviceLicensing</span></span>|<span data-ttu-id="34558-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="34558-114">Boolean</span></span>|<span data-ttu-id="34558-115">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="34558-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="34558-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="34558-116">vpnConfigurationId</span></span>|<span data-ttu-id="34558-117">String</span><span class="sxs-lookup"><span data-stu-id="34558-117">String</span></span>|<span data-ttu-id="34558-118">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="34558-118">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="34558-119">**应用**</span><span class="sxs-lookup"><span data-stu-id="34558-119">**Apps**</span></span>|
|<span data-ttu-id="34558-120">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="34558-120">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="34558-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="34558-121">Boolean</span></span>|<span data-ttu-id="34558-122">从 Intune 中删除设备时是否卸载应用。</span><span class="sxs-lookup"><span data-stu-id="34558-122">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34558-123">关系</span><span class="sxs-lookup"><span data-stu-id="34558-123">Relationships</span></span>
<span data-ttu-id="34558-124">无</span><span class="sxs-lookup"><span data-stu-id="34558-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34558-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34558-125">JSON Representation</span></span>
<span data-ttu-id="34558-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34558-126">Here is a JSON representation of the resource.</span></span>
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




