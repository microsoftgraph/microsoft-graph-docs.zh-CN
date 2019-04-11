---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48bac2fcc8dd8c7da65c3ee138aabaaf5649b356
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795182"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="2f25c-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f25c-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="2f25c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f25c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f25c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f25c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f25c-106">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="2f25c-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="2f25c-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="2f25c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2f25c-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f25c-108">Properties</span></span>
|<span data-ttu-id="2f25c-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f25c-109">Property</span></span>|<span data-ttu-id="2f25c-110">类型</span><span class="sxs-lookup"><span data-stu-id="2f25c-110">Type</span></span>|<span data-ttu-id="2f25c-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f25c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f25c-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="2f25c-112">vpnConfigurationId</span></span>|<span data-ttu-id="2f25c-113">String</span><span class="sxs-lookup"><span data-stu-id="2f25c-113">String</span></span>|<span data-ttu-id="2f25c-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="2f25c-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f25c-115">关系</span><span class="sxs-lookup"><span data-stu-id="2f25c-115">Relationships</span></span>
<span data-ttu-id="2f25c-116">无</span><span class="sxs-lookup"><span data-stu-id="2f25c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f25c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f25c-117">JSON Representation</span></span>
<span data-ttu-id="2f25c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f25c-118">Here is a JSON representation of the resource.</span></span>
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





