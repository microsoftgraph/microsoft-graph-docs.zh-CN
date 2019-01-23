---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4f2d954b016ed2a59938974f995d9bd040bc69b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404349"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="17dd3-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="17dd3-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="17dd3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="17dd3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="17dd3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="17dd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17dd3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="17dd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17dd3-107">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="17dd3-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>


<span data-ttu-id="17dd3-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="17dd3-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="17dd3-109">属性</span><span class="sxs-lookup"><span data-stu-id="17dd3-109">Properties</span></span>
|<span data-ttu-id="17dd3-110">属性</span><span class="sxs-lookup"><span data-stu-id="17dd3-110">Property</span></span>|<span data-ttu-id="17dd3-111">类型</span><span class="sxs-lookup"><span data-stu-id="17dd3-111">Type</span></span>|<span data-ttu-id="17dd3-112">说明</span><span class="sxs-lookup"><span data-stu-id="17dd3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17dd3-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="17dd3-113">vpnConfigurationId</span></span>|<span data-ttu-id="17dd3-114">String</span><span class="sxs-lookup"><span data-stu-id="17dd3-114">String</span></span>|<span data-ttu-id="17dd3-115">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="17dd3-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17dd3-116">关系</span><span class="sxs-lookup"><span data-stu-id="17dd3-116">Relationships</span></span>
<span data-ttu-id="17dd3-117">无</span><span class="sxs-lookup"><span data-stu-id="17dd3-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17dd3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17dd3-118">JSON Representation</span></span>
<span data-ttu-id="17dd3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17dd3-119">Here is a JSON representation of the resource.</span></span>
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




