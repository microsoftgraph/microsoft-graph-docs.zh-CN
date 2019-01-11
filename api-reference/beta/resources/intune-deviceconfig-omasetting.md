---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b9abc7db7b6d2ad16aa13886905c348e6c8f01b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826472"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="b5da0-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5da0-103">omaSetting resource type</span></span>

> <span data-ttu-id="b5da0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b5da0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b5da0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b5da0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b5da0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5da0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5da0-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="b5da0-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="b5da0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b5da0-108">Properties</span></span>
|<span data-ttu-id="b5da0-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5da0-109">Property</span></span>|<span data-ttu-id="b5da0-110">类型</span><span class="sxs-lookup"><span data-stu-id="b5da0-110">Type</span></span>|<span data-ttu-id="b5da0-111">说明</span><span class="sxs-lookup"><span data-stu-id="b5da0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5da0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b5da0-112">displayName</span></span>|<span data-ttu-id="b5da0-113">String</span><span class="sxs-lookup"><span data-stu-id="b5da0-113">String</span></span>|<span data-ttu-id="b5da0-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="b5da0-114">Display Name.</span></span>|
|<span data-ttu-id="b5da0-115">description</span><span class="sxs-lookup"><span data-stu-id="b5da0-115">description</span></span>|<span data-ttu-id="b5da0-116">String</span><span class="sxs-lookup"><span data-stu-id="b5da0-116">String</span></span>|<span data-ttu-id="b5da0-117">说明。</span><span class="sxs-lookup"><span data-stu-id="b5da0-117">Description.</span></span>|
|<span data-ttu-id="b5da0-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="b5da0-118">omaUri</span></span>|<span data-ttu-id="b5da0-119">String</span><span class="sxs-lookup"><span data-stu-id="b5da0-119">String</span></span>|<span data-ttu-id="b5da0-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="b5da0-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5da0-121">关系</span><span class="sxs-lookup"><span data-stu-id="b5da0-121">Relationships</span></span>
<span data-ttu-id="b5da0-122">无</span><span class="sxs-lookup"><span data-stu-id="b5da0-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5da0-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5da0-123">JSON Representation</span></span>
<span data-ttu-id="b5da0-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5da0-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```





