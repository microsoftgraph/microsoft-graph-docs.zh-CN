---
title: windowsAppXAppAssignmentSettings 资源类型
description: 包含分配给组的 Windows 约移动应用程序时使用的属性。
author: tfitzmac
ms.openlocfilehash: 84103a91c3c670ef3da8a0ea2a2e38a95cff79a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311618"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a><span data-ttu-id="24c46-103">windowsAppXAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="24c46-103">windowsAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="24c46-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="24c46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="24c46-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="24c46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24c46-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="24c46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24c46-107">包含分配给组的 Windows 约移动应用程序时使用的属性。</span><span class="sxs-lookup"><span data-stu-id="24c46-107">Contains properties used when assigning a Windows AppX mobile app to a group.</span></span>

<span data-ttu-id="24c46-108">继承自 [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="24c46-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24c46-109">属性</span><span class="sxs-lookup"><span data-stu-id="24c46-109">Properties</span></span>
|<span data-ttu-id="24c46-110">属性</span><span class="sxs-lookup"><span data-stu-id="24c46-110">Property</span></span>|<span data-ttu-id="24c46-111">类型</span><span class="sxs-lookup"><span data-stu-id="24c46-111">Type</span></span>|<span data-ttu-id="24c46-112">说明</span><span class="sxs-lookup"><span data-stu-id="24c46-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24c46-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="24c46-113">useDeviceContext</span></span>|<span data-ttu-id="24c46-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="24c46-114">Boolean</span></span>|<span data-ttu-id="24c46-115">是否使用 Windows 约移动应用程序的设备执行上下文。</span><span class="sxs-lookup"><span data-stu-id="24c46-115">Whether or not to use device execution context for Windows AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24c46-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="24c46-116">Relationships</span></span>
<span data-ttu-id="24c46-117">无</span><span class="sxs-lookup"><span data-stu-id="24c46-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="24c46-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24c46-118">JSON Representation</span></span>
<span data-ttu-id="24c46-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24c46-119">Here is a JSON representation of the resource.</span></span>
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





