---
title: windowsAppXAppAssignmentSettings 资源类型
description: 包含将 Windows AppX 移动应用程序分配给组时使用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83e384167984f1eda640ef1faa1f4241b1badbbb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167576"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="fa718-103">windowsAppXAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa718-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="fa718-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fa718-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa718-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fa718-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa718-106">包含将 Windows AppX 移动应用程序分配给组时使用的属性。</span><span class="sxs-lookup"><span data-stu-id="fa718-106">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>


<span data-ttu-id="fa718-107">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="fa718-107">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fa718-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa718-108">Properties</span></span>
|<span data-ttu-id="fa718-109">属性</span><span class="sxs-lookup"><span data-stu-id="fa718-109">Property</span></span>|<span data-ttu-id="fa718-110">类型</span><span class="sxs-lookup"><span data-stu-id="fa718-110">Type</span></span>|<span data-ttu-id="fa718-111">说明</span><span class="sxs-lookup"><span data-stu-id="fa718-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa718-112">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="fa718-112">useDeviceContext</span></span>|<span data-ttu-id="fa718-113">布尔值</span><span class="sxs-lookup"><span data-stu-id="fa718-113">Boolean</span></span>|<span data-ttu-id="fa718-114">是否对 Windows AppX 移动应用程序使用设备执行上下文。</span><span class="sxs-lookup"><span data-stu-id="fa718-114">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fa718-115">关系</span><span class="sxs-lookup"><span data-stu-id="fa718-115">Relationships</span></span>
<span data-ttu-id="fa718-116">无</span><span class="sxs-lookup"><span data-stu-id="fa718-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa718-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa718-117">JSON Representation</span></span>
<span data-ttu-id="fa718-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa718-118">Here is a JSON representation of the resource.</span></span>
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




