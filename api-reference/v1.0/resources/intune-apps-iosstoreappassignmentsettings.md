---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b7a0b76ff2ac66ecffc7b55e0b4d28f234cbec43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029139"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="fb3ad-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb3ad-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="fb3ad-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb3ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb3ad-105">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="fb3ad-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="fb3ad-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fb3ad-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fb3ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="fb3ad-107">Properties</span></span>
|<span data-ttu-id="fb3ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb3ad-108">Property</span></span>|<span data-ttu-id="fb3ad-109">类型</span><span class="sxs-lookup"><span data-stu-id="fb3ad-109">Type</span></span>|<span data-ttu-id="fb3ad-110">说明</span><span class="sxs-lookup"><span data-stu-id="fb3ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb3ad-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="fb3ad-111">vpnConfigurationId</span></span>|<span data-ttu-id="fb3ad-112">String</span><span class="sxs-lookup"><span data-stu-id="fb3ad-112">String</span></span>|<span data-ttu-id="fb3ad-113">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="fb3ad-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb3ad-114">关系</span><span class="sxs-lookup"><span data-stu-id="fb3ad-114">Relationships</span></span>
<span data-ttu-id="fb3ad-115">无</span><span class="sxs-lookup"><span data-stu-id="fb3ad-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb3ad-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb3ad-116">JSON Representation</span></span>
<span data-ttu-id="fb3ad-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb3ad-117">Here is a JSON representation of the resource.</span></span>
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



