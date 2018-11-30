---
title: iosLobAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS LOB 移动应用的属性。
ms.openlocfilehash: 5c4380103c7d06032d3605d944fe8d420258d070
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042515"
---
# <a name="ioslobappassignmentsettings-resource-type"></a><span data-ttu-id="f1522-103">iosLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1522-103">iosLobAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="f1522-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f1522-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1522-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f1522-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1522-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f1522-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1522-107">包含用于为组分配 iOS LOB 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="f1522-107">Contains properties used to assign an iOS LOB mobile app to a group.</span></span>

<span data-ttu-id="f1522-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="f1522-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f1522-109">属性</span><span class="sxs-lookup"><span data-stu-id="f1522-109">Properties</span></span>
|<span data-ttu-id="f1522-110">属性</span><span class="sxs-lookup"><span data-stu-id="f1522-110">Property</span></span>|<span data-ttu-id="f1522-111">类型</span><span class="sxs-lookup"><span data-stu-id="f1522-111">Type</span></span>|<span data-ttu-id="f1522-112">说明</span><span class="sxs-lookup"><span data-stu-id="f1522-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1522-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="f1522-113">vpnConfigurationId</span></span>|<span data-ttu-id="f1522-114">String</span><span class="sxs-lookup"><span data-stu-id="f1522-114">String</span></span>|<span data-ttu-id="f1522-115">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="f1522-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1522-116">关系</span><span class="sxs-lookup"><span data-stu-id="f1522-116">Relationships</span></span>
<span data-ttu-id="f1522-117">无</span><span class="sxs-lookup"><span data-stu-id="f1522-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1522-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1522-118">JSON Representation</span></span>
<span data-ttu-id="f1522-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1522-119">Here is a JSON representation of the resource.</span></span>
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





