---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a30794ee909fffef098d643108a947cd1a540ff9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410628"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="2f4d7-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f4d7-103">iosHomeScreenItem resource type</span></span>

<span data-ttu-id="2f4d7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f4d7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f4d7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f4d7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f4d7-106">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="2f4d7-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="2f4d7-107">属性</span><span class="sxs-lookup"><span data-stu-id="2f4d7-107">Properties</span></span>
|<span data-ttu-id="2f4d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f4d7-108">Property</span></span>|<span data-ttu-id="2f4d7-109">类型</span><span class="sxs-lookup"><span data-stu-id="2f4d7-109">Type</span></span>|<span data-ttu-id="2f4d7-110">说明</span><span class="sxs-lookup"><span data-stu-id="2f4d7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f4d7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2f4d7-111">displayName</span></span>|<span data-ttu-id="2f4d7-112">String</span><span class="sxs-lookup"><span data-stu-id="2f4d7-112">String</span></span>|<span data-ttu-id="2f4d7-113">应用的名称</span><span class="sxs-lookup"><span data-stu-id="2f4d7-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f4d7-114">关系</span><span class="sxs-lookup"><span data-stu-id="2f4d7-114">Relationships</span></span>
<span data-ttu-id="2f4d7-115">无</span><span class="sxs-lookup"><span data-stu-id="2f4d7-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f4d7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f4d7-116">JSON Representation</span></span>
<span data-ttu-id="2f4d7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f4d7-117">Here is a JSON representation of the resource.</span></span>
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







