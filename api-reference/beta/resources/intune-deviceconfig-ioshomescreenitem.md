---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c84c61128e9f8f81cf21c2908c4615f0fc7134e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526351"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="b23e5-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b23e5-103">iosHomeScreenItem resource type</span></span>

<span data-ttu-id="b23e5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b23e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b23e5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b23e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b23e5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b23e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b23e5-107">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="b23e5-107">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="b23e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="b23e5-108">Properties</span></span>
|<span data-ttu-id="b23e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="b23e5-109">Property</span></span>|<span data-ttu-id="b23e5-110">类型</span><span class="sxs-lookup"><span data-stu-id="b23e5-110">Type</span></span>|<span data-ttu-id="b23e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="b23e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b23e5-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b23e5-112">displayName</span></span>|<span data-ttu-id="b23e5-113">String</span><span class="sxs-lookup"><span data-stu-id="b23e5-113">String</span></span>|<span data-ttu-id="b23e5-114">应用的名称</span><span class="sxs-lookup"><span data-stu-id="b23e5-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="b23e5-115">关系</span><span class="sxs-lookup"><span data-stu-id="b23e5-115">Relationships</span></span>
<span data-ttu-id="b23e5-116">无</span><span class="sxs-lookup"><span data-stu-id="b23e5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b23e5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b23e5-117">JSON Representation</span></span>
<span data-ttu-id="b23e5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b23e5-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



