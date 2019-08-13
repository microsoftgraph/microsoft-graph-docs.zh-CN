---
title: windowsUniversalAppXAppAssignmentSettings 资源类型
description: 包含将 Windows 通用 AppX 移动应用程序分配给组时使用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9b93a6a7b5a0b23bf4b47531e3c810c20de0eefc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335289"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="e2ec9-103">windowsUniversalAppXAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e2ec9-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="e2ec9-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e2ec9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2ec9-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e2ec9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2ec9-106">包含将 Windows 通用 AppX 移动应用程序分配给组时使用的属性。</span><span class="sxs-lookup"><span data-stu-id="e2ec9-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="e2ec9-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="e2ec9-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2ec9-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2ec9-108">Properties</span></span>
|<span data-ttu-id="e2ec9-109">属性</span><span class="sxs-lookup"><span data-stu-id="e2ec9-109">Property</span></span>|<span data-ttu-id="e2ec9-110">类型</span><span class="sxs-lookup"><span data-stu-id="e2ec9-110">Type</span></span>|<span data-ttu-id="e2ec9-111">说明</span><span class="sxs-lookup"><span data-stu-id="e2ec9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2ec9-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="e2ec9-112">useDeviceContext</span></span>|<span data-ttu-id="e2ec9-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="e2ec9-113">Boolean</span></span>|<span data-ttu-id="e2ec9-114">是否对 Windows 通用 AppX 移动应用程序使用设备执行上下文。</span><span class="sxs-lookup"><span data-stu-id="e2ec9-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2ec9-115">关系</span><span class="sxs-lookup"><span data-stu-id="e2ec9-115">Relationships</span></span>
<span data-ttu-id="e2ec9-116">无</span><span class="sxs-lookup"><span data-stu-id="e2ec9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e2ec9-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e2ec9-117">JSON Representation</span></span>
<span data-ttu-id="e2ec9-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e2ec9-118">Here is a JSON representation of the resource.</span></span>
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



