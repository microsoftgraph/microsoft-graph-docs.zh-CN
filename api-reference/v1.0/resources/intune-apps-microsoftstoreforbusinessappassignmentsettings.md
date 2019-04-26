---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1aed45ba54abdcb25f5436beeb2a03f53b9dbae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558116"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="dc627-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="dc627-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="dc627-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc627-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc627-105">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="dc627-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="dc627-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="dc627-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dc627-107">属性</span><span class="sxs-lookup"><span data-stu-id="dc627-107">Properties</span></span>
|<span data-ttu-id="dc627-108">属性</span><span class="sxs-lookup"><span data-stu-id="dc627-108">Property</span></span>|<span data-ttu-id="dc627-109">类型</span><span class="sxs-lookup"><span data-stu-id="dc627-109">Type</span></span>|<span data-ttu-id="dc627-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc627-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc627-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="dc627-111">useDeviceContext</span></span>|<span data-ttu-id="dc627-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="dc627-112">Boolean</span></span>|<span data-ttu-id="dc627-113">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="dc627-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc627-114">关系</span><span class="sxs-lookup"><span data-stu-id="dc627-114">Relationships</span></span>
<span data-ttu-id="dc627-115">无</span><span class="sxs-lookup"><span data-stu-id="dc627-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc627-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dc627-116">JSON Representation</span></span>
<span data-ttu-id="dc627-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dc627-117">Here is a JSON representation of the resource.</span></span>
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



