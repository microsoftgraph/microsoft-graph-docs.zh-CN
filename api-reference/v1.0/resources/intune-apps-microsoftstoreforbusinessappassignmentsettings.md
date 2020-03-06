---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3f742b443e0f7b8ab360dbb20022b94837aca051
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531128"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="aa83c-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa83c-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="aa83c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa83c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa83c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa83c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa83c-106">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="aa83c-106">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="aa83c-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="aa83c-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa83c-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa83c-108">Properties</span></span>
|<span data-ttu-id="aa83c-109">属性</span><span class="sxs-lookup"><span data-stu-id="aa83c-109">Property</span></span>|<span data-ttu-id="aa83c-110">类型</span><span class="sxs-lookup"><span data-stu-id="aa83c-110">Type</span></span>|<span data-ttu-id="aa83c-111">说明</span><span class="sxs-lookup"><span data-stu-id="aa83c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa83c-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="aa83c-112">useDeviceContext</span></span>|<span data-ttu-id="aa83c-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="aa83c-113">Boolean</span></span>|<span data-ttu-id="aa83c-114">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="aa83c-114">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa83c-115">关系</span><span class="sxs-lookup"><span data-stu-id="aa83c-115">Relationships</span></span>
<span data-ttu-id="aa83c-116">无</span><span class="sxs-lookup"><span data-stu-id="aa83c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa83c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa83c-117">JSON Representation</span></span>
<span data-ttu-id="aa83c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa83c-118">Here is a JSON representation of the resource.</span></span>
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




