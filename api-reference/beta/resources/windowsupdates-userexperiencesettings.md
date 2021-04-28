---
title: userExperienceSettings 资源类型
description: 设置控制用户对设备的更新体验。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a5d920d1618cb6d212baf0487a39960638859cef
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067257"
---
# <a name="userexperiencesettings-resource-type"></a><span data-ttu-id="a8af4-103">userExperienceSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8af4-103">userExperienceSettings resource type</span></span>

<span data-ttu-id="a8af4-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="a8af4-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8af4-105">设置控制用户对设备的更新体验。</span><span class="sxs-lookup"><span data-stu-id="a8af4-105">Settings controlling the user's update experience on a device.</span></span>

## <a name="properties"></a><span data-ttu-id="a8af4-106">属性</span><span class="sxs-lookup"><span data-stu-id="a8af4-106">Properties</span></span>
|<span data-ttu-id="a8af4-107">属性</span><span class="sxs-lookup"><span data-stu-id="a8af4-107">Property</span></span>|<span data-ttu-id="a8af4-108">类型</span><span class="sxs-lookup"><span data-stu-id="a8af4-108">Type</span></span>|<span data-ttu-id="a8af4-109">说明</span><span class="sxs-lookup"><span data-stu-id="a8af4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8af4-110">daysUntilForcedReboot</span><span class="sxs-lookup"><span data-stu-id="a8af4-110">daysUntilForcedReboot</span></span>|<span data-ttu-id="a8af4-111">Int32</span><span class="sxs-lookup"><span data-stu-id="a8af4-111">Int32</span></span>|<span data-ttu-id="a8af4-112">指定安装更新后的天数，在此期间设备用户可以控制设备重启的时间。</span><span class="sxs-lookup"><span data-stu-id="a8af4-112">Specifies the number of days after an update is installed, during which the user of the device can control when the device restarts.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8af4-113">关系</span><span class="sxs-lookup"><span data-stu-id="a8af4-113">Relationships</span></span>
<span data-ttu-id="a8af4-114">无。</span><span class="sxs-lookup"><span data-stu-id="a8af4-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8af4-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8af4-115">JSON representation</span></span>
<span data-ttu-id="a8af4-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8af4-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.userExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.userExperienceSettings",
  "daysUntilForcedReboot": "Integer"
}
```

