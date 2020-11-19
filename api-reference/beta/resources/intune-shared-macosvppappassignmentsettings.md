---
title: macOsVppAppAssignmentSettings 资源类型
description: 包含用于将 Mac VPP 移动应用程序分配给组的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fbd6d9193bc9a441caf66662dab42bcb7648d374
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258946"
---
# <a name="macosvppappassignmentsettings-resource-type"></a><span data-ttu-id="96ba9-103">macOsVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="96ba9-103">macOsVppAppAssignmentSettings resource type</span></span>

<span data-ttu-id="96ba9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96ba9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96ba9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96ba9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96ba9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96ba9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96ba9-107">包含用于将 Mac VPP 移动应用程序分配给组的属性。</span><span class="sxs-lookup"><span data-stu-id="96ba9-107">Contains properties used to assign an Mac VPP mobile app to a group.</span></span>


<span data-ttu-id="96ba9-108">继承自 [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="96ba9-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-shared-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="96ba9-109">属性</span><span class="sxs-lookup"><span data-stu-id="96ba9-109">Properties</span></span>
|<span data-ttu-id="96ba9-110">属性</span><span class="sxs-lookup"><span data-stu-id="96ba9-110">Property</span></span>|<span data-ttu-id="96ba9-111">类型</span><span class="sxs-lookup"><span data-stu-id="96ba9-111">Type</span></span>|<span data-ttu-id="96ba9-112">描述</span><span class="sxs-lookup"><span data-stu-id="96ba9-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ba9-113">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="96ba9-113">useDeviceLicensing</span></span>|<span data-ttu-id="96ba9-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="96ba9-114">Boolean</span></span>|<span data-ttu-id="96ba9-115">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="96ba9-115">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="96ba9-116">uninstallOnDeviceRemoval</span><span class="sxs-lookup"><span data-stu-id="96ba9-116">uninstallOnDeviceRemoval</span></span>|<span data-ttu-id="96ba9-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="96ba9-117">Boolean</span></span>|<span data-ttu-id="96ba9-118">从 Intune 中删除设备时是否卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="96ba9-118">Whether or not to uninstall the app when device is removed from Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96ba9-119">关系</span><span class="sxs-lookup"><span data-stu-id="96ba9-119">Relationships</span></span>
<span data-ttu-id="96ba9-120">无</span><span class="sxs-lookup"><span data-stu-id="96ba9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96ba9-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96ba9-121">JSON Representation</span></span>
<span data-ttu-id="96ba9-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96ba9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOsVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "uninstallOnDeviceRemoval": true
}
```




