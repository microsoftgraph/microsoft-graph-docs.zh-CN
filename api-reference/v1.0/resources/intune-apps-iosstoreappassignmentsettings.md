---
title: iosStoreAppAssignmentSettings 资源类型
description: 包含用于为组分配 iOS 应用商店移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 111f7a1f1a5b48e46e00ee98f95eaa7397bf6ab4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075033"
---
# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="06523-103">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="06523-103">iosStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="06523-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06523-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06523-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06523-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06523-106">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="06523-106">Contains properties used to assign an iOS Store mobile app to a group.</span></span>


<span data-ttu-id="06523-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="06523-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06523-108">属性</span><span class="sxs-lookup"><span data-stu-id="06523-108">Properties</span></span>
|<span data-ttu-id="06523-109">属性</span><span class="sxs-lookup"><span data-stu-id="06523-109">Property</span></span>|<span data-ttu-id="06523-110">类型</span><span class="sxs-lookup"><span data-stu-id="06523-110">Type</span></span>|<span data-ttu-id="06523-111">说明</span><span class="sxs-lookup"><span data-stu-id="06523-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06523-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="06523-112">vpnConfigurationId</span></span>|<span data-ttu-id="06523-113">String</span><span class="sxs-lookup"><span data-stu-id="06523-113">String</span></span>|<span data-ttu-id="06523-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="06523-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06523-115">关系</span><span class="sxs-lookup"><span data-stu-id="06523-115">Relationships</span></span>
<span data-ttu-id="06523-116">无</span><span class="sxs-lookup"><span data-stu-id="06523-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06523-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06523-117">JSON Representation</span></span>
<span data-ttu-id="06523-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06523-118">Here is a JSON representation of the resource.</span></span>
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









