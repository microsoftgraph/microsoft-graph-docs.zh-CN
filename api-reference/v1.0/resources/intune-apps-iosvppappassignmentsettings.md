---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: tfitzmac
ms.openlocfilehash: 65a143c1f6cc9eed4dfdc6dabeb6f9379517277c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310246"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="45c1e-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="45c1e-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="45c1e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="45c1e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45c1e-105">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="45c1e-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="45c1e-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="45c1e-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45c1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="45c1e-107">Properties</span></span>
|<span data-ttu-id="45c1e-108">属性</span><span class="sxs-lookup"><span data-stu-id="45c1e-108">Property</span></span>|<span data-ttu-id="45c1e-109">类型</span><span class="sxs-lookup"><span data-stu-id="45c1e-109">Type</span></span>|<span data-ttu-id="45c1e-110">说明</span><span class="sxs-lookup"><span data-stu-id="45c1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45c1e-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="45c1e-111">useDeviceLicensing</span></span>|<span data-ttu-id="45c1e-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="45c1e-112">Boolean</span></span>|<span data-ttu-id="45c1e-113">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="45c1e-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="45c1e-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="45c1e-114">vpnConfigurationId</span></span>|<span data-ttu-id="45c1e-115">String</span><span class="sxs-lookup"><span data-stu-id="45c1e-115">String</span></span>|<span data-ttu-id="45c1e-116">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="45c1e-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45c1e-117">关系</span><span class="sxs-lookup"><span data-stu-id="45c1e-117">Relationships</span></span>
<span data-ttu-id="45c1e-118">无</span><span class="sxs-lookup"><span data-stu-id="45c1e-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45c1e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45c1e-119">JSON Representation</span></span>
<span data-ttu-id="45c1e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45c1e-120">Here is a JSON representation of the resource.</span></span>
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



