---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c427962565f7ecbe507e1eec8229e487885faf22
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360732"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="4e9b2-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="4e9b2-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="4e9b2-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4e9b2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e9b2-105">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="4e9b2-105">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="4e9b2-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="4e9b2-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e9b2-107">属性</span><span class="sxs-lookup"><span data-stu-id="4e9b2-107">Properties</span></span>
|<span data-ttu-id="4e9b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e9b2-108">Property</span></span>|<span data-ttu-id="4e9b2-109">类型</span><span class="sxs-lookup"><span data-stu-id="4e9b2-109">Type</span></span>|<span data-ttu-id="4e9b2-110">说明</span><span class="sxs-lookup"><span data-stu-id="4e9b2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e9b2-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="4e9b2-111">vpnConfigurationId</span></span>|<span data-ttu-id="4e9b2-112">String</span><span class="sxs-lookup"><span data-stu-id="4e9b2-112">String</span></span>|<span data-ttu-id="4e9b2-113">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="4e9b2-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e9b2-114">关系</span><span class="sxs-lookup"><span data-stu-id="4e9b2-114">Relationships</span></span>
<span data-ttu-id="4e9b2-115">无</span><span class="sxs-lookup"><span data-stu-id="4e9b2-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e9b2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4e9b2-116">JSON Representation</span></span>
<span data-ttu-id="4e9b2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4e9b2-117">Here is a JSON representation of the resource.</span></span>
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




