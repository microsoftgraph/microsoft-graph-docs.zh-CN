---
title: windowsUniversalAppXAppAssignmentSettings 资源类型
description: 包含分配给组的 Windows 通用约移动应用程序时使用的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27755a483be44584aeb82166f56e825df79f8eaa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400716"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="16aef-103">windowsUniversalAppXAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="16aef-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="16aef-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="16aef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16aef-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="16aef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16aef-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16aef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16aef-107">包含分配给组的 Windows 通用约移动应用程序时使用的属性。</span><span class="sxs-lookup"><span data-stu-id="16aef-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="16aef-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="16aef-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16aef-109">属性</span><span class="sxs-lookup"><span data-stu-id="16aef-109">Properties</span></span>
|<span data-ttu-id="16aef-110">属性</span><span class="sxs-lookup"><span data-stu-id="16aef-110">Property</span></span>|<span data-ttu-id="16aef-111">类型</span><span class="sxs-lookup"><span data-stu-id="16aef-111">Type</span></span>|<span data-ttu-id="16aef-112">说明</span><span class="sxs-lookup"><span data-stu-id="16aef-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16aef-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="16aef-113">useDeviceContext</span></span>|<span data-ttu-id="16aef-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="16aef-114">Boolean</span></span>|<span data-ttu-id="16aef-115">是否对 Windows 通用约移动应用程序使用设备执行上下文。</span><span class="sxs-lookup"><span data-stu-id="16aef-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16aef-116">关系</span><span class="sxs-lookup"><span data-stu-id="16aef-116">Relationships</span></span>
<span data-ttu-id="16aef-117">无</span><span class="sxs-lookup"><span data-stu-id="16aef-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16aef-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16aef-118">JSON Representation</span></span>
<span data-ttu-id="16aef-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16aef-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```




