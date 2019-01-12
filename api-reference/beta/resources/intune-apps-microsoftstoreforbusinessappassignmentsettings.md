---
title: microsoftStoreForBusinessAppAssignmentSettings 资源类型
description: 包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4cbb3a12482c1a740e1d7e0f98b4f38d424500d4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952249"
---
# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="8c7d1-103">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c7d1-103">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="8c7d1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8c7d1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c7d1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8c7d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c7d1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8c7d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c7d1-107">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="8c7d1-107">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="8c7d1-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="8c7d1-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8c7d1-109">属性</span><span class="sxs-lookup"><span data-stu-id="8c7d1-109">Properties</span></span>
|<span data-ttu-id="8c7d1-110">属性</span><span class="sxs-lookup"><span data-stu-id="8c7d1-110">Property</span></span>|<span data-ttu-id="8c7d1-111">类型</span><span class="sxs-lookup"><span data-stu-id="8c7d1-111">Type</span></span>|<span data-ttu-id="8c7d1-112">说明</span><span class="sxs-lookup"><span data-stu-id="8c7d1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c7d1-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="8c7d1-113">useDeviceContext</span></span>|<span data-ttu-id="8c7d1-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="8c7d1-114">Boolean</span></span>|<span data-ttu-id="8c7d1-115">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="8c7d1-115">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c7d1-116">关系</span><span class="sxs-lookup"><span data-stu-id="8c7d1-116">Relationships</span></span>
<span data-ttu-id="8c7d1-117">无</span><span class="sxs-lookup"><span data-stu-id="8c7d1-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c7d1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c7d1-118">JSON Representation</span></span>
<span data-ttu-id="8c7d1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c7d1-119">Here is a JSON representation of the resource.</span></span>
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





