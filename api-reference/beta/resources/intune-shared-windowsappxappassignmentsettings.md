---
title: windowsAppXAppAssignmentSettings 资源类型
description: 包含将 Windows AppX 移动应用程序分配给组时使用的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f0732a9399f711d3db8b9e95b57182877879fc8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42766852"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="b9cea-103">windowsAppXAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9cea-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="b9cea-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9cea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9cea-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9cea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9cea-106">包含将 Windows AppX 移动应用程序分配给组时使用的属性。</span><span class="sxs-lookup"><span data-stu-id="b9cea-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="b9cea-107">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="b9cea-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9cea-108">属性</span><span class="sxs-lookup"><span data-stu-id="b9cea-108">Properties</span></span>
|<span data-ttu-id="b9cea-109">属性</span><span class="sxs-lookup"><span data-stu-id="b9cea-109">Property</span></span>|<span data-ttu-id="b9cea-110">类型</span><span class="sxs-lookup"><span data-stu-id="b9cea-110">Type</span></span>|<span data-ttu-id="b9cea-111">说明</span><span class="sxs-lookup"><span data-stu-id="b9cea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9cea-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="b9cea-112">useDeviceContext</span></span>|<span data-ttu-id="b9cea-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="b9cea-113">Boolean</span></span>|<span data-ttu-id="b9cea-114">是否对 Windows AppX 移动应用程序使用设备执行上下文。</span><span class="sxs-lookup"><span data-stu-id="b9cea-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9cea-115">关系</span><span class="sxs-lookup"><span data-stu-id="b9cea-115">Relationships</span></span>
<span data-ttu-id="b9cea-116">无</span><span class="sxs-lookup"><span data-stu-id="b9cea-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9cea-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9cea-117">JSON Representation</span></span>
<span data-ttu-id="b9cea-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9cea-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```



