---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e6cb37078eb6c5b4aee00a9ac7bfc77061ec0bcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946593"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="12569-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="12569-103">omaSetting resource type</span></span>

> <span data-ttu-id="12569-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="12569-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12569-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="12569-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12569-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="12569-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12569-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="12569-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="12569-108">属性</span><span class="sxs-lookup"><span data-stu-id="12569-108">Properties</span></span>
|<span data-ttu-id="12569-109">属性</span><span class="sxs-lookup"><span data-stu-id="12569-109">Property</span></span>|<span data-ttu-id="12569-110">类型</span><span class="sxs-lookup"><span data-stu-id="12569-110">Type</span></span>|<span data-ttu-id="12569-111">说明</span><span class="sxs-lookup"><span data-stu-id="12569-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12569-112">displayName</span><span class="sxs-lookup"><span data-stu-id="12569-112">displayName</span></span>|<span data-ttu-id="12569-113">String</span><span class="sxs-lookup"><span data-stu-id="12569-113">String</span></span>|<span data-ttu-id="12569-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="12569-114">Display Name.</span></span>|
|<span data-ttu-id="12569-115">description</span><span class="sxs-lookup"><span data-stu-id="12569-115">description</span></span>|<span data-ttu-id="12569-116">String</span><span class="sxs-lookup"><span data-stu-id="12569-116">String</span></span>|<span data-ttu-id="12569-117">说明。</span><span class="sxs-lookup"><span data-stu-id="12569-117">Description.</span></span>|
|<span data-ttu-id="12569-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="12569-118">omaUri</span></span>|<span data-ttu-id="12569-119">String</span><span class="sxs-lookup"><span data-stu-id="12569-119">String</span></span>|<span data-ttu-id="12569-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="12569-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="12569-121">关系</span><span class="sxs-lookup"><span data-stu-id="12569-121">Relationships</span></span>
<span data-ttu-id="12569-122">无</span><span class="sxs-lookup"><span data-stu-id="12569-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12569-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12569-123">JSON Representation</span></span>
<span data-ttu-id="12569-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12569-124">Here is a JSON representation of the resource.</span></span>
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





