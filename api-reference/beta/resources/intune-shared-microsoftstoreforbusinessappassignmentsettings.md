---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb2dc1fda4fdc903bd64d053ce377f4f5f203aa7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523630"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="54443-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="54443-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

<span data-ttu-id="54443-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="54443-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="54443-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="54443-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54443-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="54443-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54443-107">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="54443-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="54443-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="54443-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="54443-109">属性</span><span class="sxs-lookup"><span data-stu-id="54443-109">Properties</span></span>
|<span data-ttu-id="54443-110">属性</span><span class="sxs-lookup"><span data-stu-id="54443-110">Property</span></span>|<span data-ttu-id="54443-111">类型</span><span class="sxs-lookup"><span data-stu-id="54443-111">Type</span></span>|<span data-ttu-id="54443-112">说明</span><span class="sxs-lookup"><span data-stu-id="54443-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54443-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="54443-113">useDeviceContext</span></span>|<span data-ttu-id="54443-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="54443-114">Boolean</span></span>|<span data-ttu-id="54443-115">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="54443-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54443-116">关系</span><span class="sxs-lookup"><span data-stu-id="54443-116">Relationships</span></span>
<span data-ttu-id="54443-117">无</span><span class="sxs-lookup"><span data-stu-id="54443-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="54443-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54443-118">JSON Representation</span></span>
<span data-ttu-id="54443-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54443-119">Here is a JSON representation of the resource.</span></span>
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



