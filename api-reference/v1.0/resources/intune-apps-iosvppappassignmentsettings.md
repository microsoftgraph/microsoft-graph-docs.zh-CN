---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
ms.openlocfilehash: 6fc529fe1aeea6bdbef46ad0cd97fb5830250b4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010683"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="96523-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="96523-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="96523-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="96523-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96523-105">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="96523-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="96523-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="96523-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96523-107">属性</span><span class="sxs-lookup"><span data-stu-id="96523-107">Properties</span></span>
|<span data-ttu-id="96523-108">属性</span><span class="sxs-lookup"><span data-stu-id="96523-108">Property</span></span>|<span data-ttu-id="96523-109">类型</span><span class="sxs-lookup"><span data-stu-id="96523-109">Type</span></span>|<span data-ttu-id="96523-110">说明</span><span class="sxs-lookup"><span data-stu-id="96523-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96523-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="96523-111">useDeviceLicensing</span></span>|<span data-ttu-id="96523-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="96523-112">Boolean</span></span>|<span data-ttu-id="96523-113">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="96523-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="96523-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="96523-114">vpnConfigurationId</span></span>|<span data-ttu-id="96523-115">String</span><span class="sxs-lookup"><span data-stu-id="96523-115">String</span></span>|<span data-ttu-id="96523-116">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="96523-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96523-117">关系</span><span class="sxs-lookup"><span data-stu-id="96523-117">Relationships</span></span>
<span data-ttu-id="96523-118">无</span><span class="sxs-lookup"><span data-stu-id="96523-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96523-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96523-119">JSON Representation</span></span>
<span data-ttu-id="96523-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96523-120">Here is a JSON representation of the resource.</span></span>
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



