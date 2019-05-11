---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8855a73f148e9e80b2bb82ba16f784a4ac52441f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950058"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="a50be-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="a50be-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a50be-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a50be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a50be-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a50be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a50be-106">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="a50be-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="a50be-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="a50be-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a50be-108">属性</span><span class="sxs-lookup"><span data-stu-id="a50be-108">Properties</span></span>
|<span data-ttu-id="a50be-109">属性</span><span class="sxs-lookup"><span data-stu-id="a50be-109">Property</span></span>|<span data-ttu-id="a50be-110">类型</span><span class="sxs-lookup"><span data-stu-id="a50be-110">Type</span></span>|<span data-ttu-id="a50be-111">说明</span><span class="sxs-lookup"><span data-stu-id="a50be-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a50be-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="a50be-112">useDeviceContext</span></span>|<span data-ttu-id="a50be-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="a50be-113">Boolean</span></span>|<span data-ttu-id="a50be-114">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="a50be-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a50be-115">关系</span><span class="sxs-lookup"><span data-stu-id="a50be-115">Relationships</span></span>
<span data-ttu-id="a50be-116">无</span><span class="sxs-lookup"><span data-stu-id="a50be-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a50be-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a50be-117">JSON Representation</span></span>
<span data-ttu-id="a50be-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a50be-118">Here is a JSON representation of the resource.</span></span>
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




