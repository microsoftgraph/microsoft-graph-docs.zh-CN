---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8aecb99c036d3e8a5d89271afd6042ccb18b4fda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554651"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="8b015-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="8b015-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="8b015-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b015-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b015-105">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="8b015-105">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="8b015-106">属性</span><span class="sxs-lookup"><span data-stu-id="8b015-106">Properties</span></span>
|<span data-ttu-id="8b015-107">属性</span><span class="sxs-lookup"><span data-stu-id="8b015-107">Property</span></span>|<span data-ttu-id="8b015-108">类型</span><span class="sxs-lookup"><span data-stu-id="8b015-108">Type</span></span>|<span data-ttu-id="8b015-109">说明</span><span class="sxs-lookup"><span data-stu-id="8b015-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b015-110">displayName</span><span class="sxs-lookup"><span data-stu-id="8b015-110">displayName</span></span>|<span data-ttu-id="8b015-111">String</span><span class="sxs-lookup"><span data-stu-id="8b015-111">String</span></span>|<span data-ttu-id="8b015-112">应用的名称</span><span class="sxs-lookup"><span data-stu-id="8b015-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b015-113">关系</span><span class="sxs-lookup"><span data-stu-id="8b015-113">Relationships</span></span>
<span data-ttu-id="8b015-114">无</span><span class="sxs-lookup"><span data-stu-id="8b015-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b015-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8b015-115">JSON Representation</span></span>
<span data-ttu-id="8b015-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b015-116">Here is a JSON representation of the resource.</span></span>
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



