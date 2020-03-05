---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用程序
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbdec2156c135544a6ce36887fcd7c911217dff5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529681"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="860cc-103">macOSLaunchItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="860cc-103">macOSLaunchItem resource type</span></span>

<span data-ttu-id="860cc-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="860cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="860cc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="860cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="860cc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="860cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="860cc-107">表示 macOS 启动项列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="860cc-107">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="860cc-108">属性</span><span class="sxs-lookup"><span data-stu-id="860cc-108">Properties</span></span>
|<span data-ttu-id="860cc-109">属性</span><span class="sxs-lookup"><span data-stu-id="860cc-109">Property</span></span>|<span data-ttu-id="860cc-110">类型</span><span class="sxs-lookup"><span data-stu-id="860cc-110">Type</span></span>|<span data-ttu-id="860cc-111">说明</span><span class="sxs-lookup"><span data-stu-id="860cc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="860cc-112">路径</span><span class="sxs-lookup"><span data-stu-id="860cc-112">path</span></span>|<span data-ttu-id="860cc-113">String</span><span class="sxs-lookup"><span data-stu-id="860cc-113">String</span></span>|<span data-ttu-id="860cc-114">启动项目的路径。</span><span class="sxs-lookup"><span data-stu-id="860cc-114">Path to the launch item.</span></span>|
|<span data-ttu-id="860cc-115">选中</span><span class="sxs-lookup"><span data-stu-id="860cc-115">hide</span></span>|<span data-ttu-id="860cc-116">布尔</span><span class="sxs-lookup"><span data-stu-id="860cc-116">Boolean</span></span>|<span data-ttu-id="860cc-117">是否要从 "用户和组" 列表中隐藏项目。</span><span class="sxs-lookup"><span data-stu-id="860cc-117">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="860cc-118">关系</span><span class="sxs-lookup"><span data-stu-id="860cc-118">Relationships</span></span>
<span data-ttu-id="860cc-119">无</span><span class="sxs-lookup"><span data-stu-id="860cc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="860cc-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="860cc-120">JSON Representation</span></span>
<span data-ttu-id="860cc-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="860cc-121">Here is a JSON representation of the resource.</span></span>
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



