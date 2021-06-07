---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0b47c71f151e0cb83f9e682789fcde3a7b69ae4b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756069"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="5cc38-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="5cc38-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="5cc38-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cc38-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cc38-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5cc38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cc38-106">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="5cc38-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="5cc38-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="5cc38-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5cc38-108">属性</span><span class="sxs-lookup"><span data-stu-id="5cc38-108">Properties</span></span>
|<span data-ttu-id="5cc38-109">属性</span><span class="sxs-lookup"><span data-stu-id="5cc38-109">Property</span></span>|<span data-ttu-id="5cc38-110">类型</span><span class="sxs-lookup"><span data-stu-id="5cc38-110">Type</span></span>|<span data-ttu-id="5cc38-111">Description</span><span class="sxs-lookup"><span data-stu-id="5cc38-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cc38-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="5cc38-112">vpnConfigurationId</span></span>|<span data-ttu-id="5cc38-113">String</span><span class="sxs-lookup"><span data-stu-id="5cc38-113">String</span></span>|<span data-ttu-id="5cc38-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="5cc38-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5cc38-115">关系</span><span class="sxs-lookup"><span data-stu-id="5cc38-115">Relationships</span></span>
<span data-ttu-id="5cc38-116">无</span><span class="sxs-lookup"><span data-stu-id="5cc38-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5cc38-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5cc38-117">JSON Representation</span></span>
<span data-ttu-id="5cc38-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cc38-118">Here is a JSON representation of the resource.</span></span>
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




