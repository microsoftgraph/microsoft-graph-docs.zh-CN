---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: tfitzmac
ms.openlocfilehash: 6c7fed2efda2b4c6d36eb53923b578535cce90e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354619"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="db67e-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="db67e-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="db67e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="db67e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db67e-105">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="db67e-105">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="db67e-106">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="db67e-106">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="db67e-107">属性</span><span class="sxs-lookup"><span data-stu-id="db67e-107">Properties</span></span>
|<span data-ttu-id="db67e-108">属性</span><span class="sxs-lookup"><span data-stu-id="db67e-108">Property</span></span>|<span data-ttu-id="db67e-109">类型</span><span class="sxs-lookup"><span data-stu-id="db67e-109">Type</span></span>|<span data-ttu-id="db67e-110">说明</span><span class="sxs-lookup"><span data-stu-id="db67e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db67e-111">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="db67e-111">useDeviceContext</span></span>|<span data-ttu-id="db67e-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="db67e-112">Boolean</span></span>|<span data-ttu-id="db67e-113">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="db67e-113">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db67e-114">关系</span><span class="sxs-lookup"><span data-stu-id="db67e-114">Relationships</span></span>
<span data-ttu-id="db67e-115">无</span><span class="sxs-lookup"><span data-stu-id="db67e-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="db67e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db67e-116">JSON Representation</span></span>
<span data-ttu-id="db67e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db67e-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



