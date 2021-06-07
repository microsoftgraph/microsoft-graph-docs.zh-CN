---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e364ae3ef38bd01376d937c6538ce00c39ba6172
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755152"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="a2444-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2444-103">iosLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="a2444-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2444-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2444-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2444-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2444-106">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="a2444-106">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="a2444-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a2444-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2444-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2444-108">Properties</span></span>
|<span data-ttu-id="a2444-109">属性</span><span class="sxs-lookup"><span data-stu-id="a2444-109">Property</span></span>|<span data-ttu-id="a2444-110">类型</span><span class="sxs-lookup"><span data-stu-id="a2444-110">Type</span></span>|<span data-ttu-id="a2444-111">Description</span><span class="sxs-lookup"><span data-stu-id="a2444-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2444-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a2444-112">vpnConfigurationId</span></span>|<span data-ttu-id="a2444-113">String</span><span class="sxs-lookup"><span data-stu-id="a2444-113">String</span></span>|<span data-ttu-id="a2444-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="a2444-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2444-115">关系</span><span class="sxs-lookup"><span data-stu-id="a2444-115">Relationships</span></span>
<span data-ttu-id="a2444-116">无</span><span class="sxs-lookup"><span data-stu-id="a2444-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2444-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2444-117">JSON Representation</span></span>
<span data-ttu-id="a2444-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2444-118">Here is a JSON representation of the resource.</span></span>
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




