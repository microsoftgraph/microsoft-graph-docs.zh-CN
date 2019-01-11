---
title: numberRange 资源类型
description: 号码范围定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5b428320fd66263149b6d443a15c6a0e1eee744a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845701"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="f3257-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3257-103">numberRange resource type</span></span>

> <span data-ttu-id="f3257-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f3257-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3257-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f3257-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f3257-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f3257-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f3257-107">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="f3257-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="f3257-108">属性</span><span class="sxs-lookup"><span data-stu-id="f3257-108">Properties</span></span>
|<span data-ttu-id="f3257-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3257-109">Property</span></span>|<span data-ttu-id="f3257-110">类型</span><span class="sxs-lookup"><span data-stu-id="f3257-110">Type</span></span>|<span data-ttu-id="f3257-111">Description</span><span class="sxs-lookup"><span data-stu-id="f3257-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3257-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="f3257-112">lowerNumber</span></span>|<span data-ttu-id="f3257-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f3257-113">Int32</span></span>|<span data-ttu-id="f3257-114">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="f3257-114">Lower number.</span></span>|
|<span data-ttu-id="f3257-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="f3257-115">upperNumber</span></span>|<span data-ttu-id="f3257-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f3257-116">Int32</span></span>|<span data-ttu-id="f3257-117">上限数字。</span><span class="sxs-lookup"><span data-stu-id="f3257-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3257-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="f3257-118">Relationships</span></span>
<span data-ttu-id="f3257-119">无</span><span class="sxs-lookup"><span data-stu-id="f3257-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f3257-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3257-120">JSON Representation</span></span>
<span data-ttu-id="f3257-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3257-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```





