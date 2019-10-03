---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 625eb4d6df63cfacab7e263c305d35f7de25fdd1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368132"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="c5aaf-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5aaf-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c5aaf-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c5aaf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5aaf-105">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="c5aaf-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="c5aaf-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c5aaf-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c5aaf-107">属性</span><span class="sxs-lookup"><span data-stu-id="c5aaf-107">Properties</span></span>
|<span data-ttu-id="c5aaf-108">属性</span><span class="sxs-lookup"><span data-stu-id="c5aaf-108">Property</span></span>|<span data-ttu-id="c5aaf-109">类型</span><span class="sxs-lookup"><span data-stu-id="c5aaf-109">Type</span></span>|<span data-ttu-id="c5aaf-110">说明</span><span class="sxs-lookup"><span data-stu-id="c5aaf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5aaf-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="c5aaf-111">useDeviceContext</span></span>|<span data-ttu-id="c5aaf-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="c5aaf-112">Boolean</span></span>|<span data-ttu-id="c5aaf-113">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="c5aaf-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5aaf-114">关系</span><span class="sxs-lookup"><span data-stu-id="c5aaf-114">Relationships</span></span>
<span data-ttu-id="c5aaf-115">无</span><span class="sxs-lookup"><span data-stu-id="c5aaf-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5aaf-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5aaf-116">JSON Representation</span></span>
<span data-ttu-id="c5aaf-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5aaf-117">Here is a JSON representation of the resource.</span></span>
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




