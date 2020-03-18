---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 62dab652d6b4f9b16d8f95d6820f3361835f4711
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768924"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="9ea1d-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ea1d-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="9ea1d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ea1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ea1d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ea1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ea1d-106">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="9ea1d-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="9ea1d-107">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="9ea1d-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9ea1d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ea1d-108">Properties</span></span>
|<span data-ttu-id="9ea1d-109">属性</span><span class="sxs-lookup"><span data-stu-id="9ea1d-109">Property</span></span>|<span data-ttu-id="9ea1d-110">类型</span><span class="sxs-lookup"><span data-stu-id="9ea1d-110">Type</span></span>|<span data-ttu-id="9ea1d-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ea1d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ea1d-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="9ea1d-112">useDeviceContext</span></span>|<span data-ttu-id="9ea1d-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="9ea1d-113">Boolean</span></span>|<span data-ttu-id="9ea1d-114">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="9ea1d-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ea1d-115">关系</span><span class="sxs-lookup"><span data-stu-id="9ea1d-115">Relationships</span></span>
<span data-ttu-id="9ea1d-116">无</span><span class="sxs-lookup"><span data-stu-id="9ea1d-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ea1d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ea1d-117">JSON Representation</span></span>
<span data-ttu-id="9ea1d-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ea1d-118">Here is a JSON representation of the resource.</span></span>
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



