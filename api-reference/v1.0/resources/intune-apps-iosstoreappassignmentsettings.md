---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: afbb1ecf250b67563f965aae6d5e7e39ebc9083d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531210"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="b9a74-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9a74-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="b9a74-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9a74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9a74-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9a74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a74-106">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="b9a74-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="b9a74-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b9a74-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9a74-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9a74-108">Properties</span></span>
|<span data-ttu-id="b9a74-109">属性</span><span class="sxs-lookup"><span data-stu-id="b9a74-109">Property</span></span>|<span data-ttu-id="b9a74-110">类型</span><span class="sxs-lookup"><span data-stu-id="b9a74-110">Type</span></span>|<span data-ttu-id="b9a74-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9a74-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a74-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="b9a74-112">vpnConfigurationId</span></span>|<span data-ttu-id="b9a74-113">String</span><span class="sxs-lookup"><span data-stu-id="b9a74-113">String</span></span>|<span data-ttu-id="b9a74-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="b9a74-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9a74-115">关系</span><span class="sxs-lookup"><span data-stu-id="b9a74-115">Relationships</span></span>
<span data-ttu-id="b9a74-116">无</span><span class="sxs-lookup"><span data-stu-id="b9a74-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9a74-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9a74-117">JSON Representation</span></span>
<span data-ttu-id="b9a74-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9a74-118">Here is a JSON representation of the resource.</span></span>
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




