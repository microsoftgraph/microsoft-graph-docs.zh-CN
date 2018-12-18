---
title: iosVppAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS APP 移动应用的属性。
author: tfitzmac
ms.openlocfilehash: 9e1233c9d5a33876da64ab3c75419c322ee83931
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321327"
---
# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="8e108-103">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e108-103">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8e108-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8e108-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e108-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e108-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e108-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8e108-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e108-107">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="8e108-107">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="8e108-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8e108-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8e108-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e108-109">Properties</span></span>
|<span data-ttu-id="8e108-110">属性</span><span class="sxs-lookup"><span data-stu-id="8e108-110">Property</span></span>|<span data-ttu-id="8e108-111">类型</span><span class="sxs-lookup"><span data-stu-id="8e108-111">Type</span></span>|<span data-ttu-id="8e108-112">说明</span><span class="sxs-lookup"><span data-stu-id="8e108-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e108-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="8e108-113">useDeviceLicensing</span></span>|<span data-ttu-id="8e108-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="8e108-114">Boolean</span></span>|<span data-ttu-id="8e108-115">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="8e108-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="8e108-116">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="8e108-116">vpnConfigurationId</span></span>|<span data-ttu-id="8e108-117">String</span><span class="sxs-lookup"><span data-stu-id="8e108-117">String</span></span>|<span data-ttu-id="8e108-118">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="8e108-118">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e108-119">关系</span><span class="sxs-lookup"><span data-stu-id="8e108-119">Relationships</span></span>
<span data-ttu-id="8e108-120">无</span><span class="sxs-lookup"><span data-stu-id="8e108-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8e108-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e108-121">JSON Representation</span></span>
<span data-ttu-id="8e108-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e108-122">Here is a JSON representation of the resource.</span></span>
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





