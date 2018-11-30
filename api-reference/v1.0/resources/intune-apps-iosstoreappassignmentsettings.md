---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
ms.openlocfilehash: ec26e3367aabedfca009db003468164c468e9ecd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008801"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="eca16-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="eca16-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="eca16-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eca16-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eca16-105">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="eca16-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="eca16-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="eca16-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eca16-107">属性</span><span class="sxs-lookup"><span data-stu-id="eca16-107">Properties</span></span>
|<span data-ttu-id="eca16-108">属性</span><span class="sxs-lookup"><span data-stu-id="eca16-108">Property</span></span>|<span data-ttu-id="eca16-109">类型</span><span class="sxs-lookup"><span data-stu-id="eca16-109">Type</span></span>|<span data-ttu-id="eca16-110">说明</span><span class="sxs-lookup"><span data-stu-id="eca16-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca16-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="eca16-111">vpnConfigurationId</span></span>|<span data-ttu-id="eca16-112">String</span><span class="sxs-lookup"><span data-stu-id="eca16-112">String</span></span>|<span data-ttu-id="eca16-113">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="eca16-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eca16-114">关系</span><span class="sxs-lookup"><span data-stu-id="eca16-114">Relationships</span></span>
<span data-ttu-id="eca16-115">无</span><span class="sxs-lookup"><span data-stu-id="eca16-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eca16-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eca16-116">JSON Representation</span></span>
<span data-ttu-id="eca16-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eca16-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



