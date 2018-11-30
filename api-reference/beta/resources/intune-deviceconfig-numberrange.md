---
title: numberRange 资源类型
description: 号码范围定义。
ms.openlocfilehash: ef4b24e3034414221365d81c40b453e7ca66a94b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041812"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="29710-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="29710-103">numberRange resource type</span></span>

> <span data-ttu-id="29710-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="29710-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="29710-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="29710-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29710-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="29710-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="29710-107">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="29710-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="29710-108">属性</span><span class="sxs-lookup"><span data-stu-id="29710-108">Properties</span></span>
|<span data-ttu-id="29710-109">属性</span><span class="sxs-lookup"><span data-stu-id="29710-109">Property</span></span>|<span data-ttu-id="29710-110">类型</span><span class="sxs-lookup"><span data-stu-id="29710-110">Type</span></span>|<span data-ttu-id="29710-111">说明</span><span class="sxs-lookup"><span data-stu-id="29710-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29710-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="29710-112">lowerNumber</span></span>|<span data-ttu-id="29710-113">Int32</span><span class="sxs-lookup"><span data-stu-id="29710-113">Int32</span></span>|<span data-ttu-id="29710-114">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="29710-114">Lower number.</span></span>|
|<span data-ttu-id="29710-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="29710-115">upperNumber</span></span>|<span data-ttu-id="29710-116">Int32</span><span class="sxs-lookup"><span data-stu-id="29710-116">Int32</span></span>|<span data-ttu-id="29710-117">上限数字。</span><span class="sxs-lookup"><span data-stu-id="29710-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29710-118">Relationships</span><span class="sxs-lookup"><span data-stu-id="29710-118">Relationships</span></span>
<span data-ttu-id="29710-119">无</span><span class="sxs-lookup"><span data-stu-id="29710-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="29710-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29710-120">JSON Representation</span></span>
<span data-ttu-id="29710-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29710-121">Here is a JSON representation of the resource.</span></span>
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





