---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e221ceb67789f9d96195a31bd7eba8f37a9df6bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917641"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="8aad9-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8aad9-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8aad9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8aad9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8aad9-105">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="8aad9-105">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="8aad9-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8aad9-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8aad9-107">属性</span><span class="sxs-lookup"><span data-stu-id="8aad9-107">Properties</span></span>
|<span data-ttu-id="8aad9-108">属性</span><span class="sxs-lookup"><span data-stu-id="8aad9-108">Property</span></span>|<span data-ttu-id="8aad9-109">类型</span><span class="sxs-lookup"><span data-stu-id="8aad9-109">Type</span></span>|<span data-ttu-id="8aad9-110">说明</span><span class="sxs-lookup"><span data-stu-id="8aad9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aad9-111">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8aad9-111">useDeviceLicensing</span></span>|<span data-ttu-id="8aad9-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="8aad9-112">Boolean</span></span>|<span data-ttu-id="8aad9-113">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="8aad9-113">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="8aad9-114">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="8aad9-114">vpnConfigurationId</span></span>|<span data-ttu-id="8aad9-115">String</span><span class="sxs-lookup"><span data-stu-id="8aad9-115">String</span></span>|<span data-ttu-id="8aad9-116">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="8aad9-116">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8aad9-117">关系</span><span class="sxs-lookup"><span data-stu-id="8aad9-117">Relationships</span></span>
<span data-ttu-id="8aad9-118">无</span><span class="sxs-lookup"><span data-stu-id="8aad9-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8aad9-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8aad9-119">JSON Representation</span></span>
<span data-ttu-id="8aad9-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8aad9-120">Here is a JSON representation of the resource.</span></span>
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



