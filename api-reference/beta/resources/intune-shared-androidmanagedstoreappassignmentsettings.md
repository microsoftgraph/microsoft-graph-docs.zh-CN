---
title: androidManagedStoreAppAssignmentSettings 资源类型
description: 包含用于将 Android 托管存储移动应用程序分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 383c272efc420cba893208e806a29df55f5429f6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073675"
---
# <a name="androidmanagedstoreappassignmentsettings-resource-type"></a><span data-ttu-id="d3f54-103">androidManagedStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3f54-103">androidManagedStoreAppAssignmentSettings resource type</span></span>

<span data-ttu-id="d3f54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3f54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3f54-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3f54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3f54-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3f54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3f54-107">包含用于将 Android 托管存储移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="d3f54-107">Contains properties used to assign an Android Managed Store mobile app to a group.</span></span>


<span data-ttu-id="d3f54-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="d3f54-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d3f54-109">属性</span><span class="sxs-lookup"><span data-stu-id="d3f54-109">Properties</span></span>
|<span data-ttu-id="d3f54-110">属性</span><span class="sxs-lookup"><span data-stu-id="d3f54-110">Property</span></span>|<span data-ttu-id="d3f54-111">类型</span><span class="sxs-lookup"><span data-stu-id="d3f54-111">Type</span></span>|<span data-ttu-id="d3f54-112">说明</span><span class="sxs-lookup"><span data-stu-id="d3f54-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3f54-113">androidManagedStoreAppTrackIds</span><span class="sxs-lookup"><span data-stu-id="d3f54-113">androidManagedStoreAppTrackIds</span></span>|<span data-ttu-id="d3f54-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="d3f54-114">String collection</span></span>|<span data-ttu-id="d3f54-115">要为此应用分配启用的跟踪 Id。</span><span class="sxs-lookup"><span data-stu-id="d3f54-115">The track IDs to enable for this app assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3f54-116">关系</span><span class="sxs-lookup"><span data-stu-id="d3f54-116">Relationships</span></span>
<span data-ttu-id="d3f54-117">无</span><span class="sxs-lookup"><span data-stu-id="d3f54-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3f54-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3f54-118">JSON Representation</span></span>
<span data-ttu-id="d3f54-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3f54-119">Here is a JSON representation of the resource.</span></span>
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






