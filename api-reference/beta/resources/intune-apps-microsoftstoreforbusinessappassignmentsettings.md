---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5f566a04169be20777b9f0fb5a7aa911ad3e864
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393247"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="c254e-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="c254e-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="c254e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c254e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c254e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c254e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c254e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c254e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c254e-107">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="c254e-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>


<span data-ttu-id="c254e-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="c254e-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c254e-109">属性</span><span class="sxs-lookup"><span data-stu-id="c254e-109">Properties</span></span>
|<span data-ttu-id="c254e-110">属性</span><span class="sxs-lookup"><span data-stu-id="c254e-110">Property</span></span>|<span data-ttu-id="c254e-111">类型</span><span class="sxs-lookup"><span data-stu-id="c254e-111">Type</span></span>|<span data-ttu-id="c254e-112">说明</span><span class="sxs-lookup"><span data-stu-id="c254e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c254e-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="c254e-113">useDeviceContext</span></span>|<span data-ttu-id="c254e-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="c254e-114">Boolean</span></span>|<span data-ttu-id="c254e-115">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="c254e-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c254e-116">关系</span><span class="sxs-lookup"><span data-stu-id="c254e-116">Relationships</span></span>
<span data-ttu-id="c254e-117">无</span><span class="sxs-lookup"><span data-stu-id="c254e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c254e-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c254e-118">JSON Representation</span></span>
<span data-ttu-id="c254e-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c254e-119">Here is a JSON representation of the resource.</span></span>
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




