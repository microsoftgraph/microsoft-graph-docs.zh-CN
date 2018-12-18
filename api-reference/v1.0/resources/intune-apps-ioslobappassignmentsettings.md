---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: tfitzmac
ms.openlocfilehash: 78de511bdbdf2e4a8b16d9ce32a790329d2eb3c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306088"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="85a93-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="85a93-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="85a93-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="85a93-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85a93-105">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="85a93-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="85a93-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="85a93-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="85a93-107">属性</span><span class="sxs-lookup"><span data-stu-id="85a93-107">Properties</span></span>
|<span data-ttu-id="85a93-108">属性</span><span class="sxs-lookup"><span data-stu-id="85a93-108">Property</span></span>|<span data-ttu-id="85a93-109">类型</span><span class="sxs-lookup"><span data-stu-id="85a93-109">Type</span></span>|<span data-ttu-id="85a93-110">说明</span><span class="sxs-lookup"><span data-stu-id="85a93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85a93-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="85a93-111">vpnConfigurationId</span></span>|<span data-ttu-id="85a93-112">String</span><span class="sxs-lookup"><span data-stu-id="85a93-112">String</span></span>|<span data-ttu-id="85a93-113">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="85a93-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85a93-114">关系</span><span class="sxs-lookup"><span data-stu-id="85a93-114">Relationships</span></span>
<span data-ttu-id="85a93-115">无</span><span class="sxs-lookup"><span data-stu-id="85a93-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85a93-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85a93-116">JSON Representation</span></span>
<span data-ttu-id="85a93-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85a93-117">Here is a JSON representation of the resource.</span></span>
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



