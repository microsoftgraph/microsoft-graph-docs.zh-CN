---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 077c0eea7a4953d0cba3e9223a24fd9107f1b6c0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990251"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="16d8d-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="16d8d-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="16d8d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16d8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16d8d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16d8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16d8d-106">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="16d8d-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="16d8d-107">属性</span><span class="sxs-lookup"><span data-stu-id="16d8d-107">Properties</span></span>
|<span data-ttu-id="16d8d-108">属性</span><span class="sxs-lookup"><span data-stu-id="16d8d-108">Property</span></span>|<span data-ttu-id="16d8d-109">类型</span><span class="sxs-lookup"><span data-stu-id="16d8d-109">Type</span></span>|<span data-ttu-id="16d8d-110">说明</span><span class="sxs-lookup"><span data-stu-id="16d8d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16d8d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="16d8d-111">displayName</span></span>|<span data-ttu-id="16d8d-112">String</span><span class="sxs-lookup"><span data-stu-id="16d8d-112">String</span></span>|<span data-ttu-id="16d8d-113">应用的名称</span><span class="sxs-lookup"><span data-stu-id="16d8d-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="16d8d-114">关系</span><span class="sxs-lookup"><span data-stu-id="16d8d-114">Relationships</span></span>
<span data-ttu-id="16d8d-115">无</span><span class="sxs-lookup"><span data-stu-id="16d8d-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16d8d-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="16d8d-116">JSON Representation</span></span>
<span data-ttu-id="16d8d-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16d8d-117">Here is a JSON representation of the resource.</span></span>
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





