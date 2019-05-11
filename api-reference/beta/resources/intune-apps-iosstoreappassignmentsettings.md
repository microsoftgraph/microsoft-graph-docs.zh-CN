---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef89526a928ed2f8edb9a8c1ce26f199bdfdec77
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950415"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="26c1a-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="26c1a-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="26c1a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="26c1a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26c1a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="26c1a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26c1a-106">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="26c1a-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="26c1a-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="26c1a-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="26c1a-108">属性</span><span class="sxs-lookup"><span data-stu-id="26c1a-108">Properties</span></span>
|<span data-ttu-id="26c1a-109">属性</span><span class="sxs-lookup"><span data-stu-id="26c1a-109">Property</span></span>|<span data-ttu-id="26c1a-110">类型</span><span class="sxs-lookup"><span data-stu-id="26c1a-110">Type</span></span>|<span data-ttu-id="26c1a-111">说明</span><span class="sxs-lookup"><span data-stu-id="26c1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26c1a-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="26c1a-112">vpnConfigurationId</span></span>|<span data-ttu-id="26c1a-113">String</span><span class="sxs-lookup"><span data-stu-id="26c1a-113">String</span></span>|<span data-ttu-id="26c1a-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="26c1a-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26c1a-115">关系</span><span class="sxs-lookup"><span data-stu-id="26c1a-115">Relationships</span></span>
<span data-ttu-id="26c1a-116">无</span><span class="sxs-lookup"><span data-stu-id="26c1a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="26c1a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26c1a-117">JSON Representation</span></span>
<span data-ttu-id="26c1a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26c1a-118">Here is a JSON representation of the resource.</span></span>
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




