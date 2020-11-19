---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 60a7d42d686129948c0934f494633671145fe9c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49300589"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="1f4ef-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f4ef-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="1f4ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f4ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f4ef-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1f4ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1f4ef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1f4ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f4ef-107">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="1f4ef-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="1f4ef-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="1f4ef-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1f4ef-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f4ef-109">Properties</span></span>
|<span data-ttu-id="1f4ef-110">属性</span><span class="sxs-lookup"><span data-stu-id="1f4ef-110">Property</span></span>|<span data-ttu-id="1f4ef-111">类型</span><span class="sxs-lookup"><span data-stu-id="1f4ef-111">Type</span></span>|<span data-ttu-id="1f4ef-112">Description</span><span class="sxs-lookup"><span data-stu-id="1f4ef-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f4ef-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="1f4ef-113">vpnConfigurationId</span></span>|<span data-ttu-id="1f4ef-114">String</span><span class="sxs-lookup"><span data-stu-id="1f4ef-114">String</span></span>|<span data-ttu-id="1f4ef-115">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="1f4ef-115">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="1f4ef-116">**应用**</span><span class="sxs-lookup"><span data-stu-id="1f4ef-116">**Apps**</span></span>|
|<span data-ttu-id="1f4ef-117">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="1f4ef-117">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="1f4ef-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f4ef-118">Boolean</span></span>|<span data-ttu-id="1f4ef-119">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="1f4ef-119">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f4ef-120">关系</span><span class="sxs-lookup"><span data-stu-id="1f4ef-120">Relationships</span></span>
<span data-ttu-id="1f4ef-121">无</span><span class="sxs-lookup"><span data-stu-id="1f4ef-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f4ef-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f4ef-122">JSON Representation</span></span>
<span data-ttu-id="1f4ef-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f4ef-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```




