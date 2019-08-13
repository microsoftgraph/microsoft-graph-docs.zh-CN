---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3cb8c437d5cb943ef4d6f76ed515b917f8a3e10a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366061"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="b584f-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b584f-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b584f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b584f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b584f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b584f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b584f-106">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="b584f-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="b584f-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b584f-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b584f-108">属性</span><span class="sxs-lookup"><span data-stu-id="b584f-108">Properties</span></span>
|<span data-ttu-id="b584f-109">属性</span><span class="sxs-lookup"><span data-stu-id="b584f-109">Property</span></span>|<span data-ttu-id="b584f-110">类型</span><span class="sxs-lookup"><span data-stu-id="b584f-110">Type</span></span>|<span data-ttu-id="b584f-111">说明</span><span class="sxs-lookup"><span data-stu-id="b584f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b584f-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b584f-112">vpnConfigurationId</span></span>|<span data-ttu-id="b584f-113">String</span><span class="sxs-lookup"><span data-stu-id="b584f-113">String</span></span>|<span data-ttu-id="b584f-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="b584f-114">The VPN Configuration Id to apply for this app.</span></span>|
|<span data-ttu-id="b584f-115">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="b584f-115">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="b584f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b584f-116">Boolean</span></span>|<span data-ttu-id="b584f-117">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="b584f-117">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b584f-118">关系</span><span class="sxs-lookup"><span data-stu-id="b584f-118">Relationships</span></span>
<span data-ttu-id="b584f-119">无</span><span class="sxs-lookup"><span data-stu-id="b584f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b584f-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b584f-120">JSON Representation</span></span>
<span data-ttu-id="b584f-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b584f-121">Here is a JSON representation of the resource.</span></span>
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



