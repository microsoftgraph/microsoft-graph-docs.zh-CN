---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 39f007a88fc05504fc83b624a886c719ffe08ba3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962269"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="bf6fe-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf6fe-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="bf6fe-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bf6fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf6fe-105">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="bf6fe-105">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="bf6fe-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="bf6fe-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf6fe-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf6fe-107">Properties</span></span>
|<span data-ttu-id="bf6fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="bf6fe-108">Property</span></span>|<span data-ttu-id="bf6fe-109">类型</span><span class="sxs-lookup"><span data-stu-id="bf6fe-109">Type</span></span>|<span data-ttu-id="bf6fe-110">说明</span><span class="sxs-lookup"><span data-stu-id="bf6fe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf6fe-111">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="bf6fe-111">vpnConfigurationId</span></span>|<span data-ttu-id="bf6fe-112">String</span><span class="sxs-lookup"><span data-stu-id="bf6fe-112">String</span></span>|<span data-ttu-id="bf6fe-113">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="bf6fe-113">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf6fe-114">关系</span><span class="sxs-lookup"><span data-stu-id="bf6fe-114">Relationships</span></span>
<span data-ttu-id="bf6fe-115">无</span><span class="sxs-lookup"><span data-stu-id="bf6fe-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf6fe-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf6fe-116">JSON Representation</span></span>
<span data-ttu-id="bf6fe-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf6fe-117">Here is a JSON representation of the resource.</span></span>
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



