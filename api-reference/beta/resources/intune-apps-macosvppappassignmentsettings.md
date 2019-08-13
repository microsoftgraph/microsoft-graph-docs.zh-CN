---
title: macOsVppAppAssignmentSettings 资源类型
description: 包含用于将 Mac VPP 移动应用程序分配给组的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3892ad8e00d95be00101ba4bc11c38e61e3a59c6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366719"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="080fe-103">macOsVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="080fe-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="080fe-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="080fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="080fe-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="080fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="080fe-106">包含用于将 Mac VPP 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="080fe-106">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="080fe-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="080fe-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="080fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="080fe-108">Properties</span></span>
|<span data-ttu-id="080fe-109">属性</span><span class="sxs-lookup"><span data-stu-id="080fe-109">Property</span></span>|<span data-ttu-id="080fe-110">类型</span><span class="sxs-lookup"><span data-stu-id="080fe-110">Type</span></span>|<span data-ttu-id="080fe-111">说明</span><span class="sxs-lookup"><span data-stu-id="080fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="080fe-112">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="080fe-112">useDeviceLicensing</span></span>|<span data-ttu-id="080fe-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="080fe-113">Boolean</span></span>|<span data-ttu-id="080fe-114">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="080fe-114">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="080fe-115">关系</span><span class="sxs-lookup"><span data-stu-id="080fe-115">Relationships</span></span>
<span data-ttu-id="080fe-116">无</span><span class="sxs-lookup"><span data-stu-id="080fe-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="080fe-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="080fe-117">JSON Representation</span></span>
<span data-ttu-id="080fe-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="080fe-118">Here is a JSON representation of the resource.</span></span>
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



