---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32186cd4c5b4321d668e350b5f03ec6e127399cd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094454"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="7aafa-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="7aafa-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="7aafa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aafa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7aafa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7aafa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aafa-106">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="7aafa-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="7aafa-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="7aafa-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7aafa-108">属性</span><span class="sxs-lookup"><span data-stu-id="7aafa-108">Properties</span></span>
|<span data-ttu-id="7aafa-109">属性</span><span class="sxs-lookup"><span data-stu-id="7aafa-109">Property</span></span>|<span data-ttu-id="7aafa-110">类型</span><span class="sxs-lookup"><span data-stu-id="7aafa-110">Type</span></span>|<span data-ttu-id="7aafa-111">说明</span><span class="sxs-lookup"><span data-stu-id="7aafa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aafa-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="7aafa-112">useDeviceContext</span></span>|<span data-ttu-id="7aafa-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="7aafa-113">Boolean</span></span>|<span data-ttu-id="7aafa-114">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="7aafa-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7aafa-115">关系</span><span class="sxs-lookup"><span data-stu-id="7aafa-115">Relationships</span></span>
<span data-ttu-id="7aafa-116">无</span><span class="sxs-lookup"><span data-stu-id="7aafa-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7aafa-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7aafa-117">JSON Representation</span></span>
<span data-ttu-id="7aafa-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7aafa-118">Here is a JSON representation of the resource.</span></span>
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









