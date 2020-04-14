---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40d1631264f1aaaab5483cecd08222bb969c8a48
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447043"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="8f3fe-103">macOSLaunchItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f3fe-103">macOSLaunchItem resource type</span></span>

<span data-ttu-id="8f3fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f3fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f3fe-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8f3fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f3fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f3fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f3fe-107">表示 macOS 启动项列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="8f3fe-107">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="8f3fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f3fe-108">Properties</span></span>
|<span data-ttu-id="8f3fe-109">属性</span><span class="sxs-lookup"><span data-stu-id="8f3fe-109">Property</span></span>|<span data-ttu-id="8f3fe-110">类型</span><span class="sxs-lookup"><span data-stu-id="8f3fe-110">Type</span></span>|<span data-ttu-id="8f3fe-111">说明</span><span class="sxs-lookup"><span data-stu-id="8f3fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f3fe-112">路径</span><span class="sxs-lookup"><span data-stu-id="8f3fe-112">path</span></span>|<span data-ttu-id="8f3fe-113">String</span><span class="sxs-lookup"><span data-stu-id="8f3fe-113">String</span></span>|<span data-ttu-id="8f3fe-114">启动项目的路径。</span><span class="sxs-lookup"><span data-stu-id="8f3fe-114">Path to the launch item.</span></span>|
|<span data-ttu-id="8f3fe-115">选中</span><span class="sxs-lookup"><span data-stu-id="8f3fe-115">hide</span></span>|<span data-ttu-id="8f3fe-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8f3fe-116">Boolean</span></span>|<span data-ttu-id="8f3fe-117">是否要从 "用户和组" 列表中隐藏项目。</span><span class="sxs-lookup"><span data-stu-id="8f3fe-117">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f3fe-118">关系</span><span class="sxs-lookup"><span data-stu-id="8f3fe-118">Relationships</span></span>
<span data-ttu-id="8f3fe-119">无</span><span class="sxs-lookup"><span data-stu-id="8f3fe-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f3fe-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f3fe-120">JSON Representation</span></span>
<span data-ttu-id="8f3fe-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f3fe-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```



