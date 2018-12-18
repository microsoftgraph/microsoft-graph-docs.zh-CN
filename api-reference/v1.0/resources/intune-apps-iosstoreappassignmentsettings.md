---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: tfitzmac
ms.openlocfilehash: 2f37a4b0cbcacb9e7223793628422fb7bad8a28c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306081"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="e0053-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0053-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e0053-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0053-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0053-105">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="e0053-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="e0053-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e0053-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0053-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0053-107">Properties</span></span>
|<span data-ttu-id="e0053-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0053-108">Property</span></span>|<span data-ttu-id="e0053-109">类型</span><span class="sxs-lookup"><span data-stu-id="e0053-109">Type</span></span>|<span data-ttu-id="e0053-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0053-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0053-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="e0053-111">vpnConfigurationId</span></span>|<span data-ttu-id="e0053-112">String</span><span class="sxs-lookup"><span data-stu-id="e0053-112">String</span></span>|<span data-ttu-id="e0053-113">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="e0053-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0053-114">关系</span><span class="sxs-lookup"><span data-stu-id="e0053-114">Relationships</span></span>
<span data-ttu-id="e0053-115">无</span><span class="sxs-lookup"><span data-stu-id="e0053-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0053-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0053-116">JSON Representation</span></span>
<span data-ttu-id="e0053-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0053-117">Here is a JSON representation of the resource.</span></span>
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



