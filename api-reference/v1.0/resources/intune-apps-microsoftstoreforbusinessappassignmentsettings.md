---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbfb271e8cfb0d019a0e127d1ad81ee033544a17
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43457888"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="45258-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="45258-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="45258-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45258-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45258-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45258-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45258-106">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="45258-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="45258-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="45258-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="45258-108">属性</span><span class="sxs-lookup"><span data-stu-id="45258-108">Properties</span></span>
|<span data-ttu-id="45258-109">属性</span><span class="sxs-lookup"><span data-stu-id="45258-109">Property</span></span>|<span data-ttu-id="45258-110">类型</span><span class="sxs-lookup"><span data-stu-id="45258-110">Type</span></span>|<span data-ttu-id="45258-111">说明</span><span class="sxs-lookup"><span data-stu-id="45258-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45258-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="45258-112">useDeviceContext</span></span>|<span data-ttu-id="45258-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="45258-113">Boolean</span></span>|<span data-ttu-id="45258-114">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="45258-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45258-115">关系</span><span class="sxs-lookup"><span data-stu-id="45258-115">Relationships</span></span>
<span data-ttu-id="45258-116">无</span><span class="sxs-lookup"><span data-stu-id="45258-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45258-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45258-117">JSON Representation</span></span>
<span data-ttu-id="45258-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45258-118">Here is a JSON representation of the resource.</span></span>
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







