---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b6d5fcea7b3b46acf8d0a119213f679d99aed6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961482"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="40b46-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="40b46-103">omaSetting resource type</span></span>

> <span data-ttu-id="40b46-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="40b46-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40b46-105">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="40b46-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="40b46-106">属性</span><span class="sxs-lookup"><span data-stu-id="40b46-106">Properties</span></span>
|<span data-ttu-id="40b46-107">属性</span><span class="sxs-lookup"><span data-stu-id="40b46-107">Property</span></span>|<span data-ttu-id="40b46-108">类型</span><span class="sxs-lookup"><span data-stu-id="40b46-108">Type</span></span>|<span data-ttu-id="40b46-109">说明</span><span class="sxs-lookup"><span data-stu-id="40b46-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40b46-110">displayName</span><span class="sxs-lookup"><span data-stu-id="40b46-110">displayName</span></span>|<span data-ttu-id="40b46-111">String</span><span class="sxs-lookup"><span data-stu-id="40b46-111">String</span></span>|<span data-ttu-id="40b46-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="40b46-112">Display Name.</span></span>|
|<span data-ttu-id="40b46-113">description</span><span class="sxs-lookup"><span data-stu-id="40b46-113">description</span></span>|<span data-ttu-id="40b46-114">String</span><span class="sxs-lookup"><span data-stu-id="40b46-114">String</span></span>|<span data-ttu-id="40b46-115">说明。</span><span class="sxs-lookup"><span data-stu-id="40b46-115">Description.</span></span>|
|<span data-ttu-id="40b46-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="40b46-116">omaUri</span></span>|<span data-ttu-id="40b46-117">String</span><span class="sxs-lookup"><span data-stu-id="40b46-117">String</span></span>|<span data-ttu-id="40b46-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="40b46-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40b46-119">关系</span><span class="sxs-lookup"><span data-stu-id="40b46-119">Relationships</span></span>
<span data-ttu-id="40b46-120">无</span><span class="sxs-lookup"><span data-stu-id="40b46-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="40b46-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="40b46-121">JSON Representation</span></span>
<span data-ttu-id="40b46-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40b46-122">Here is a JSON representation of the resource.</span></span>
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



