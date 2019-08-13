---
title: macOSLaunchItem 资源类型
description: 表示 macOS 启动项列表中的应用程序
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d1d9f2e2f17deeca2267bcc0397d4cfc7d650a7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321923"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="5766c-103">macOSLaunchItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5766c-103">macOSLaunchItem resource type</span></span>

> <span data-ttu-id="5766c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5766c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5766c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5766c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5766c-106">表示 macOS 启动项列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="5766c-106">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="5766c-107">属性</span><span class="sxs-lookup"><span data-stu-id="5766c-107">Properties</span></span>
|<span data-ttu-id="5766c-108">属性</span><span class="sxs-lookup"><span data-stu-id="5766c-108">Property</span></span>|<span data-ttu-id="5766c-109">类型</span><span class="sxs-lookup"><span data-stu-id="5766c-109">Type</span></span>|<span data-ttu-id="5766c-110">说明</span><span class="sxs-lookup"><span data-stu-id="5766c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5766c-111">路径</span><span class="sxs-lookup"><span data-stu-id="5766c-111">path</span></span>|<span data-ttu-id="5766c-112">String</span><span class="sxs-lookup"><span data-stu-id="5766c-112">String</span></span>|<span data-ttu-id="5766c-113">启动项目的路径。</span><span class="sxs-lookup"><span data-stu-id="5766c-113">Path to the launch item.</span></span>|
|<span data-ttu-id="5766c-114">选中</span><span class="sxs-lookup"><span data-stu-id="5766c-114">hide</span></span>|<span data-ttu-id="5766c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5766c-115">Boolean</span></span>|<span data-ttu-id="5766c-116">是否要从 "用户和组" 列表中隐藏项目。</span><span class="sxs-lookup"><span data-stu-id="5766c-116">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5766c-117">关系</span><span class="sxs-lookup"><span data-stu-id="5766c-117">Relationships</span></span>
<span data-ttu-id="5766c-118">无</span><span class="sxs-lookup"><span data-stu-id="5766c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5766c-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5766c-119">JSON Representation</span></span>
<span data-ttu-id="5766c-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5766c-120">Here is a JSON representation of the resource.</span></span>
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



