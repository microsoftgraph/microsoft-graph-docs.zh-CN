---
title: androidManagedStoreAppAssignmentSettings 资源类型
description: 包含用于将 Android 托管存储移动应用程序分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f07b1dc3535e624302b3d2ad2bfd047c286604b8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723783"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="0d798-103">androidManagedStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d798-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="0d798-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d798-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d798-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d798-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d798-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d798-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d798-107">包含用于将 Android 托管存储移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="0d798-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="0d798-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0d798-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d798-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d798-109">Properties</span></span>
|<span data-ttu-id="0d798-110">属性</span><span class="sxs-lookup"><span data-stu-id="0d798-110">Property</span></span>|<span data-ttu-id="0d798-111">类型</span><span class="sxs-lookup"><span data-stu-id="0d798-111">Type</span></span>|<span data-ttu-id="0d798-112">说明</span><span class="sxs-lookup"><span data-stu-id="0d798-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d798-113">androidManagedStoreAppTrackIds</span><span class="sxs-lookup"><span data-stu-id="0d798-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="0d798-114">String collection</span><span class="sxs-lookup"><span data-stu-id="0d798-114">String collection</span></span>|<span data-ttu-id="0d798-115">要为此应用分配启用的跟踪 Id。</span><span class="sxs-lookup"><span data-stu-id="0d798-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d798-116">关系</span><span class="sxs-lookup"><span data-stu-id="0d798-116">Relationships</span></span>
<span data-ttu-id="0d798-117">无</span><span class="sxs-lookup"><span data-stu-id="0d798-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d798-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d798-118">JSON Representation</span></span>
<span data-ttu-id="0d798-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d798-119">Here is a JSON representation of the resource.</span></span>
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





