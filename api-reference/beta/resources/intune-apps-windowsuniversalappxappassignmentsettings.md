---
title: windowsUniversalAppXAppAssignmentSettings 资源类型
description: 包含将 Windows 通用 AppX 移动应用程序分配给组时使用的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f04f8207eab8bea01fd164eb1fdd7b34baf605a7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34985645"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="6ea34-103">windowsUniversalAppXAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ea34-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="6ea34-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ea34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ea34-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ea34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ea34-106">包含将 Windows 通用 AppX 移动应用程序分配给组时使用的属性。</span><span class="sxs-lookup"><span data-stu-id="6ea34-106">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>


<span data-ttu-id="6ea34-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="6ea34-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ea34-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ea34-108">Properties</span></span>
|<span data-ttu-id="6ea34-109">属性</span><span class="sxs-lookup"><span data-stu-id="6ea34-109">Property</span></span>|<span data-ttu-id="6ea34-110">类型</span><span class="sxs-lookup"><span data-stu-id="6ea34-110">Type</span></span>|<span data-ttu-id="6ea34-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ea34-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ea34-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="6ea34-112">useDeviceContext</span></span>|<span data-ttu-id="6ea34-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="6ea34-113">Boolean</span></span>|<span data-ttu-id="6ea34-114">是否对 Windows 通用 AppX 移动应用程序使用设备执行上下文。</span><span class="sxs-lookup"><span data-stu-id="6ea34-114">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ea34-115">关系</span><span class="sxs-lookup"><span data-stu-id="6ea34-115">Relationships</span></span>
<span data-ttu-id="6ea34-116">无</span><span class="sxs-lookup"><span data-stu-id="6ea34-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ea34-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ea34-117">JSON Representation</span></span>
<span data-ttu-id="6ea34-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ea34-118">Here is a JSON representation of the resource.</span></span>
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





