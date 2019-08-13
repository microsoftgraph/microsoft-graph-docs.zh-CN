---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da1d42d092c7a85831da6ae26b55b43db7ac7db7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365984"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="07cfa-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="07cfa-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="07cfa-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="07cfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07cfa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07cfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07cfa-106">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="07cfa-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="07cfa-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="07cfa-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07cfa-108">属性</span><span class="sxs-lookup"><span data-stu-id="07cfa-108">Properties</span></span>
|<span data-ttu-id="07cfa-109">属性</span><span class="sxs-lookup"><span data-stu-id="07cfa-109">Property</span></span>|<span data-ttu-id="07cfa-110">类型</span><span class="sxs-lookup"><span data-stu-id="07cfa-110">Type</span></span>|<span data-ttu-id="07cfa-111">说明</span><span class="sxs-lookup"><span data-stu-id="07cfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07cfa-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="07cfa-112">vpnConfigurationId</span></span>|<span data-ttu-id="07cfa-113">String</span><span class="sxs-lookup"><span data-stu-id="07cfa-113">String</span></span>|<span data-ttu-id="07cfa-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="07cfa-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="07cfa-115">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="07cfa-115">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="07cfa-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="07cfa-116">Boolean</span></span>|<span data-ttu-id="07cfa-117">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="07cfa-117">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07cfa-118">关系</span><span class="sxs-lookup"><span data-stu-id="07cfa-118">Relationships</span></span>
<span data-ttu-id="07cfa-119">无</span><span class="sxs-lookup"><span data-stu-id="07cfa-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07cfa-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07cfa-120">JSON Representation</span></span>
<span data-ttu-id="07cfa-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07cfa-121">Here is a JSON representation of the resource.</span></span>
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



