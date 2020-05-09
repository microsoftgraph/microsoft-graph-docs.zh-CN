---
title: androidManagedStoreAppAssignmentSettings 资源类型
description: 包含用于将 Android 托管存储移动应用程序分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cfdca91e3499a495ba810b1c791653d62c769e4a
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178211"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="8ad55-103">androidManagedStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ad55-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="8ad55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ad55-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8ad55-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8ad55-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ad55-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ad55-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ad55-107">包含用于将 Android 托管存储移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="8ad55-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="8ad55-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8ad55-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8ad55-109">属性</span><span class="sxs-lookup"><span data-stu-id="8ad55-109">Properties</span></span>
|<span data-ttu-id="8ad55-110">属性</span><span class="sxs-lookup"><span data-stu-id="8ad55-110">Property</span></span>|<span data-ttu-id="8ad55-111">类型</span><span class="sxs-lookup"><span data-stu-id="8ad55-111">Type</span></span>|<span data-ttu-id="8ad55-112">说明</span><span class="sxs-lookup"><span data-stu-id="8ad55-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ad55-113">androidManagedStoreAppTrackIds</span><span class="sxs-lookup"><span data-stu-id="8ad55-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="8ad55-114">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8ad55-114">String collection</span></span>|<span data-ttu-id="8ad55-115">要为此应用分配启用的跟踪 Id。</span><span class="sxs-lookup"><span data-stu-id="8ad55-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ad55-116">关系</span><span class="sxs-lookup"><span data-stu-id="8ad55-116">Relationships</span></span>
<span data-ttu-id="8ad55-117">无</span><span class="sxs-lookup"><span data-stu-id="8ad55-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ad55-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ad55-118">JSON Representation</span></span>
<span data-ttu-id="8ad55-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ad55-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppAssignmentSettings",
  "androidManagedStoreAppTrackIds": [
    "String"
  ]
}
```



