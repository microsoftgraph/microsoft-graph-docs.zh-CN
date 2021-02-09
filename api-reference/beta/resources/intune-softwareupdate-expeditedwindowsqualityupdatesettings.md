---
title: expeditedWindowsQualityUpdateSettings 资源类型
description: 用于存储快速质量更新设置（如发布日期和天，直到强制重启）的复杂类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 700b86d15737c75cbf10679ea6e944726d667431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160197"
---
# <a name="expeditedwindowsqualityupdatesettings-resource-type"></a><span data-ttu-id="85f78-103">expeditedWindowsQualityUpdateSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="85f78-103">expeditedWindowsQualityUpdateSettings resource type</span></span>

<span data-ttu-id="85f78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85f78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="85f78-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="85f78-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="85f78-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="85f78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="85f78-107">用于存储快速质量更新设置（如发布日期和天，直到强制重启）的复杂类型。</span><span class="sxs-lookup"><span data-stu-id="85f78-107">A complex type to store the expedited quality update settings such as release date and days until forced reboot.</span></span>

## <a name="properties"></a><span data-ttu-id="85f78-108">属性</span><span class="sxs-lookup"><span data-stu-id="85f78-108">Properties</span></span>
|<span data-ttu-id="85f78-109">属性</span><span class="sxs-lookup"><span data-stu-id="85f78-109">Property</span></span>|<span data-ttu-id="85f78-110">类型</span><span class="sxs-lookup"><span data-stu-id="85f78-110">Type</span></span>|<span data-ttu-id="85f78-111">说明</span><span class="sxs-lookup"><span data-stu-id="85f78-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85f78-112">qualityUpdateRelease</span><span class="sxs-lookup"><span data-stu-id="85f78-112">qualityUpdateRelease</span></span>|<span data-ttu-id="85f78-113">String</span><span class="sxs-lookup"><span data-stu-id="85f78-113">String</span></span>|<span data-ttu-id="85f78-114">用于标识质量更新的发布日期。</span><span class="sxs-lookup"><span data-stu-id="85f78-114">The release date to identify a quality update.</span></span>|
|<span data-ttu-id="85f78-115">daysUntilForcedReboot</span><span class="sxs-lookup"><span data-stu-id="85f78-115">daysUntilForcedReboot</span></span>|<span data-ttu-id="85f78-116">Int32</span><span class="sxs-lookup"><span data-stu-id="85f78-116">Int32</span></span>|<span data-ttu-id="85f78-117">安装后将发生强制重启的天数。</span><span class="sxs-lookup"><span data-stu-id="85f78-117">The number of days after installation that forced reboot will happen.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85f78-118">关系</span><span class="sxs-lookup"><span data-stu-id="85f78-118">Relationships</span></span>
<span data-ttu-id="85f78-119">无</span><span class="sxs-lookup"><span data-stu-id="85f78-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85f78-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85f78-120">JSON Representation</span></span>
<span data-ttu-id="85f78-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85f78-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.expeditedWindowsQualityUpdateSettings",
  "qualityUpdateRelease": "String",
  "daysUntilForcedReboot": 1024
}
```




