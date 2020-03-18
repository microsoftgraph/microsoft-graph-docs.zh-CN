---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23cb5d484aaa813bfb1b3cd352cd0168e750713e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769673"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="4a621-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a621-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4a621-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a621-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a621-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a621-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a621-106">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="4a621-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="4a621-107">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="4a621-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4a621-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a621-108">Properties</span></span>
|<span data-ttu-id="4a621-109">属性</span><span class="sxs-lookup"><span data-stu-id="4a621-109">Property</span></span>|<span data-ttu-id="4a621-110">类型</span><span class="sxs-lookup"><span data-stu-id="4a621-110">Type</span></span>|<span data-ttu-id="4a621-111">说明</span><span class="sxs-lookup"><span data-stu-id="4a621-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a621-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4a621-112">vpnConfigurationId</span></span>|<span data-ttu-id="4a621-113">String</span><span class="sxs-lookup"><span data-stu-id="4a621-113">String</span></span>|<span data-ttu-id="4a621-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="4a621-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="4a621-115">**应用**</span><span class="sxs-lookup"><span data-stu-id="4a621-115">**Apps**</span></span>|
|<span data-ttu-id="4a621-116">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="4a621-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="4a621-117">布尔值</span><span class="sxs-lookup"><span data-stu-id="4a621-117">Boolean</span></span>|<span data-ttu-id="4a621-118">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="4a621-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a621-119">关系</span><span class="sxs-lookup"><span data-stu-id="4a621-119">Relationships</span></span>
<span data-ttu-id="4a621-120">无</span><span class="sxs-lookup"><span data-stu-id="4a621-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a621-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a621-121">JSON Representation</span></span>
<span data-ttu-id="4a621-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a621-122">Here is a JSON representation of the resource.</span></span>
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



