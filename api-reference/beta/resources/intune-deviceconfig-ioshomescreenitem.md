---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 477be5c509ab4d062a695c4b8df7eb00af6f51fe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962602"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="b4e8e-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4e8e-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="b4e8e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b4e8e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b4e8e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b4e8e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b4e8e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b4e8e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b4e8e-107">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="b4e8e-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="b4e8e-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4e8e-108">Properties</span></span>
|<span data-ttu-id="b4e8e-109">属性</span><span class="sxs-lookup"><span data-stu-id="b4e8e-109">Property</span></span>|<span data-ttu-id="b4e8e-110">类型</span><span class="sxs-lookup"><span data-stu-id="b4e8e-110">Type</span></span>|<span data-ttu-id="b4e8e-111">说明</span><span class="sxs-lookup"><span data-stu-id="b4e8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4e8e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b4e8e-112">displayName</span></span>|<span data-ttu-id="b4e8e-113">String</span><span class="sxs-lookup"><span data-stu-id="b4e8e-113">String</span></span>|<span data-ttu-id="b4e8e-114">应用的名称</span><span class="sxs-lookup"><span data-stu-id="b4e8e-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4e8e-115">关系</span><span class="sxs-lookup"><span data-stu-id="b4e8e-115">Relationships</span></span>
<span data-ttu-id="b4e8e-116">无</span><span class="sxs-lookup"><span data-stu-id="b4e8e-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b4e8e-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4e8e-117">JSON Representation</span></span>
<span data-ttu-id="b4e8e-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4e8e-118">Here is a JSON representation of the resource.</span></span>
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





