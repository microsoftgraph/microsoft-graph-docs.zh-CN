---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
ms.openlocfilehash: fa1fc438ef97357ebd5f13443077384bc98e24f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314040"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="65784-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="65784-103">omaSetting resource type</span></span>

> <span data-ttu-id="65784-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="65784-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="65784-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="65784-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65784-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="65784-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65784-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="65784-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="65784-108">属性</span><span class="sxs-lookup"><span data-stu-id="65784-108">Properties</span></span>
|<span data-ttu-id="65784-109">属性</span><span class="sxs-lookup"><span data-stu-id="65784-109">Property</span></span>|<span data-ttu-id="65784-110">类型</span><span class="sxs-lookup"><span data-stu-id="65784-110">Type</span></span>|<span data-ttu-id="65784-111">说明</span><span class="sxs-lookup"><span data-stu-id="65784-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65784-112">displayName</span><span class="sxs-lookup"><span data-stu-id="65784-112">displayName</span></span>|<span data-ttu-id="65784-113">String</span><span class="sxs-lookup"><span data-stu-id="65784-113">String</span></span>|<span data-ttu-id="65784-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="65784-114">Display Name.</span></span>|
|<span data-ttu-id="65784-115">description</span><span class="sxs-lookup"><span data-stu-id="65784-115">description</span></span>|<span data-ttu-id="65784-116">String</span><span class="sxs-lookup"><span data-stu-id="65784-116">String</span></span>|<span data-ttu-id="65784-117">说明。</span><span class="sxs-lookup"><span data-stu-id="65784-117">Description.</span></span>|
|<span data-ttu-id="65784-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="65784-118">omaUri</span></span>|<span data-ttu-id="65784-119">String</span><span class="sxs-lookup"><span data-stu-id="65784-119">String</span></span>|<span data-ttu-id="65784-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="65784-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65784-121">关系</span><span class="sxs-lookup"><span data-stu-id="65784-121">Relationships</span></span>
<span data-ttu-id="65784-122">无</span><span class="sxs-lookup"><span data-stu-id="65784-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65784-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65784-123">JSON Representation</span></span>
<span data-ttu-id="65784-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65784-124">Here is a JSON representation of the resource.</span></span>
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





