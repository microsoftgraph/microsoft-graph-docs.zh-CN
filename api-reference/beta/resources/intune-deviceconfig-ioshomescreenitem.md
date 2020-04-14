---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 74230d93a75edad64521f33dd25dfa8699fa270c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455146"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="d5789-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="d5789-103">iosHomeScreenItem resource type</span></span>

<span data-ttu-id="d5789-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5789-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5789-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5789-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5789-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5789-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5789-107">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="d5789-107">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="d5789-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5789-108">Properties</span></span>
|<span data-ttu-id="d5789-109">属性</span><span class="sxs-lookup"><span data-stu-id="d5789-109">Property</span></span>|<span data-ttu-id="d5789-110">类型</span><span class="sxs-lookup"><span data-stu-id="d5789-110">Type</span></span>|<span data-ttu-id="d5789-111">说明</span><span class="sxs-lookup"><span data-stu-id="d5789-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5789-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d5789-112">displayName</span></span>|<span data-ttu-id="d5789-113">String</span><span class="sxs-lookup"><span data-stu-id="d5789-113">String</span></span>|<span data-ttu-id="d5789-114">应用的名称</span><span class="sxs-lookup"><span data-stu-id="d5789-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5789-115">关系</span><span class="sxs-lookup"><span data-stu-id="d5789-115">Relationships</span></span>
<span data-ttu-id="d5789-116">无</span><span class="sxs-lookup"><span data-stu-id="d5789-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d5789-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d5789-117">JSON Representation</span></span>
<span data-ttu-id="d5789-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d5789-118">Here is a JSON representation of the resource.</span></span>
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



