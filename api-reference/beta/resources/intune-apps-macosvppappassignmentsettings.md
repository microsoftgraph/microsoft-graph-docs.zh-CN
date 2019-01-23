---
title: macOsVppAppAssignmentSettings 资源类型
description: 包含用于 Mac VPP 移动应用程序分配给组的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0927277b11416da001ad826200bf4ec841341118
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431402"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="581ea-103">macOsVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="581ea-103">macOsVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="581ea-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="581ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="581ea-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="581ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="581ea-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="581ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="581ea-107">包含用于 Mac VPP 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="581ea-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="581ea-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="581ea-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="581ea-109">属性</span><span class="sxs-lookup"><span data-stu-id="581ea-109">Properties</span></span>
|<span data-ttu-id="581ea-110">属性</span><span class="sxs-lookup"><span data-stu-id="581ea-110">Property</span></span>|<span data-ttu-id="581ea-111">类型</span><span class="sxs-lookup"><span data-stu-id="581ea-111">Type</span></span>|<span data-ttu-id="581ea-112">说明</span><span class="sxs-lookup"><span data-stu-id="581ea-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581ea-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="581ea-113">useDeviceLicensing</span></span>|<span data-ttu-id="581ea-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="581ea-114">Boolean</span></span>|<span data-ttu-id="581ea-115">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="581ea-115">Whether or not to use device licensing.</span></span>|

## <a name="relationships"></a><span data-ttu-id="581ea-116">关系</span><span class="sxs-lookup"><span data-stu-id="581ea-116">Relationships</span></span>
<span data-ttu-id="581ea-117">无</span><span class="sxs-lookup"><span data-stu-id="581ea-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="581ea-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="581ea-118">JSON Representation</span></span>
<span data-ttu-id="581ea-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="581ea-119">Here is a JSON representation of the resource.</span></span>
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




