---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e347bc5967ccd732530cbe9fde5367d354c9a81b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028978"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a5429-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5429-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a5429-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a5429-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5429-105">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="a5429-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="a5429-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a5429-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a5429-107">属性</span><span class="sxs-lookup"><span data-stu-id="a5429-107">Properties</span></span>
|<span data-ttu-id="a5429-108">属性</span><span class="sxs-lookup"><span data-stu-id="a5429-108">Property</span></span>|<span data-ttu-id="a5429-109">类型</span><span class="sxs-lookup"><span data-stu-id="a5429-109">Type</span></span>|<span data-ttu-id="a5429-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5429-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5429-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a5429-111">useDeviceContext</span></span>|<span data-ttu-id="a5429-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="a5429-112">Boolean</span></span>|<span data-ttu-id="a5429-113">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="a5429-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5429-114">关系</span><span class="sxs-lookup"><span data-stu-id="a5429-114">Relationships</span></span>
<span data-ttu-id="a5429-115">无</span><span class="sxs-lookup"><span data-stu-id="a5429-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5429-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5429-116">JSON Representation</span></span>
<span data-ttu-id="a5429-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5429-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



