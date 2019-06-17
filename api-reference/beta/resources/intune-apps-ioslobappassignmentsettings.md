---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c27321490cca54a912a5956026706e1d9b48d1d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991168"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="cde93-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="cde93-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="cde93-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cde93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cde93-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cde93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cde93-106">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="cde93-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="cde93-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="cde93-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cde93-108">属性</span><span class="sxs-lookup"><span data-stu-id="cde93-108">Properties</span></span>
|<span data-ttu-id="cde93-109">属性</span><span class="sxs-lookup"><span data-stu-id="cde93-109">Property</span></span>|<span data-ttu-id="cde93-110">类型</span><span class="sxs-lookup"><span data-stu-id="cde93-110">Type</span></span>|<span data-ttu-id="cde93-111">说明</span><span class="sxs-lookup"><span data-stu-id="cde93-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cde93-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="cde93-112">vpnConfigurationId</span></span>|<span data-ttu-id="cde93-113">String</span><span class="sxs-lookup"><span data-stu-id="cde93-113">String</span></span>|<span data-ttu-id="cde93-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="cde93-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cde93-115">关系</span><span class="sxs-lookup"><span data-stu-id="cde93-115">Relationships</span></span>
<span data-ttu-id="cde93-116">无</span><span class="sxs-lookup"><span data-stu-id="cde93-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cde93-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cde93-117">JSON Representation</span></span>
<span data-ttu-id="cde93-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cde93-118">Here is a JSON representation of the resource.</span></span>
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





