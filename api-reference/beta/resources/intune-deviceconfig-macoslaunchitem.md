---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用程序
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2752abd8d76c08e1da162d58aa8863d2f8b63940
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992120"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="2c1cf-103">macOSLaunchItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c1cf-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="2c1cf-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2c1cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c1cf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c1cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c1cf-106">表示 macOS 启动项列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="2c1cf-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="2c1cf-107">属性</span><span class="sxs-lookup"><span data-stu-id="2c1cf-107">Properties</span></span>
|<span data-ttu-id="2c1cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="2c1cf-108">Property</span></span>|<span data-ttu-id="2c1cf-109">类型</span><span class="sxs-lookup"><span data-stu-id="2c1cf-109">Type</span></span>|<span data-ttu-id="2c1cf-110">说明</span><span class="sxs-lookup"><span data-stu-id="2c1cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c1cf-111">路径</span><span class="sxs-lookup"><span data-stu-id="2c1cf-111">path</span></span>|<span data-ttu-id="2c1cf-112">String</span><span class="sxs-lookup"><span data-stu-id="2c1cf-112">String</span></span>|<span data-ttu-id="2c1cf-113">启动项目的路径。</span><span class="sxs-lookup"><span data-stu-id="2c1cf-113">Path to the launch item.</span></span>|
|<span data-ttu-id="2c1cf-114">选中</span><span class="sxs-lookup"><span data-stu-id="2c1cf-114">hide</span></span>|<span data-ttu-id="2c1cf-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c1cf-115">Boolean</span></span>|<span data-ttu-id="2c1cf-116">是否要从 "用户和组" 列表中隐藏项目。</span><span class="sxs-lookup"><span data-stu-id="2c1cf-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c1cf-117">关系</span><span class="sxs-lookup"><span data-stu-id="2c1cf-117">Relationships</span></span>
<span data-ttu-id="2c1cf-118">无</span><span class="sxs-lookup"><span data-stu-id="2c1cf-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c1cf-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c1cf-119">JSON Representation</span></span>
<span data-ttu-id="2c1cf-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c1cf-120">Here is a JSON representation of the resource.</span></span>
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





