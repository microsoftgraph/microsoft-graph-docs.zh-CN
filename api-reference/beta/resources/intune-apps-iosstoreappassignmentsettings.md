---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcda842b97c6c7baf257145f0333c6194e97a403
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806424"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="f0fa6-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0fa6-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f0fa6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0fa6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0fa6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0fa6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0fa6-106">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="f0fa6-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="f0fa6-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f0fa6-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f0fa6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0fa6-108">Properties</span></span>
|<span data-ttu-id="f0fa6-109">属性</span><span class="sxs-lookup"><span data-stu-id="f0fa6-109">Property</span></span>|<span data-ttu-id="f0fa6-110">类型</span><span class="sxs-lookup"><span data-stu-id="f0fa6-110">Type</span></span>|<span data-ttu-id="f0fa6-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0fa6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0fa6-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f0fa6-112">vpnConfigurationId</span></span>|<span data-ttu-id="f0fa6-113">String</span><span class="sxs-lookup"><span data-stu-id="f0fa6-113">String</span></span>|<span data-ttu-id="f0fa6-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="f0fa6-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f0fa6-115">关系</span><span class="sxs-lookup"><span data-stu-id="f0fa6-115">Relationships</span></span>
<span data-ttu-id="f0fa6-116">无</span><span class="sxs-lookup"><span data-stu-id="f0fa6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0fa6-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0fa6-117">JSON Representation</span></span>
<span data-ttu-id="f0fa6-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0fa6-118">Here is a JSON representation of the resource.</span></span>
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





