---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c8f1dadc7a302c3b4b78f0fc9e278e9285ecbcc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172308"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="d0c32-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0c32-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="d0c32-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0c32-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0c32-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0c32-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0c32-106">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="d0c32-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="d0c32-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d0c32-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0c32-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0c32-108">Properties</span></span>
|<span data-ttu-id="d0c32-109">属性</span><span class="sxs-lookup"><span data-stu-id="d0c32-109">Property</span></span>|<span data-ttu-id="d0c32-110">类型</span><span class="sxs-lookup"><span data-stu-id="d0c32-110">Type</span></span>|<span data-ttu-id="d0c32-111">说明</span><span class="sxs-lookup"><span data-stu-id="d0c32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0c32-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d0c32-112">vpnConfigurationId</span></span>|<span data-ttu-id="d0c32-113">String</span><span class="sxs-lookup"><span data-stu-id="d0c32-113">String</span></span>|<span data-ttu-id="d0c32-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="d0c32-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0c32-115">关系</span><span class="sxs-lookup"><span data-stu-id="d0c32-115">Relationships</span></span>
<span data-ttu-id="d0c32-116">无</span><span class="sxs-lookup"><span data-stu-id="d0c32-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0c32-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0c32-117">JSON Representation</span></span>
<span data-ttu-id="d0c32-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0c32-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```




