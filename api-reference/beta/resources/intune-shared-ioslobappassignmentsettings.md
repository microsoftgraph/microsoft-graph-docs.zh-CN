---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a379e7467fb7e76a1043d73f766dace5b28a27d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199932"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="ad195-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ad195-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="ad195-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ad195-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad195-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ad195-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad195-106">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="ad195-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="ad195-107">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="ad195-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ad195-108">属性</span><span class="sxs-lookup"><span data-stu-id="ad195-108">Properties</span></span>
|<span data-ttu-id="ad195-109">属性</span><span class="sxs-lookup"><span data-stu-id="ad195-109">Property</span></span>|<span data-ttu-id="ad195-110">类型</span><span class="sxs-lookup"><span data-stu-id="ad195-110">Type</span></span>|<span data-ttu-id="ad195-111">说明</span><span class="sxs-lookup"><span data-stu-id="ad195-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad195-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="ad195-112">vpnConfigurationId</span></span>|<span data-ttu-id="ad195-113">String</span><span class="sxs-lookup"><span data-stu-id="ad195-113">String</span></span>|<span data-ttu-id="ad195-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="ad195-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="ad195-115">**应用**</span><span class="sxs-lookup"><span data-stu-id="ad195-115">**Apps**</span></span>|
|<span data-ttu-id="ad195-116">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="ad195-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="ad195-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad195-117">Boolean</span></span>|<span data-ttu-id="ad195-118">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="ad195-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad195-119">关系</span><span class="sxs-lookup"><span data-stu-id="ad195-119">Relationships</span></span>
<span data-ttu-id="ad195-120">无</span><span class="sxs-lookup"><span data-stu-id="ad195-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad195-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ad195-121">JSON Representation</span></span>
<span data-ttu-id="ad195-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad195-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String",
  "uninstallOnDeviceRemoval": true
}
```



