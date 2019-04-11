---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用程序
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1317f2d42c21d0d11d45290696f183c679b049e1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809177"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="eeaea-103">macOSLaunchItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="eeaea-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="eeaea-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eeaea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eeaea-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eeaea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eeaea-106">表示 macOS 启动项列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="eeaea-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="eeaea-107">属性</span><span class="sxs-lookup"><span data-stu-id="eeaea-107">Properties</span></span>
|<span data-ttu-id="eeaea-108">属性</span><span class="sxs-lookup"><span data-stu-id="eeaea-108">Property</span></span>|<span data-ttu-id="eeaea-109">类型</span><span class="sxs-lookup"><span data-stu-id="eeaea-109">Type</span></span>|<span data-ttu-id="eeaea-110">说明</span><span class="sxs-lookup"><span data-stu-id="eeaea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeaea-111">路径</span><span class="sxs-lookup"><span data-stu-id="eeaea-111">path</span></span>|<span data-ttu-id="eeaea-112">String</span><span class="sxs-lookup"><span data-stu-id="eeaea-112">String</span></span>|<span data-ttu-id="eeaea-113">启动项目的路径。</span><span class="sxs-lookup"><span data-stu-id="eeaea-113">Path to the launch item.</span></span>|
|<span data-ttu-id="eeaea-114">选中</span><span class="sxs-lookup"><span data-stu-id="eeaea-114">hide</span></span>|<span data-ttu-id="eeaea-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="eeaea-115">Boolean</span></span>|<span data-ttu-id="eeaea-116">是否要从 "用户和组" 列表中隐藏项目。</span><span class="sxs-lookup"><span data-stu-id="eeaea-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eeaea-117">关系</span><span class="sxs-lookup"><span data-stu-id="eeaea-117">Relationships</span></span>
<span data-ttu-id="eeaea-118">无</span><span class="sxs-lookup"><span data-stu-id="eeaea-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eeaea-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eeaea-119">JSON Representation</span></span>
<span data-ttu-id="eeaea-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eeaea-120">Here is a JSON representation of the resource.</span></span>
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





