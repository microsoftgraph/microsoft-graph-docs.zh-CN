---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbde13f06df55b984aed8f2e0920a6ec3e3ce158
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835803"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="9ef02-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ef02-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="9ef02-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ef02-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ef02-105">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="9ef02-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="9ef02-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ef02-106">Properties</span></span>
|<span data-ttu-id="9ef02-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ef02-107">Property</span></span>|<span data-ttu-id="9ef02-108">类型</span><span class="sxs-lookup"><span data-stu-id="9ef02-108">Type</span></span>|<span data-ttu-id="9ef02-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ef02-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef02-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9ef02-110">displayName</span></span>|<span data-ttu-id="9ef02-111">String</span><span class="sxs-lookup"><span data-stu-id="9ef02-111">String</span></span>|<span data-ttu-id="9ef02-112">应用的名称</span><span class="sxs-lookup"><span data-stu-id="9ef02-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef02-113">关系</span><span class="sxs-lookup"><span data-stu-id="9ef02-113">Relationships</span></span>
<span data-ttu-id="9ef02-114">无</span><span class="sxs-lookup"><span data-stu-id="9ef02-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ef02-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ef02-115">JSON Representation</span></span>
<span data-ttu-id="9ef02-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ef02-116">Here is a JSON representation of the resource.</span></span>
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



