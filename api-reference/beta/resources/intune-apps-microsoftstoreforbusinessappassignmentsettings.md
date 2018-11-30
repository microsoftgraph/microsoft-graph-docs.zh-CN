---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
ms.openlocfilehash: 53dc4e9887147253047df67db865c45488b51009
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043506"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="efd72-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="efd72-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="efd72-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="efd72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="efd72-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="efd72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="efd72-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="efd72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="efd72-107">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="efd72-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="efd72-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="efd72-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="efd72-109">属性</span><span class="sxs-lookup"><span data-stu-id="efd72-109">Properties</span></span>
|<span data-ttu-id="efd72-110">属性</span><span class="sxs-lookup"><span data-stu-id="efd72-110">Property</span></span>|<span data-ttu-id="efd72-111">类型</span><span class="sxs-lookup"><span data-stu-id="efd72-111">Type</span></span>|<span data-ttu-id="efd72-112">说明</span><span class="sxs-lookup"><span data-stu-id="efd72-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efd72-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="efd72-113">useDeviceContext</span></span>|<span data-ttu-id="efd72-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="efd72-114">Boolean</span></span>|<span data-ttu-id="efd72-115">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="efd72-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efd72-116">关系</span><span class="sxs-lookup"><span data-stu-id="efd72-116">Relationships</span></span>
<span data-ttu-id="efd72-117">无</span><span class="sxs-lookup"><span data-stu-id="efd72-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="efd72-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efd72-118">JSON Representation</span></span>
<span data-ttu-id="efd72-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efd72-119">Here is a JSON representation of the resource.</span></span>
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





