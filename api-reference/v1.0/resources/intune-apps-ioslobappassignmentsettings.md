---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc764c68fb6ad872fba7a7e12e3a53f92b9ba2c1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451619"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="fba2b-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="fba2b-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="fba2b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fba2b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fba2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fba2b-106">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="fba2b-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="fba2b-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fba2b-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fba2b-108">属性</span><span class="sxs-lookup"><span data-stu-id="fba2b-108">Properties</span></span>
|<span data-ttu-id="fba2b-109">属性</span><span class="sxs-lookup"><span data-stu-id="fba2b-109">Property</span></span>|<span data-ttu-id="fba2b-110">类型</span><span class="sxs-lookup"><span data-stu-id="fba2b-110">Type</span></span>|<span data-ttu-id="fba2b-111">说明</span><span class="sxs-lookup"><span data-stu-id="fba2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fba2b-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="fba2b-112">vpnConfigurationId</span></span>|<span data-ttu-id="fba2b-113">String</span><span class="sxs-lookup"><span data-stu-id="fba2b-113">String</span></span>|<span data-ttu-id="fba2b-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="fba2b-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fba2b-115">关系</span><span class="sxs-lookup"><span data-stu-id="fba2b-115">Relationships</span></span>
<span data-ttu-id="fba2b-116">无</span><span class="sxs-lookup"><span data-stu-id="fba2b-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fba2b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fba2b-117">JSON Representation</span></span>
<span data-ttu-id="fba2b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fba2b-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```







