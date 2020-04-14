---
title: macOsVppAppAssignmentSettings 资源类型
description: 包含用于将 Mac VPP 移动应用程序分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ddd69a94880c97ad389150eb66a429496d36335
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466255"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="e9ae0-103">macOsVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e9ae0-103">macOsVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="e9ae0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9ae0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9ae0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9ae0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9ae0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9ae0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9ae0-107">包含用于将 Mac VPP 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="e9ae0-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="e9ae0-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e9ae0-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9ae0-109">属性</span><span class="sxs-lookup"><span data-stu-id="e9ae0-109">Properties</span></span>
|<span data-ttu-id="e9ae0-110">属性</span><span class="sxs-lookup"><span data-stu-id="e9ae0-110">Property</span></span>|<span data-ttu-id="e9ae0-111">类型</span><span class="sxs-lookup"><span data-stu-id="e9ae0-111">Type</span></span>|<span data-ttu-id="e9ae0-112">说明</span><span class="sxs-lookup"><span data-stu-id="e9ae0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9ae0-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="e9ae0-113">useDeviceLicensing</span></span>|<span data-ttu-id="e9ae0-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="e9ae0-114">Boolean</span></span>|<span data-ttu-id="e9ae0-115">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="e9ae0-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9ae0-116">关系</span><span class="sxs-lookup"><span data-stu-id="e9ae0-116">Relationships</span></span>
<span data-ttu-id="e9ae0-117">无</span><span class="sxs-lookup"><span data-stu-id="e9ae0-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9ae0-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e9ae0-118">JSON Representation</span></span>
<span data-ttu-id="e9ae0-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9ae0-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true
}
```



