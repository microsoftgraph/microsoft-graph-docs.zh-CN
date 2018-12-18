---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
ms.openlocfilehash: 168214da57f2cc903bac110709d721061d4298cd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362515"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="160b8-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="160b8-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="160b8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="160b8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="160b8-105">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="160b8-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="160b8-106">属性</span><span class="sxs-lookup"><span data-stu-id="160b8-106">Properties</span></span>
|<span data-ttu-id="160b8-107">属性</span><span class="sxs-lookup"><span data-stu-id="160b8-107">Property</span></span>|<span data-ttu-id="160b8-108">类型</span><span class="sxs-lookup"><span data-stu-id="160b8-108">Type</span></span>|<span data-ttu-id="160b8-109">说明</span><span class="sxs-lookup"><span data-stu-id="160b8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="160b8-110">displayName</span><span class="sxs-lookup"><span data-stu-id="160b8-110">displayName</span></span>|<span data-ttu-id="160b8-111">String</span><span class="sxs-lookup"><span data-stu-id="160b8-111">String</span></span>|<span data-ttu-id="160b8-112">应用的名称</span><span class="sxs-lookup"><span data-stu-id="160b8-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="160b8-113">关系</span><span class="sxs-lookup"><span data-stu-id="160b8-113">Relationships</span></span>
<span data-ttu-id="160b8-114">无</span><span class="sxs-lookup"><span data-stu-id="160b8-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="160b8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="160b8-115">JSON Representation</span></span>
<span data-ttu-id="160b8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="160b8-116">Here is a JSON representation of the resource.</span></span>
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



