---
title: windowsAppXAppAssignmentSettings 资源类型
description: 包含分配给组的 Windows 约移动应用程序时使用的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f55400b0e17884a4e6ca3de0692e69d388c46e2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410922"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="66d21-103">windowsAppXAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="66d21-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="66d21-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="66d21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="66d21-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="66d21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="66d21-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66d21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d21-107">包含分配给组的 Windows 约移动应用程序时使用的属性。</span><span class="sxs-lookup"><span data-stu-id="66d21-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="66d21-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="66d21-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="66d21-109">属性</span><span class="sxs-lookup"><span data-stu-id="66d21-109">Properties</span></span>
|<span data-ttu-id="66d21-110">属性</span><span class="sxs-lookup"><span data-stu-id="66d21-110">Property</span></span>|<span data-ttu-id="66d21-111">类型</span><span class="sxs-lookup"><span data-stu-id="66d21-111">Type</span></span>|<span data-ttu-id="66d21-112">说明</span><span class="sxs-lookup"><span data-stu-id="66d21-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d21-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="66d21-113">useDeviceContext</span></span>|<span data-ttu-id="66d21-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="66d21-114">Boolean</span></span>|<span data-ttu-id="66d21-115">是否使用 Windows 约移动应用程序的设备执行上下文。</span><span class="sxs-lookup"><span data-stu-id="66d21-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66d21-116">关系</span><span class="sxs-lookup"><span data-stu-id="66d21-116">Relationships</span></span>
<span data-ttu-id="66d21-117">无</span><span class="sxs-lookup"><span data-stu-id="66d21-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66d21-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66d21-118">JSON Representation</span></span>
<span data-ttu-id="66d21-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66d21-119">Here is a JSON representation of the resource.</span></span>
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




