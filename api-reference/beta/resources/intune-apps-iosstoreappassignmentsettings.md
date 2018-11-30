---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
ms.openlocfilehash: 5509227dd28d7d89c9afcd8c6abeb89db6096ddf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046085"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="9d42f-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d42f-103">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9d42f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d42f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d42f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d42f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d42f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9d42f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d42f-107">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="9d42f-107">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="9d42f-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9d42f-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9d42f-109">属性</span><span class="sxs-lookup"><span data-stu-id="9d42f-109">Properties</span></span>
|<span data-ttu-id="9d42f-110">属性</span><span class="sxs-lookup"><span data-stu-id="9d42f-110">Property</span></span>|<span data-ttu-id="9d42f-111">类型</span><span class="sxs-lookup"><span data-stu-id="9d42f-111">Type</span></span>|<span data-ttu-id="9d42f-112">说明</span><span class="sxs-lookup"><span data-stu-id="9d42f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d42f-113">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9d42f-113">vpnConfigurationId</span></span>|<span data-ttu-id="9d42f-114">String</span><span class="sxs-lookup"><span data-stu-id="9d42f-114">String</span></span>|<span data-ttu-id="9d42f-115">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="9d42f-115">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d42f-116">关系</span><span class="sxs-lookup"><span data-stu-id="9d42f-116">Relationships</span></span>
<span data-ttu-id="9d42f-117">无</span><span class="sxs-lookup"><span data-stu-id="9d42f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9d42f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d42f-118">JSON Representation</span></span>
<span data-ttu-id="9d42f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d42f-119">Here is a JSON representation of the resource.</span></span>
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





