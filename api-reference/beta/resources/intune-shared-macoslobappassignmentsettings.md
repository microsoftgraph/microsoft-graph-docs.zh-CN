---
title: macOsLobAppAssignmentSettings 资源类型
description: 包含用于将 Mac LOB 应用分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3e00019e2ed7609aa02fc3f16b2076027617fcab
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160544"
---
# <a name="macoslobappassignmentsettings-resource-type"></a><span data-ttu-id="392f4-103">macOsLobAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="392f4-103">macOsLobAppAssignmentSettings resource type</span></span>

<span data-ttu-id="392f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="392f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="392f4-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="392f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="392f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="392f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="392f4-107">包含用于将 Mac LOB 应用分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="392f4-107">Contains properties used to assign an Mac LOB  app to a group.</span></span>


<span data-ttu-id="392f4-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="392f4-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="392f4-109">属性</span><span class="sxs-lookup"><span data-stu-id="392f4-109">Properties</span></span>
|<span data-ttu-id="392f4-110">属性</span><span class="sxs-lookup"><span data-stu-id="392f4-110">Property</span></span>|<span data-ttu-id="392f4-111">类型</span><span class="sxs-lookup"><span data-stu-id="392f4-111">Type</span></span>|<span data-ttu-id="392f4-112">说明</span><span class="sxs-lookup"><span data-stu-id="392f4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="392f4-113">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="392f4-113">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="392f4-114">布尔</span><span class="sxs-lookup"><span data-stu-id="392f4-114">Boolean</span></span>|<span data-ttu-id="392f4-115">从 Intune 中删除设备时是否卸载应用。</span><span class="sxs-lookup"><span data-stu-id="392f4-115">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="392f4-116">关系</span><span class="sxs-lookup"><span data-stu-id="392f4-116">Relationships</span></span>
<span data-ttu-id="392f4-117">无</span><span class="sxs-lookup"><span data-stu-id="392f4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="392f4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="392f4-118">JSON Representation</span></span>
<span data-ttu-id="392f4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="392f4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsLobAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsLobAppAssignmentSettings",
  "uninstallOnDeviceRemoval": true
}
```




